# Issue Closure：问题关闭

## 适用场景与发送时机

| 项目 | 使用说明 |
| --- | --- |
| 流程/阶段 | 修复后验证、复测结果确认及问题生命周期收尾 |
| 触发条件 | 约定范围的验证已完成且证据可定位；关闭仍待有权者确认时发关闭确认请求，已有明确关闭决定时可发通知 |
| To / CC | To：已知验证/关闭确认人或原问题负责人；CC：用户指定的受影响团队。不能依据职位或抄送推断关闭权限 |
| 发送前准备 | 原问题、版本/环境、验证范围与结果、证据、剩余限制，以及关闭决定的真实状态/来源 |
| 期望反馈/时间 | 对指定问题和范围明确确认是否可关闭；已有关闭决定的通知不再制造待批准事项。未验证时转 Verification Required，而非请求直接关闭 |

## 完整英文 Sample：请求确认关闭

To: [Closure confirmation owner]

Cc: [Confirmed CC recipients]

Subject: [Project] Closure Confirmation Requested – [Issue ID]

Dear [Closure confirmation owner],

Verification of [Issue ID and symptom] has been completed for [Version and Environment]. We would like to request your confirmation to close this issue for the scope below.

- Verified scope: [Behavior and cases actually checked].
- Result: [Actual verification result].
- Evidence: [Report/log reference and section, row or case ID].
- Remaining limitations: [Known limitations, or none if verified].

The attached Issue_Closure_Record.csv links the original issue, verification evidence and proposed closure scope. CLS-01 identifies the result supporting this request.

Could you please confirm whether the issue can be closed for this scope by [Requested response deadline]? If further verification is required, please identify the missing check or evidence.

Closure remains pending until your confirmation is received.

Thank you for your support in verifying the outcome.

Best regards,

[Sender name]

## 附件 Sample

[下载 Issue_Closure_Record.csv](../../assets/attachments/Issue_Closure_Record.csv)。默认 `Pending confirmation` 是请求阶段的状态，不能替代真实验证或关闭记录。

| ClosureID | IssueReference | VersionAndEnvironment | VerifiedScope | VerificationResult | ClosureStatus |
| --- | --- | --- | --- | --- | --- |
| CLS-01 | [Original issue] | [Actual version/environment] | [Checked behavior/cases] | [Actual result] | Pending confirmation |

CSV 另列证据位置、剩余限制及关闭确认来源。若已有关闭决定，用真实记录填写确认人、日期及状态，不从请求本身推断已关闭。

## 写作解读与表达建议

- **开场/背景**：写已验证的具体版本/环境，并明确这是请求关闭，不让 `fixed` 自动变为 `closed`。
- **现状/证据**：把复测范围、实际结果及限制留在正文；附件建立原问题到验证和确认的关系。
- **行动/结尾**：给确认或指出缺失证据的回答路径；不以未回复作为默认关闭条件。
- 推荐 `Please confirm whether the issue can be closed for this scope`；避免 `It is fixed, so we have closed the issue`，除非关闭决定已有依据。

## 已确认关闭时的通知变体

仅在本次材料明确提供关闭决定时使用；将登记表更新为实际状态。

Subject: [Project] Issue Closure Notice – [Issue ID]

Dear [Name],

Following [Confirmed decision reference], [Issue ID] was closed on [Confirmed closure date] for [Version, Environment and Scope].

Verification covered [Actual checks], with the result [Actual result]. The supporting evidence is [File and section/case ID]. [Known remaining limitation, if applicable]. The attached Issue_Closure_Record.csv records the verified scope and the confirmed closure decision.

This email records the confirmed closure; no further confirmation is requested. Please let us know if the recorded scope or decision reference is inaccurate.

Best regards,

[Sender name]

## 注意事项

“后端报告已修复/已部署”不能替代复测，UAT 通过不能扩大为生产通过。证据不足时改发[验证请求](../templates.md#13-修复验证与问题关闭)，不虚构关闭批准、时间或状态。剩余缺陷影响关闭条件时明确列出，不用模板保证无风险。期限未知改问可确认时间；附件未附按[复制规则](../external-communication.md#复制使用与事实边界)处理。
