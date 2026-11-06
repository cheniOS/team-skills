# Issue Escalation：重要问题升级

## 适用场景与发送时机

| 项目 | 使用说明 |
| --- | --- |
| 流程/阶段 | 关键依赖受阻、影响超出当前处理团队权限或需要重大取舍的阶段 |
| 触发条件 | 存在已确认重大影响、到达既有升级条件，或需要指定决策/资源才能继续；紧急事项沿已知应急渠道及时处理，不为凑历史而等待多次催办 |
| To / CC | To：用户明确的决策人或协调负责人；CC：指定的原行动人及受影响工作流负责人。不自行扩大到高层、客户全员或无关第三方 |
| 发送前准备 | 已知事实时间线、已尝试动作及结果（如有）、实际影响、仍未知的部分、所需决定；仅有依据时给方案及取舍 |
| 期望反馈/时间 | 对具体决定、责任人、资源或处置路径作答；请求反馈时点与既有约定区分，不默认赔偿、承认违约或改排期 |

## 完整英文 Sample

To: [Decision or coordination owner]

Cc: [Confirmed CC recipients]

Subject: [Project] Escalation – [Issue ID] Affecting [Milestone or Activity]

Dear [Decision or coordination owner],

We need your support with [specific decision or coordination request] because [confirmed issue] is affecting [specific activity or milestone].

The confirmed position is as follows:

- Issue: [Observed problem and affected scope].
- Actions taken: [Actual action, date and result].
- Current impact: [Verified dependency or milestone impact].
- Still under investigation: [Unconfirmed cause, scope or timing, if relevant].

The attached Escalation_Brief.csv records the timeline, supporting references and the decision required. ESC-01 summarizes [key fact and evidence location].

Could you please confirm [specific decision] and the responsible owner by [Requested response deadline]? This will allow [dependent next step]. If this decision is outside your remit, please advise which agreed coordination route we should use.

Thank you for your support in resolving this dependency.

Best regards,

[Sender name]

## 附件 Sample

[下载 Escalation_Brief.csv](../../assets/attachments/Escalation_Brief.csv)。各行区分事实事件与决定请求，不能把调查假设写成已确认根因。

| EntryID | EntryType | DateTimeUTCOffset | FactOrDecision | EvidenceReference |
| --- | --- | --- | --- | --- |
| ESC-01 | Fact | [Known event time] | [Observed impact] | [Source reference] |
| ESC-02 | Decision request | [Requested response time] | [Specific decision] | [Supporting reference] |

CSV 另列已确认影响及对应行动/决策负责人。若要给多个方案，补充实际已评估的收益、代价及限制；没有材料时不为升级而编造选项。

## 写作解读与表达建议

- **开场/背景**：第一句把“需要什么支持”和“为什么需要”放在一起，升级目标是解除阻塞，不是加重语气。
- **现状/证据**：按问题、已尝试动作、影响和未知点组织；附件保留可追溯时间线，减少争论和重复解释。
- **行动/结尾**：`confirm [specific decision] and the responsible owner` 比 `Please escalate urgently` 更可执行。
- 说明影响用 `This is affecting [verified activity]`；原因待查用 `The cause is still being investigated`。避免未经核实的 `Your team caused the delay`。

## 注意事项

没有既往动作记录时删除该行；有重大影响可按已知流程直接升级。没有确认排期变化就不宣布延期或暂停；未知费用、根因、合同责任、补偿和上线时间均不补造。不能把未回复解释为失职或批准。附件未附按[复制规则](../external-communication.md#复制使用与事实边界)处理。
