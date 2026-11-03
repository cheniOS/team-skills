# 接口问题邮件与日志脱敏

适用于后端、App、测试或 QA 向接口负责方反馈问题。正文让读者立即理解“哪个接口、什么环境、何时发生、预期和实际差异、如何查到、需要做什么”。不凭 HTTP 状态码推断确定根因或责任方。

## 正文信息顺序

1. 一句话说明现象和已确认影响。
2. 接口定位：环境、HTTP method、host（确有必要时）与 path、API 版本、相关服务/App build、发生时间及明确时区、可用于查日志的 request ID/trace ID。
3. 预期与实际：HTTP status、业务 code/message、关键返回字段或耗时及单位；两类状态不要混淆。例如 HTTP 200 也可能带业务失败码。
4. 最小复现：必要前置条件、步骤、相关请求字段、必要 headers。不同环境对比时明确每组版本、条件和结果，不将不同请求当作严格同条件对照。
5. 正文贴一组脱敏的请求/响应和少量相邻日志，保留同一次请求的关联关系。长日志放脱敏附件，并写出文件名、时间范围、行号（已核实时）或请求 ID。
6. 明确请求：请核查什么、是否需确认契约/部署/配置、希望返回调查结果/方案/预计时间。解决时间未知时可请求下一次调查更新时间。区分已知根因与尚待验证的判断，仅在本次材料支持时报告复现频次、数量和影响范围。

字段按实际需要取舍；资料不足用占位或在邮件外列待补项，不编造调用、日志、数据或定位。

## 脱敏边界

| 数据 | 邮件处理方式 |
| --- | --- |
| Authorization、access/refresh token、API key、client secret、密码、Cookie/Set-Cookie、session token、签名密钥、私钥 | 删除完整值或替换为 `<REDACTED>`；诊断需要时保留 header/字段名及鉴权类型，不保留凭据首尾片段。测试环境凭据也一样 |
| URL query、path、body、错误 message/stack trace 中的同类秘密，带临时签名的下载链接 | 同样脱敏；不要以为没有 Authorization header 就没有秘密 |
| 姓名、手机号、邮箱、证件、账号、卡号等个人或客户标识 | 省略无关字段；必要关联用一致的 `[USER_A]`、`[CARD_A]` 等替代标识。避免同一值前后换不同代号，或不同值混成一个代号 |
| 支付卡完整号码、安全码、PIN、完整支付敏感载荷 | 不放入普通邮件正文、截图或附件；只保留必要非敏感状态与获准共享的定位信息 |
| request ID、trace ID、非敏感业务流水号 | 为协查保留必要值，但先检查是否含个人数据、秘密或本身用于访问资源。确需遮蔽时标明已替换，并通过双方认可的受控渠道提供真实定位值，不能把代号冒充可查询的 ID |
| method、接口 path/版本、环境、时间及时区、HTTP status、业务错误码、字段名、耗时与单位 | 通常保留以支持定位；path 中的个人标识或秘密单独替换，不把整个接口信息都遮掉 |
| 内部 host/IP、堆栈、服务路径、配置 | 仅保留接收方排查所需且获准共享的部分；不为无关上下文附上完整拓扑或配置。示例一律用 example.com 等占位域名 |

脱敏同时适用于正文、附件、截图、复制的 curl/HAR、历史引用和文件名。截图应移除敏感区域或使用不可恢复的实心覆盖，不用模糊或可移除遮罩。只处理本次准备共享的副本，不覆盖用户的原始证据。

保留结构和问题条件：不要删掉触发问题所需的字段、大小写、类型、空值/缺省差异而不说明。遮蔽导致类型或格式变化时，标明示例不可直接执行；JSON 字符串中的 `<REDACTED>` 也只是占位符。若安全排查必须使用真实敏感载荷，应按团队已有受控渠道共享，不随普通邮件发送。

## 可复制邮件骨架

以下全部是占位模板，并非真实调用。替换前核对材料；只保留相关小节。代码块仅供展示请求/响应/日志，在邮件中使用等宽文本或代码样式，不用代码围栏包住整封信。

Subject: [Project][Environment] API Issue – [Operation] Returns [HTTP Status / Business Error]

Dear [Team Name] Team,

Could you please investigate [issue] when calling [operation]? This is affecting [confirmed scope]. The relevant request and evidence are provided below.

Context:
- Environment: [Environment]
- API: [METHOD] [Host if needed]/[API path and version]
- Client/service version: [Version or build, if relevant]
- Timestamp: [Date and time with UTC offset]
- Request ID / Trace ID: [Actual non-sensitive ID suitable for lookup]

Expected: [Expected HTTP/business result]
Actual: [Observed HTTP status, business code/message and relevant fields]

Reproduction:
1. [Required precondition]
2. [Action and relevant input]

Relevant request and response (sanitized):

```http
[METHOD] /[API path]
Content-Type: application/json
Authorization: <REDACTED>
```

```json
{
  "relevantField": "[Actual non-sensitive value or explicitly marked replacement]"
}
```

Response: HTTP [Actual status]

```json
{
  "code": "[Actual business code]",
  "message": "[Actual message with any sensitive values redacted]"
}
```

Relevant log excerpt (sanitized):

```text
[timestamp with offset] [level] requestId=[same actual ID] method=[METHOD] path=[path] status=[status] durationMs=[actual value]
[timestamp with offset] [level] requestId=[same actual ID] code=[actual code] message="[relevant sanitized message]"
```

Attachment reference: [Sanitized file name], [time range and request ID / verified line range]. [Brief summary of additional evidence.]

Please check [specific routing, contract, deployment or processing question] and share your findings and proposed next steps. If the resolution time cannot yet be confirmed, please advise when the next investigation update can be provided.

Authentication credentials and unrelated personal information have been redacted.

Thank you for your support.

Best regards,
[Signature]

## 发送前检查

- 请求、响应、时间、ID、环境是否对应同一次调用？日志是否支持正文结论？
- HTTP status 和业务 code 是否分别标明，是否把 404/500 等现象误写为已证实的部署或代码根因？
- 正文是否已含最小关键证据，完整脱敏附件是否有可搜索定位？
- URL、headers、body、日志、截图、附件及引用是否仍含凭据或无关个人信息？
- 占位值/脱敏值是否明确标记？是否错误地声称所有内容都已脱敏或附件已添加，而实际未核对？
- 解决时间与下次更新时间是否区分？已确认的跟进安排是否写明日期、时间和当日 UTC 偏移，且没有凭空承诺？
