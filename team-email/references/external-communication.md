# 对外邮件沟通手册

用于客户、供应商和合作伙伴之间的项目协作。先选沟通目的，再选场景；只读相关场景，不把整份手册或全部栏目塞进一封邮件。现有会议、交接、变更、短回复等[通用模板](templates.md)继续适用。

## Communication Type：八类核心沟通

| 类型 | 业务阶段与目的 | 完整场景与英文 Sample | 对应原模板 |
| --- | --- | --- | --- |
| Information Request | 启动、需求、设计、准备：取得缺少的信息或资源 | [信息或资料请求](external-scenarios/01-information-request.md) | 1 |
| Clarification | 需求、设计、开发、验收前：消除规则或理解差异 | [问题澄清](external-scenarios/02-clarification.md) | 3 |
| Progress Update | 执行、测试、交付准备：同步已完成、当前状态和下一步 | [进展汇报](external-scenarios/03-progress-update.md) | 6 |
| Issue Follow-up | 调查、处理、验证：追踪已提出但仍需核实的事项 | [问题跟进与催办](external-scenarios/04-issue-follow-up.md) | 9 |
| Issue Escalation | 发生重大影响或现有路径无法解除阻塞：请求协调或决定 | [重要问题升级](external-scenarios/05-issue-escalation.md) | 9 的升级场景 |
| Review & Confirmation | 基线或下一阶段开始前：取得评审反馈及指定范围的确认 | [评审与确认](external-scenarios/06-review-confirmation.md) | 2/5 |
| Delivery & Acceptance | 可交付物已就绪：交付明确版本并请求按标准验收 | [交付与验收](external-scenarios/07-delivery-acceptance.md) | 7/13 |
| Issue Closure | 指定范围验证完成：请求确认关闭或记录已有关闭决定 | [问题关闭](external-scenarios/08-issue-closure.md) | 13 |

类别是选模板的辅助信息，不默认把 `Communication Type` 等内部分类栏目写进收件人的正文。一封邮件保留一个主要目的；跟进不等于升级，交付不等于验收，修复不等于关闭。

## 复制使用与事实边界

1. 每个场景都提供流程阶段、触发条件、To/CC、准备资料、反馈要求、完整英文 Sample、可下载 CSV 附件 Sample、写作解读和注意事项。方括号是待替换字段，不是已确认业务事实；编号仅用于对应示例，不代表真实工单。
2. 选择最贴近实际的场景，替换项目、联系人、事项、版本、日期和附件信息。删去不适用段落及无依据的状态、影响、原因或承诺；不能从 Sample 补造本次事实。已有草稿仍默认最小修改，不为套模板强行重组。
3. `To` 放已知的行动或决策负责人；`CC` 仅保留用户指定或已确认需知情的人，没有则删除整行。角色建议不授权搜索联系人、添加管理层、回复全部或扩大共享范围。
4. 所有时间字段用 `DD Mon YYYY, HH:mm, UTC±HH:mm`。`[Requested response deadline]` 是本次提出的反馈请求，不伪装为已约定期限；用户未给日期时，改问可提供时间。`[Confirmed next update]` 等承诺字段只有已有明确安排才保留，否则省略或列待补，不自行承诺 24/48 小时、EOD 或下一次更新时间。
5. 下载的 CSV 是待填示例，不是测试证据、报告或已附文件。先填入并核对实际内容，再按需改名；正文文件名、条目编号和附件内容保持一致。转成 XLSX/PDF 后同步修改引用，不把 CSV 样例当成真实验证结果。
6. Sample 中的 `attached` 仅在实际附件已核实且已附入邮件时保留。仅有文件或生成稿时，在正文外列“待附上”；未核实附入时改为 `The checklist below...` 等正文内信息，或使用用户提供的受控共享位置，不宣称已发送/已上传/已附。引用附件只依据实际读到的内容。
7. 邮件正文保留关键结论及证据定位，附件承载完整明细。外发前核对收件范围、保密边界和脱敏；模板不给合同解释、责任归属、批准、验收或关闭权限。

具体发信稿中，附件尚未附入、未提供共享链接、用户没有给起草者反馈日期或备选方案，通常属于准备信息：在稿外列待补或省略，不逐条写给客户。除非用户明确要通知材料暂缺、延期等业务情况，否则不写 `The file has not yet been attached` 或 `No shared link is available`；可介绍待交付文件，并请求对方在收到后确认。真实业务状态未知但会影响处理时（例如恢复时间尚未确定），仍应在正文准确说明。

## 六个写作模块：何时用、怎么写

### 3.1 Greeting & Opening：问候与开场

