# Issue Follow-up：问题跟进与催办

## 适用场景与发送时机

| 项目 | 使用说明 |
| --- | --- |
| 流程/阶段 | 已有问题/资料请求的调查、处理、联调或验证阶段 |
| 触发条件 | 到达已约定反馈点、缺少最新状态，或依赖正在影响下一步；先核对最新线程，不对已回答的问题重复催办 |
| To / CC | To：当前行动负责人；CC：用户指定且与受影响依赖相关的人员。保留原线程，不因未回复自动加管理层 |
| 发送前准备 | 原请求日期/条目、最后已确认状态、已给出的输入、实际阻碍、既有时间安排及所需反馈 |
| 期望反馈/时间 | 负责人给当前状态、下一动作和可确认的完成预计；预计未知时给可提供下一次调查更新的时间，不混作修复承诺 |

## 完整英文 Sample

To: [Action owner]

Cc: [Confirmed CC recipients]

Subject: Re: [Original subject]

Dear [Action owner],

I am following up on [Issue ID / request] raised on [Original request date]. Could you please share the current status and the next steps?

The last confirmed update was [status and source date]. We have since provided [input already supplied, with reference]. We are still awaiting confirmation of [specific remaining point], which is needed for [dependent activity].

The attached Issue_Followup_Log.csv separates the confirmed updates from the items still awaiting confirmation. Please refer to FUP-01 for [specific remaining question].

Could you please provide the following by [Requested response deadline]?

1. The current investigation status and the next action owner.
2. The expected completion date, if it can be confirmed. Otherwise, please advise when the next investigation update can be provided.

Please let us know if you need any additional information from us to proceed.

Thank you for helping us confirm the next steps.

Best regards,

[Sender name]

## 附件 Sample

[下载 Issue_Followup_Log.csv](../../assets/attachments/Issue_Followup_Log.csv)。用于复核原请求和最新进展，不用“未收到更新”证明现实中未处理。

| FollowupID | OriginalRequestReference | LastConfirmedStatus | RemainingQuestion | DependencyImpact |
| --- | --- | --- | --- | --- |
| FUP-01 | [Thread/date/issue] | [Status and source] | [Specific point] | [Confirmed impact] |
| FUP-02 | [Thread/date/issue] | [Status and source] | [Specific point] | [Confirmed impact] |

CSV 另列行动负责人、请求反馈时间及下一次更新时间；后二者用途不同，未知时不互相替代。

## 写作解读与表达建议

- **开场/背景**：`following up on` 是中性追踪，说明原请求与当前需要，避免指责对方不重视。
- **现状/证据**：用 `last confirmed update` 和 `awaiting confirmation` 区分事实与未知；保留已提供材料的定位。
- **行动/结尾**：先请求可执行状态和下一步，再区分完成预计与调查更新；主动指出可补资料的协作入口。
- 推荐 `Could you please share the current status...?`；避免 `Any update???`、`We have asked many times` 或 `You must fix this immediately`，除非本次有明确且适用的约定。

## 注意事项

删去未实际提供的输入段，未给期限时询问更新时间。不能凭主题的 Urgent、未读或 REPLIED 标签判断任务完成或逾期。需要资源/决策升级时转用升级场景，而不是把催办语气简单加重。附件未附按[复制规则](../external-communication.md#复制使用与事实边界)处理。
