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

Could you please provide [information or resource] so that we can proceed with [next step]?

We are currently working on [task]. [Brief context needed to understand the request.]

Required items:
1. [Required item and expected format]
2. [Required item and expected format]

[If applicable: Please refer to the attached [file name] and complete [specific fields].]

Could you please share the expected availability date?

Thank you for your support.

Best regards,
[Signature]

已知期限时，将预计时间请求替换为 `Could you please provide these by [date, time and time zone] so that we can [reason]?`。

求助时可补 `We have tried [approach], which resulted in [observed outcome].` 和 `If another team owns this area, could you please advise whom we should contact?`，前提是确有尝试记录或责任范围不明确；不要编造尝试、联系名单或预估耗时。

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

需要在方案间选择时，将编号确认点替换为以下决策模块；单项确认不必使用。收益、代价和建议必须来自已知需求与证据，未知项标待评估。

Decision required: [Specific decision and scope]

- Option A — [Approach]; Benefits: [Known benefit]; Trade-offs: [Known cost or constraint].
- Option B — [Approach]; Benefits: [Known benefit]; Trade-offs: [Known cost or constraint].

Recommendation: [Proposed option and evidence-based reason / Further assessment is needed before recommending an option].

Could you please confirm [option or decision] [by the confirmed date, time and UTC offset, if provided]? This decision is needed to [dependent next step].

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

Could you please investigate [specific issue]? We observed it while [activity], and it is affecting [confirmed scope or impact].

- Context: [Relevant process, document, system, version or environment]
- Expected result: [Expected outcome]
- Actual result: [Observed outcome]
- Evidence: [Attachment, screenshot, example or reference]

Please check [specific question] and share your findings and proposed next steps. If the resolution time is not yet known, please advise when the next investigation update can be provided.

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

[One-sentence status summary of [scope], its confirmed impact and any action needed, as of [date].]

- Status: [On track / At risk / Off track, only when supported; otherwise omit or state that assessment is pending]
- Completed: [Verified completed work]
- In progress: [Current work and owner, if known]
- Pending: [Dependency or decision required]
- Next step: [Next action and confirmed target, if available]
- Next update: [Confirmed update date, time and UTC offset, if provided]

[If delayed: [Item] is delayed due to [confirmed reason]. The impact is [impact]. We are taking [action].]

[If action is needed: Could you please [specific action]?]

Thank you for your support.

Best regards,
[Signature]

未知完成日期标待确认，不承诺 tomorrow、SLA、退款、赔偿或上线时间。纯通知无对方动作时删请求段。

周报或简短项目汇报可改为 `Progress / Plans / Problems` 三部分，每部分只保留少量相关事实；涉及阻塞时点明影响和所需协助。需要对方处理时保留独立行动项，纯告知写 `No action is required at this stage.`，前提是本次确为无需动作。不要将所有对外邮件都改成周报格式。

延期或故障跟进时，区分已完成、进行中、待确认；已知原因与待查假设分开。只有用户提供了下一次更新时间才填写该项，否则请求对方提供更新安排；不把“将更新进展”写成“届时已修复”。

面向管理层时保留主要成果、目标/实际差异、关键风险和所需决定，细节链接到报告；面向执行团队时增加行动负责人及证据。数据不足时不填写进度百分比、成本或趋势判断。

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

发布告知可加“变化是什么、影响谁、收件人是否需操作、去哪里查说明/反馈”，只填写已知信息。回滚方案、支持人、使用培训和发布时间均不得自行补造；纯告知且无需响应时可明确说明。

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

Could you please share the current status of [request] raised on [date]? We are waiting for [specific input] to proceed with [next step].

Please advise on the expected completion date or, if it is still being assessed, when the next update can be provided.

[If relevant: This is affecting [confirmed milestone or impact]. Please let us know if support from another team is required.]

Thank you for your support.

Best regards,
[Signature]