- 新的正式外部线程可用 `Dear [Name],`；已建立工作关系的简短回复可沿用 `Hi [Name],`。多名行动人逐一称呼或用已知团队名称；不猜称谓、性别或头衔。
- 第一段直接交代目的、影响和请求。确实收到输入时可用 `Thank you for sharing [specific input].`；初次联系可一句说明相关职责，不铺陈无关经历。
- `I hope you are well.` 可用于久未联系，但不是必填。重要问题优先说明事实，不用客套话掩盖请求。
- 确有需要且事实支持时致歉，例如已核实由己方造成的影响；责任未清时用 `We understand the impact on [activity].` 回应影响，不凭空认错、承诺赔偿或代他人道歉。

### 3.2 Background & Context：背景与上下文

- 用一两句交代原请求/讨论日期、文件版本、当前差异和下一步依赖。`Following your email of [date], ...` 定位来源；`Our current understanding is ...` 表明仍待确认。
- 只有存在确认记录才写 `As agreed, ...`；讨论过不等于达成共识。回复只补新信息，不重写整段历史或转贴长引用。

### 3.3 Progress & Current Status：进展与状态

- 按实际需要写 `Completed / In progress / Pending / Next step`，用产出及证据描述进展，而非仅列开会、看文档等活动。
- `The fix has been deployed to UAT; validation is pending.` 区分部署和验证。明确报告日期、范围与来源，不从局部完成推断总体完成。
- `At risk` 需要依赖或目标差异支撑；没有总量不写完成百分比。目标、新预计、已承诺日期分开，未知完成时间如实说明。

### 3.4 Supporting Evidence：支撑材料

- 正文写结论、关键数值/预期与实际及位置：`The result is [finding]. See [file], [section/table/row or case ID].`
- 测试写环境、版本、范围、用例及实际结果；截图写编号和对应现象；日志给脱敏片段、时间及关联 ID；交付物给版本、位置及已做的检查。来源不匹配时列待核对，不拼成一次调用或一个结果。
- `Please see the attachment.` 不足以支撑结论；正文至少说明相关发现及希望对方如何处理。不把文件已收到、数据已提供或某轮测试通过当作方案批准或整体验收。

### 3.5 Action Required：行动请求

- 使用明确动词：`provide` 索取资料、`clarify` 澄清含义、`review` 征求意见、`confirm` 确认指定事项、`approve` 请求有权限者批准、`verify` 核实行为。不要混用。
- 示例：`Could you please confirm [specific item/version] by [requested response deadline] so that we can [dependent next step]?` 未给期限时改为 `Could you please advise when you can provide your response?`
- 多项请求编号并对应负责人、回答格式和反馈时点；责任未知且影响动作时询问，不从职位推断审批权。纯进度通知无需硬加确认请求。
- 请求对方给预计时间，不等于承诺己方按该时间完成；升级邮件请求具体决定/资源，不仅写 `Please escalate.`。

### 3.6 Closing：结束语

- 请求/澄清：`Thank you for your help with [specific matter].`
- 跟进：`Thank you for helping us confirm the next steps.`
- 升级：`Thank you for your support in resolving this dependency.`
- 评审/验收请求：`Thank you for reviewing [deliverable/scope].` 表达对所请求工作的感谢，不代表已经评审通过。
- 通知：`Please let us know if you identify any inaccuracies.`；确为无需动作时可写 `No action is required at this stage.`。
- 最后使用 `Best regards,` 及已核实签名，不堆叠多段致谢、祝愿或虚构联系方式。

## 常见表达改进

| 避免或谨慎使用 | 更自然、具体的表达 | 原因 |
| --- | --- | --- |
| Please kindly help to check. | Could you please check [specific item] and share [expected result]? | 去掉重复客套，明确产出 |
| Please do the needful. | Please provide [item] / confirm [decision]. | 避免让对方猜动作 |
| Please revert ASAP. | Could you please respond by [requested date/time/UTC offset]? | `respond` 更通用，时间可执行 |
| Kindly confirm whether is OK. | Could you please confirm whether [specific approach] meets [criterion]? | 完整从句及判断标准 |
| We already discussed and confirmed. | We discussed [item] on [date]; [decision] is still awaiting confirmation. | 讨论与确认分开，以实际记录为准 |
| The issue has been solved. | [Fix/deployment/verification status and exact scope]. | 避免把修复报告扩大为验证通过 |
| Sorry to disturb you again. | I am following up on [request] because [confirmed dependency]. | 说明正当跟进原因，无需为正常协作过度致歉 |
| You did not reply, so we consider it approved. | Approval is still pending; could you please confirm [decision]? | 沉默不构成批准 |

这些是本工作流的推荐表达，不按国籍或口音评价作者。已有英文受“原样保留”约束时，只在正文外给建议，不静默改写。

## 发送前最小核对

- 类别、目的、行动人、反馈内容和时间是否清楚？是否确需回复？
- 已完成、计划、推测、确认、批准、验收和关闭是否有各自依据？
- 方括号是否已替换或在草稿外列待补？所有事实与承诺是否来自本次材料？
- To/CC 是否已确认，实际附件是否齐全、版本正确、可访问且符合外发边界？
- 标题、正文、附件条目与中英两稿是否一致？不得因模板完整而跳过这些核对。
