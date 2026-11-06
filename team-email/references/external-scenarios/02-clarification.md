# Clarification：问题澄清

## 适用场景与发送时机

| 项目 | 使用说明 |
| --- | --- |
| 流程/阶段 | 需求、设计、开发、测试标准对齐或验收准备 |
| 触发条件 | 规则、示例、接口或职责有歧义/冲突，继续实施可能造成返工；不要把待确认理解当作对方已批准 |
| To / CC | To：能解释规则或确认范围的负责人；CC：已确认会受该解释影响的实施/测试人员 |
| 发送前准备 | 来源版本和章节、现有理解、冲突证据、具体问题、影响下一步的范围 |
| 期望反馈/时间 | 逐项说明正确规则、适用条件及权威依据；必要时更新文档。请求反馈期限由本次材料提供 |

## 完整英文 Sample

To: [Rule owner]

Cc: [Confirmed CC recipients]

Subject: [Project] Clarification Required – [Rule or Scope]

Dear [Rule owner],

Could you please clarify the following points before we proceed with [dependent activity]?

Our current understanding of [document and version, section] is [current interpretation]. However, [specific example or other reference] indicates [different interpretation]. We would like to confirm the intended behavior and avoid implementing an incorrect assumption.

1. CL-01 — Under [condition], should [behavior A] or [behavior B] apply? Please confirm the applicable rule and its reference.
2. CL-02 — Does this rule apply to [scope], or only to [limited scope]? Please identify any exceptions.

The attached Clarification_Log.csv records the source references, our current understanding and the questions requiring clarification.

Could you please respond against CL-01 and CL-02 by [Requested response deadline]? If a document update is needed, please also identify the authoritative version we should use.

Thank you for helping us align on [topic].

Best regards,

[Sender name]

## 附件 Sample

[下载 Clarification_Log.csv](../../assets/attachments/Clarification_Log.csv)。保留各自来源，不把两个不一致的版本合并为同一结论。

| ClarificationID | SourceReference | CurrentUnderstanding | Question | ConfirmedAnswer |
| --- | --- | --- | --- | --- |
| CL-01 | [File/version/section] | [Interpretation] | [Which behavior applies?] | [Rule owner to complete] |
| CL-02 | [File/version/section] | [Assumed scope] | [Scope and exceptions?] | [Rule owner to complete] |

CSV 另列回答人和请求反馈时间。`ConfirmedAnswer` 未取得确认时填写 `Pending confirmation`，不能由起草者替对方补结论。

## 写作解读与表达建议

- **开场/背景**：说明澄清与下一步的关系，`Our current understanding` 主动保留不确定性。
- **现状/证据**：并列两种来源的差异，避免 `Your document is wrong` 等未经证实的归责。
- **行动/结尾**：采用编号及可直接作答的问题，明确需要规则、范围还是例外，不只问 `Is it OK?`。
- 推荐 `Could you please confirm which rule applies under [condition]?`；避免把 `discussed` 写成 `agreed`。

## 注意事项

本 Sample 中 A/B 仅适用于确有两种解释；没有备选项时直接问具体问题，不制造方案。只有本次证据支持时保留冲突描述。期限未定改问可反馈时间；附件未附按[复制规则](../external-communication.md#复制使用与事实边界)处理。澄清不等于审批，也不默认暂停全部工作。
