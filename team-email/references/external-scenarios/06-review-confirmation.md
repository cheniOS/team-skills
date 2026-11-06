# Review & Confirmation：评审与确认

## 适用场景与发送时机

| 项目 | 使用说明 |
| --- | --- |
| 流程/阶段 | 需求/设计基线、实施前评审、测试方案确认或阶段切换 |
| 触发条件 | 已形成明确版本和待评审点，需要反馈或指定范围的确认后才能执行下一步 |
| To / CC | To：已知评审人和确认人；同一人可兼任。CC：用户指定的实施或依赖负责人；普通评审人不自动拥有审批权 |
| 发送前准备 | 文件及版本、相关章节、主要变化、待确认事项、适用约束、希望返回的反馈形式和已知反馈时间 |
| 期望反馈/时间 | 逐项给评审意见及确认/待修改结论；如需正式批准，另外明确有权批准的人、版本和批准范围 |

## 完整英文 Sample

To: [Reviewer]; [Confirmation owner]

Cc: [Confirmed CC recipients]

Subject: [Project] Review and Confirmation Required – [Deliverable and Version]

Dear [Reviewer] and [Confirmation owner],

Please review [Deliverable and Version] and confirm [specific scope] before we proceed with [next activity].

This version covers [scope]. The main change from [previous reference, if available] is [verified change and its impact].

The points requiring your attention are:

1. REV-01 — [Reviewer], please review [specific section or criterion] and identify any changes needed.
2. REV-02 — [Confirmation owner], please confirm [specific rule or scope] against [reference or criterion].

The attached Review_Confirmation_Log.csv lists the source references and the response required for each item. Please record your comments and confirmation status against the relevant review ID.

Could you please return your feedback by [Requested response deadline]? If any point needs further discussion, please identify the item and the information needed to resolve it.

Thank you for reviewing [Deliverable and Version].

Best regards,

[Sender name]

## 附件 Sample

[下载 Review_Confirmation_Log.csv](../../assets/attachments/Review_Confirmation_Log.csv)。评审意见与确认结论分列，未确认时保留待确认状态。

| ReviewID | DeliverableVersionReference | ReviewPoint | RequiredResponse | ConfirmationStatus |
| --- | --- | --- | --- | --- |
| REV-01 | [File/version/section] | [Review scope] | [Comments or required changes] | Pending review |
| REV-02 | [File/version/section] | [Rule or scope] | [Confirm or identify changes] | Pending confirmation |

CSV 另列实际评审人、意见/答复和请求反馈时间。`No comments` 不自动等于 `Approved`。

## 写作解读与表达建议

- **开场/背景**：指定版本和下一步依赖，避免对方不清楚本次评审哪份材料。
- **现状/证据**：变化有前版依据才比较；REV 编号及章节把反馈定位到具体点，降低反复澄清成本。
- **行动/结尾**：分别要求 review 和 confirm，注明谁回答哪项；`identify any changes needed` 给出可否定/可修改的回答路径。
- 推荐 `Please confirm whether [scope] meets [criterion]`；避免含糊的 `Please check and approve everything`。

## 注意事项

评审人和确认人相同时合并称呼及 To，不重复名字。只要求意见时删确认项，不将评审包装成审批；正式审批须有本次明确的授权人和批准范围。没有反馈时间改问可反馈日期；沉默不视为批准。正文引用的主文件也须提供实际文件/受控位置；日志不能替代待评审材料。附件未附按[复制规则](../external-communication.md#复制使用与事实边界)处理。
