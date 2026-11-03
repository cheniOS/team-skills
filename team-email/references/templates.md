# 全岗位邮件模板

按场景选择并裁剪。`[Project]` 只在帮助识别时保留；方括号为待填字段。模板不构成真实附件、期限、完成状态或批准。`[Signature]` 替换为发件人已核实的姓名、岗位及联系方式。

以下为英文母版。实际起草默认先输出完整英文发送稿，再输出段落与行动项对应的完整中文核对稿；具体规则见 [Skill 默认输出](../SKILL.md#默认输出与检查)。不要把两种语言逐句交错，也不重复翻译日志、字段名或文件名。

## 附件正文模块

适用各岗位和下列场景。报告、需求、评审材料等有附件时，将此模块放在背景之后、动作请求之前；正文已有关键点时只补来源定位，避免重复。所有内容和位置须从实际附件核对，保留适用条件。

Please refer to [file name, version/date] for the full details. The key points are summarized below:

1. [Finding or decision needed]: [Key fact, figure with unit, or short excerpt]. Reference: [file name, section/page or sheet/range].
2. [Finding or decision needed]: [Key fact, figure with unit, or short excerpt]. Reference: [file name, section/page or sheet/range].

Could you please [specific action] regarding [item numbers or scope]?

按材料替换内容，而非全部填写：

- 产品：`[Rule or change] — [Constraint or acceptance criterion]; [document section/page].`
- 后端：`[Endpoint/version/environment] — [Expected vs. actual result or key contract change]; [log timestamp/request ID or document section].`
- App：`[Platform/build] — [Changed behavior or issue]; [screenshot number, log location or release-note section].`
- 测试：`[Executed/passed/failed/blocked figures and scope] — [Critical case/defect]; [report sheet/range and case/defect ID].`
- QA：`[Quality criterion] — [Evidence, unmet condition or residual risk]; [report section/page]; Decision required: [specific decision].`

小段表格可使用 `Item | Key Finding | Reference | Action Required` 四列；内容较宽时改编号。安装包或压缩包用 `Contents`、`Version`、`Usage` 等已知信息代替报告摘要。不自行计算缺少分母的通过率，不把某轮测试结果扩大为整体质量或发布批准。

## 1. 请求资料、资源或协助

Subject: [Project] Request for [Specific Information or Resource]

Dear [Name],

We are working on [task] and need [information or resource] to proceed with [next step].

Could you please provide the following?
1. [Required item and expected format]
2. [Required item and expected format]

[If applicable: Please refer to the attached [file name] and complete [specific fields].]

Could you please share the expected availability date?

Thank you for your support.

Best regards,
[Signature]

已知期限时，将预计时间请求替换为 `Could you please provide these by [date, time and time zone] so that we can [reason]?`。

## 2. 确认、审批或方案选择

Subject: [Project] Confirmation Required – [Specific Topic]

Dear [Name],

Before we proceed with [next step], could you please review and confirm the following items?

1. [Item title]
   [Proposed approach and relevant constraint]
   Please confirm [specific decision or option].
2. [Item title]
   [Proposed approach and relevant constraint]
   Please confirm [specific decision or option].

Your confirmation will allow us to [dependent action]. Please let us know if any changes are required.

Thank you for your support.

Best regards,
[Signature]

正式审批可改 `Approval Required` / `approve`，明确被审批的版本和范围；不把普通确认包装成批准。

## 3. 澄清需求、规则或分工

Subject: [Project] Clarification Required – [Specific Topic]

Dear [Name],

We would like to clarify [question] before proceeding with [task].

Our current understanding is [understanding based on supplied information]. However, [specific ambiguity or conflicting information].

Could you please confirm:
1. [Specific question]
2. [Specific question]

[If applicable: The relevant reference is [document or link and section].]

Thank you for your support.

Best regards,
[Signature]

## 4. 问题上报与协查

Subject: [Project] Issue – [Specific Symptom or Impact]

Dear [Name or Team],

We observed [specific issue] while [activity]. This is affecting [confirmed scope or impact].

- Context: [Relevant process, document, system, version or environment]
- Expected result: [Expected outcome]
- Actual result: [Observed outcome]
- Evidence: [Attachment, screenshot, example or reference]

Could you please investigate [specific question] and advise on the next steps and expected resolution time?

Thank you for your support.

Best regards,
[Signature]

只留适用字段。技术问题可加时间、复现步骤、关键请求/响应、工单；业务问题用单据、流程阶段、案例编号。环境影响判断时在标题加标签。现象不能证明根因时不指责责任方。

## 5. 设计、文档或交付物评审

Subject: [Project] Review Request – [Deliverable and Version]

Dear [Name or Team],

Please review [deliverable] for [purpose]. [The attached file / The link below] contains [scope].

Key points for review:
1. [Review point or general principle]
2. [Review point, with page/screen/section reference]

Could you please share your feedback on [specific decision or review scope]?

Thank you for your support.

Best regards,
[Signature]

## 6. 进度更新、延期或客服状态

Subject: [Project] Update on [Milestone, Task or Case Group]

Dear [Name or Team],

Here is the current status of [scope] as of [date].

- Completed: [Verified completed work]
- In progress: [Current work and owner, if known]
- Pending: [Dependency or decision required]
- Next step: [Next action and confirmed target, if available]

[If delayed: [Item] is delayed due to [confirmed reason]. The impact is [impact]. We are taking [action].]

[If action is needed: Could you please [specific action]?]

Thank you for your support.

Best regards,
[Signature]

未知完成日期标待确认，不承诺 tomorrow、SLA、退款、赔偿或上线时间。纯通知无对方动作时删请求段。

## 7. 交付、发布或完成通知

Subject: [Project] Delivery – [Deliverable and Version]

Dear [Name or Team],

[Deliverable] is ready for [review, testing or use].

- Scope: [Included items]
- Location: [Attachment or link]
- Validation: [Checks performed and actual result, if supplied]
- Open items: [Known limitations, if any]

Could you please [review, verify receipt or perform the next action]?

Thank you for your support.

Best regards,
[Signature]

已验证完成才用 `Completion – [Milestone]`，有发布证据才说 released/deployed。可加简短团队致谢；避免标题重复堆叠信息。

## 8. 会议安排与纪要

安排标题：`[Project] Meeting Request – [Topic] – [Date]`。正文给目的、时间和时区、参与人、议程、已提供的会议链接，再请对方确认；链接未知留占位符，不生成口令。

纪要模板：

Subject: [Project] Meeting Summary – [Topic] – [Date]

Dear [Name or Team],

Please find below the summary of our meeting on [date].

Decisions:
1. [Confirmed decision and scope]

Action items:
1. [Action] — Owner: [Name]; Due: [Confirmed date and time zone / To be confirmed]
2. [Action] — Owner: [Name]; Due: [Confirmed date and time zone / To be confirmed]

Open points:
- [Unresolved question and who needs to respond]

Please let us know if any corrections are needed.

Best regards,
[Signature]

## 9. 跟进、催办与升级

同一事项优先回复原线程。确需新线程时：

Subject: [Project] Follow-up – [Original Request or Topic]

Dear [Name],

I am following up on [request] shared on [date]. We are currently waiting for [specific input] to proceed with [next step].

Could you please share the current status and expected completion date?

[If relevant: This is affecting [confirmed milestone or impact]. Please let us know if support from another team is required.]

Thank you for your support.

Best regards,
[Signature]

升级时增加事实时间线、实际影响和所需决策，不把未回复当失职，不擅自扩大收件范围。

## 10. 简短回复与拉人协作

保留原 Subject，以下每次只选一种。

收到但尚未评审：

Dear [Name],

Thank you. We have received [material] and will review [scope].

Best regards,
[Signature]

明确确认：

Dear [Name],

We confirm [exact item, version or scope]. [Confirmed next action, if any.]

Best regards,
[Signature]

新增协作人：

Dear [Name],

Adding [person or team] to help with [specific reason]. [Person or team], could you please [specific action]?

Best regards,
[Signature]

只有用户给出确认结论或明确授权表达该结论时才用确认模板；不能把“收到”写成确认或批准。

## 调用示例

- “用 $team-email，请客户确认两处设计调整，具体期限未定。”
- “用 $team-email，催合作方提供验收报告，不承诺上线日期，回复原线程。”
- “用 $team-email，将客服处理进展整理为英文邮件，保留提供的 SLA。”
- “用 $team-email，检查采购资料请求的标题、行动项和签名，只提格式建议。”

调用仅生成或检查文本，不发送邮件。
