# Delivery & Acceptance：交付与验收

## 适用场景与发送时机

| 项目 | 使用说明 |
| --- | --- |
| 流程/阶段 | 阶段成果、文档、软件包或服务交接的交付与验收准备 |
| 触发条件 | 指定版本已达到约定交付条件，接收者能够访问，并需要按明确标准检查；未完成的交付只报告实际就绪部分 |
| To / CC | To：已知接收人及有本次验收职责的人；CC：用户指定的交付/项目负责人。收到文件的人不自动成为验收批准人 |
| 发送前准备 | 交付清单、版本与位置、适用范围、已执行验证及证据、验收标准、已知限制和未决项 |
| 期望反馈/时间 | 确认收到/可访问；另按标准提供验收结果或未满足项。请求验收时间与已约定验收窗口分清，不以沉默自动验收 |

## 完整英文 Sample

To: [Recipient]; [Acceptance owner]

Cc: [Confirmed CC recipients]

Subject: [Project] Delivery for Acceptance – [Deliverable and Version]

Dear [Recipient] and [Acceptance owner],

We are delivering [Deliverable and Version] for acceptance against [agreed criteria reference].

- Scope: [Included items and applicable environment or process].
- Delivery location: [Verified attachment name or approved shared location].
- Checks completed: [Actual checks and results, with evidence reference].
- Known limitations or open items: [Known items and their impact; state none only if verified].

The attached Delivery_Acceptance_Register.csv records the delivery items, version references and acceptance criteria. Please refer to DEL-01 for [principal deliverable] and DEL-02 for [supporting evidence or document].

Could you please confirm receipt and access, and provide the acceptance results by [Requested response deadline]? Please record any unmet criteria and supporting evidence against the relevant delivery ID.

Delivery and receipt confirmation do not constitute acceptance; we are requesting your explicit acceptance result for the stated scope.

Thank you for reviewing the delivery.

Best regards,

[Sender name]

## 附件 Sample

[下载 Delivery_Acceptance_Register.csv](../../assets/attachments/Delivery_Acceptance_Register.csv)。此文件是交付/验收登记表示例，不包含真正的软件包或验收报告。

| DeliveryID | DeliverableAndVersion | Location | AcceptanceCriteria | AcceptanceStatus |
| --- | --- | --- | --- | --- |
| DEL-01 | [Principal deliverable/version] | [Verified location] | [Criterion and reference] | Pending acceptance |
| DEL-02 | [Supporting document/version] | [Verified location] | [Criterion and reference] | Pending acceptance |

CSV 另列验证证据、已知未决项、验收人、实际验收结果及请求反馈时间。验收状态只能由本次证据支持，不根据文件可下载就填 `Accepted`。

## 写作解读与表达建议

- **开场/背景**：明确为哪个版本、依据什么标准交付，避免只写 `The work is done`。
- **现状/证据**：范围、位置、已做检查和限制并列，接收方可快速判断是否具备验收条件。
- **行动/结尾**：分别请求 receipt/access 与 acceptance result；未满足项要求对应标准及证据，便于闭环。
- 推荐 `ready for acceptance against [criteria]`；避免 `Please acknowledge, then we will consider it accepted`。

## 注意事项

仅供测试的包应写明用途，不能称生产发布。验收标准未知且影响结论时先澄清；可准备交付草稿，但不虚构标准或通过结果。原始包、报告和清单都须实际核对；未提供的验证不能从附件样例复制。未明确提供的合同条款、静默验收、质保起点和付款条件不加入邮件。附件未附按[复制规则](../external-communication.md#复制使用与事实边界)处理。

起草时文件尚未附入，默认在稿外标“待附上/提供访问位置”，不把本地发信准备过程写给客户。正文可写文件已就绪，并请求对方在收到后确认及安排验收；发送前必须实际提供文件，不能把缺少交付物的草稿称为可直接发送。
