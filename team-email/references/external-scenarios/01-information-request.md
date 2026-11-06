# Information Request：信息或资料请求

## 适用场景与发送时机

| 项目 | 使用说明 |
| --- | --- |
| 流程/阶段 | 项目启动、需求分析、方案设计、开发或测试准备 |
| 触发条件 | 缺少明确的信息、数据、文档或资源，下一步依赖尚未满足；首次索取用本类，已提出请求后的追踪用 Issue Follow-up |
| To / CC | To：已知资料或资源提供人；CC：用户已确认需知情的任务负责人。未知提供人时请求指引，不自行添加联系人 |
| 发送前准备 | 缺口清单、用途、格式/范围、已有材料及差异、可外发边界、用户给出的反馈请求时间 |
| 期望反馈/时间 | 按条目提供资料或可用位置；不能提供时说明限制和预计可提供时间。期限未知则询问预计时间 |

## 完整英文 Sample

To: [Information owner]

Cc: [Confirmed CC recipients]

Subject: [Project] Request for [Required Information]

Dear [Information owner],

Could you please provide the information below so that we can prepare for [next activity]?

We are currently working on [current task]. We have [available input], but still need the following items:

1. REQ-01 — [Required item 1], covering [scope] in [format].
2. REQ-02 — [Required item 2], including [specific fields or details].

The attached Information_Request_Checklist.csv lists each item, its purpose and the requested format. Please add your response or the relevant document reference against each request ID.

Could you please provide these items by [Requested response deadline]? If any item cannot be provided by then, please let us know what is available and its expected availability date.

Thank you for your help with [next activity].

Best regards,

[Sender name]

## 附件 Sample

[下载 Information_Request_Checklist.csv](../../assets/attachments/Information_Request_Checklist.csv)。它是待填清单，不是已取得的资料。

| RequestID | RequiredInformation | FormatOrScope | Purpose | ResponseOrReference |
| --- | --- | --- | --- | --- |
| REQ-01 | [Required item 1] | [Scope and format] | [Dependent activity] | [Provider to complete] |
| REQ-02 | [Required item 2] | [Required fields] | [Dependent activity] | [Provider to complete] |

CSV 还包含提供人及请求反馈时间。实际发出前填实必要字段；对方待填写的列可标 `Pending response`，不能填成已提供。

## 写作解读与表达建议

- **开场/背景**：先说要什么、用于什么，再说明已有输入，避免泛泛请求“所有相关资料”。
- **现状/证据**：只列已知缺口；REQ 编号连接正文与附件，方便逐项回复。
- **行动/结尾**：同时给“可以提供”和“暂不能提供”的回答路径；`expected availability date` 是询问，不是己方承诺。
- 推荐 `Could you please provide... so that we can...?`；避免 `Please do the needful` 或 `Please send all documents ASAP`。

## 注意事项

未知时间时，把期限句改为 `Could you please advise when these items will be available?`。没有已核实的已有输入时删除 `We have...`。附件尚未附入时按[复制规则](../external-communication.md#复制使用与事实边界)改写并列待附上。请求生产数据或客户资料时遵循已知共享规则，不在邮件索要密码、Secret 或原始敏感数据。
