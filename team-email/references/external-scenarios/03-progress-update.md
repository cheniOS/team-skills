# Progress Update：工作进展汇报

## 适用场景与发送时机

| 项目 | 使用说明 |
| --- | --- |
| 流程/阶段 | 项目执行、开发、测试、交付准备或服务处理 |
| 触发条件 | 到已约定汇报节点、完成关键里程碑、状态发生实质变化，或依赖/风险影响后续安排 |
| To / CC | To：约定接收状态的项目/业务负责人；CC：用户指定的相关工作流负责人或知情人员 |
| 发送前准备 | 截至时间、范围、已核实成果、正在进行项、未决依赖、证据位置；已确认时才列下次更新时间 |
| 期望反馈/时间 | 纯通知无需确认；发现错误可更正。确有决策或协助请求时另列负责人和请求反馈时点，不硬要所有人回复 |

## 完整英文 Sample

To: [Project contact]

Cc: [Confirmed CC recipients]

Subject: [Project] Progress Update – [Workstream] – [Reporting date]

Dear [Project contact],

As of [Status as-of date/time/UTC offset], [one-sentence factual summary of the workstream and its impact on the next milestone].

The current position is:

- Completed: [Verified deliverable or outcome], supported by [evidence reference].
- In progress: [Current activity and known owner].
- Pending: [Input or decision still required and its confirmed impact].
- Next step: [Planned action; include a target only if it has been confirmed].

The attached Progress_Summary.csv provides the item-level status and evidence references. In particular, [key finding and row/item reference] is relevant to [next milestone or dependency].

This email is for information; no action is required from you at this stage. Please let us know if any of the reported information needs correction.

Our next update is scheduled for [Confirmed next update].

Thank you for your continued cooperation.

Best regards,

[Sender name]

## 附件 Sample

[下载 Progress_Summary.csv](../../assets/attachments/Progress_Summary.csv)。正文引用结果和条目，不把表中占位状态当作真实进展。

| ItemID | WorkItem | Status | VerifiedOutcome | EvidenceReference |
| --- | --- | --- | --- | --- |
| UPD-01 | [Deliverable] | [Verified status] | [Actual outcome] | [File/section or case ID] |
| UPD-02 | [Dependency] | [Actual status] | [Known impact] | [Source reference] |

CSV 另列实际/已确认责任人、下一步及已确认目标。没有分母或完整数据时不生成完成百分比。

## 写作解读与表达建议

- **开场/背景**：`As of` 确定状态截点，首句交代结果及影响，让收件人先知道重点。
- **现状/证据**：完成、进行中、依赖分开；`supported by` 要有可定位记录，而非把开展活动当成果。
- **行动/结尾**：本 Sample 是纯通知，明确无需动作；有真实请求时替换通知段，写明谁需要反馈什么。
- 推荐 `Validation is pending`、`The completion date is still being assessed`（确属未知时）；避免 `Everything is on track` 或无依据的 `90% complete`。

## 注意事项

没有已确认下次更新时间就删除该句，不为了模板完整编造更新承诺。不存在 Pending 项可删除，不强凑风险；确实需要对方处理时不能同时写 `no action is required`。附件未附按[复制规则](../external-communication.md#复制使用与事实边界)处理。延期原因、费用、恢复时间和发布承诺均须来自本次材料。
