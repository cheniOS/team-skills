# 参考来源与采用范围

本 Skill 参考下列公开材料中的通用沟通框架，再结合中英核对、附件定位和接口日志脱敏需求整理为独立规则与模板。此文档供追溯与维护，不要求日常起草访问外部网站，不自动安装或执行这些第三方 Skill。

## 1. Softaworks — professional-communication

- [Skill 入口](https://github.com/softaworks/agent-toolkit/blob/main/skills/professional-communication/SKILL.md)
- [开发者邮件模板](https://github.com/softaworks/agent-toolkit/blob/main/skills/professional-communication/references/email-templates.md)
- [远程与异步沟通](https://github.com/softaworks/agent-toolkit/blob/main/skills/professional-communication/references/remote-async-communication.md)

借鉴：先说明事项、原因和下一步；按技术同事、管理者与业务读者调整细节；请求写清所需产出；决策展示选项和取舍；提供足够上下文以便异步作答。

本地调整：首段前置核心请求与影响；日期、时间及当日 UTC 偏移明确；不采用固定邮件响应时长、模糊 EOD 或默认录制会议等约定。所有外部动作仍以用户本次授权为准。

## 2. Anthropic — internal-comms

- [Skill 入口](https://github.com/anthropics/skills/blob/main/skills/internal-comms/SKILL.md)
- [Progress / Plans / Problems 更新框架](https://github.com/anthropics/skills/blob/main/skills/internal-comms/examples/3p-updates.md)
- [一般内部沟通](https://github.com/anthropics/skills/blob/main/skills/internal-comms/examples/general-comms.md)
- [逐项问答原则](https://github.com/anthropics/skills/blob/main/skills/internal-comms/examples/faq-answers.md)

借鉴：按沟通目的选择格式，先确定读者与语气；项目进展可分为已完成、后续计划和问题/阻塞，保持简短并依据事实。

本地调整：3P 仅作为项目周报/简短汇报的可选形式，不强制用于对外协查和需求确认，不强制 emoji、固定周期或额外读取邮箱/聊天记录。已有上下文足够时不重复追问。

进一步采用：多个问题按原编号逐项回应，已知答案给依据，未知答案保留待确认。不采用其全公司问题搜集范围；公司通讯的长篇汇总和主动跨系统收集，不作为一般项目邮件的默认流程。

## 3. Rampstack — stakeholder-communication

- [Skill 入口](https://github.com/rampstackco/claude-skills/blob/main/skills/stakeholder-communication/SKILL.md)
- [干系人更新模板与说明](https://github.com/rampstackco/claude-skills/blob/main/skills/stakeholder-communication/references/update-templates.md)

借鉴：结论先行；说明信息对读者的影响；明确是通知、请求、决策还是升级；延期或坏消息说明事实、影响、处理动作和所需支持；决策给出选项及有依据的建议。

本地调整：建议、工作量、期限和风险必须有本次材料支持；没有依据时保留未知，不为每封邮件强凑选项。不按固定节奏催办，不自行增加抄送或发送邮件；该来源以内部干系人沟通为主，对外邮件只参考其内容组织原则。

进一步采用：区分执行人、决策人与知情人；依据事实标明项目状态；以成果和影响代替活动堆积；求助说明已尝试动作及结果；已约定节奏下明确进展检查点。没有数据不编造指标、状态或费用，不采用按连续几次同色自动改变状态的规则，也不默认承诺按周发送。

## 本次补齐的方向

| 方向 | 来源中的启发 | 本地落点 |
| --- | --- | --- |
| 收件人角色与决策职责 | Softaworks 的读者适配；Rampstack 的关切、细节需求和决策权 | `audiences-and-scenarios.md` 的职责划分与六类读者 |
| 更完整的求助与升级 | 两套技术/干系人模板中的已尝试动作、结果和具体支持请求 | 请求/协查/跟进模板，避免空泛“请帮忙” |
| 项目状态与结果导向 | Rampstack 的周报、风险、延期、管理层更新模板 | 有依据的状态、目标/实际差异、负责人和所需决定 |
| 逐项回应和决策留痕 | Anthropic 的问答；Rampstack 的明确决定及后续跟进 | 保留问题编号、已决定/未决定范围与证据 |
| 引介、交接、变更、验证/关闭 | Softaworks 的介绍、会议行动项、计划变化沟通；通用项目协作需求 | 在本 Skill 中原创补齐模板 11–13，不声称上游提供相同完整流程 |

保留现有中英双稿、脱敏与附件定位规则；没有照搬录制会议、全公司信息搜集、自动发送、固定时长或隐含审批等做法。

## 采用边界

- 以上为写作思路来源与进一步阅读，不是对第三方 Skill 的完整安全背书，也不表示本 Skill 与其作者有官方关联。
- 本次规则和模板按本工作流重新组织、撰写，不内嵌上述第三方 Skill 的全文、脚本或工具依赖。后续若复制第三方原文或文件，应先核对对应来源的许可与署名要求。
- 中英完整对应、附件摘要与具体定位、请求/响应和日志脱敏、缺项合并询问及不编造承诺，是本 Skill 的工作流约束；并非上述各来源都提供或共同要求。
- 外部链接内容可能变化；此文档说明本次采用的具体原则。链接不可用时仍按本地 Skill 执行，维护者再核对来源。