升级时增加事实时间线、实际影响和所需决策，不把未回复当失职，不擅自扩大收件范围。

跨时区期限统一写为 `[DD Mon YYYY, HH:mm, UTC±HH:mm]` 等无歧义形式，未知时留待确认或省略；不在模板中默认承诺 24/48 小时响应。

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

## 11. 协作引介与职责交接

简短引介可用 `Subject: [Project] Introduction – [Person or Team]`，说明介绍谁、与本事项相关的职责以及希望双方如何协作；职责尚未确认时表明为拟议安排，不默认要求所有人回复。

交接模板：

Subject: [Project] Handover – [Workstream]

Dear [Name or Team],

Could you please review the handover of [scope] and confirm [receipt / acceptance of the proposed responsibilities, as applicable]?

- Current status: [Verified status and completed work]
- Open items: [Unfinished tasks, blockers and known dependencies]
- Responsibilities: [Confirmed or proposed outgoing/incoming owners, clearly distinguished]
- Materials: [Document, ticket or artifact references]
- Effective date or condition: [Confirmed date/condition / Pending confirmation]

Please let us know which items need clarification and whether the proposed handover can be accepted. [Include only if acceptance is still pending.]

Best regards,
[Signature]

接收文件与接受职责分开表述；待接受的交接不写成已完成。若涉及权限，只说明通过已有受控流程提供所需访问，不在邮件放凭据、不自动授权或移交账号。

## 12. 需求、范围或排期变更

Subject: [Project] Change Request – [Scope or Milestone]

Dear [Decision Maker],

Could you please review the proposed change to [scope or milestone]? [Brief confirmed impact or reason.]

- Baseline: [Previously confirmed scope, version or date, with reference]
- Proposed change: [Specific before/after difference]
- Reason: [Known reason]
- Impact: [Confirmed effects on users, dependencies, effort or schedule; identify estimates and unknowns]
- Recommendation: [Evidence-based recommendation, if available]

Please confirm [specific decision]. Until this is confirmed, [state only the current arrangement explicitly provided by the user].

Best regards,
[Signature]

若本次是已批准变更的通知，将标题改为 `Change Notice`，正文注明已核实的决定与生效范围，并写受影响人员需要执行的动作；不能将提议写成批准。原基线未知且影响决策时询问，非关键未知字段可省略或在邮件外标待补。未给出预算或审批前执行安排时，不为这些缺项新增正文栏；删除 `Until this is confirmed` 句，不默认声称暂停工作或继续原计划。

## 13. 修复验证与问题关闭

Subject: [Project][Environment] Verification Required – [Issue or Ticket]

Dear [Verifier or Team],

[Reported or verified fix/deployment status, attributed to its source]. Could you please verify [specific behavior and scope]?

- Reference: [Issue/ticket and affected version/environment]
- Validation requested: [Checks and expected results supported by the original issue or agreed criteria]
- Evidence available: [Fix/deployment reference or existing test evidence]
- Current verification status: [Not yet tested / In progress / Actual verified result]
- Remaining items: [Known open points, if any]

Please share the verification result and supporting evidence. [Include a confirmed date/time/UTC offset only if supplied.]

Best regards,
[Signature]

仅当有对应验证结果且关闭结论得到本次材料支持时，才改为 `Closure Confirmation – [Issue]`，说明验证的版本、环境、范围、证据和仍适用的限制。后端报告“已修复/已部署”不等于 QA 复测通过，UAT 验证不等于生产验证；材料不足时起草验证请求或标明关闭待确认，不能自行宣布关闭。

## 调用示例

- “用 $team-email，请客户确认两处设计调整，具体期限未定。”
- “用 $team-email，催合作方提供验收报告，不承诺上线日期，回复原线程。”
- “用 $team-email，将客服处理进展整理为英文邮件，保留提供的 SLA。”
- “用 $team-email，检查采购资料请求的标题、行动项和签名，只提格式建议。”

调用仅生成或检查文本，不发送邮件。
