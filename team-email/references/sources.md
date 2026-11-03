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

借鉴：按沟通目的选择格式，先确定读者与语气；项目进展可分为已完成、后续计划和问题/阻塞，保持简短并依据事实。

本地调整：3P 仅作为项目周报/简短汇报的可选形式，不强制用于对外协查和需求确认，不强制 emoji、固定周期或额外读取邮箱/聊天记录。已有上下文足够时不重复追问。

## 3. Rampstack — stakeholder-communication

- [Skill 入口](https://github.com/rampstackco/claude-skills/blob/main/skills/stakeholder-communication/SKILL.md)

借鉴：结论先行；说明信息对读者的影响；明确是通知、请求、决策还是升级；延期或坏消息说明事实、影响、处理动作和所需支持；决策给出选项及有依据的建议。

本地调整：建议、工作量、期限和风险必须有本次材料支持；没有依据时保留未知，不为每封邮件强凑选项。不按固定节奏催办，不自行增加抄送或发送邮件；该来源以内部干系人沟通为主，对外邮件只参考其内容组织原则。

## 采用边界

- 以上为写作思路来源与进一步阅读，不是对第三方 Skill 的完整安全背书，也不表示本 Skill 与其作者有官方关联。
- 本次规则和模板按本工作流重新组织、撰写，不内嵌上述第三方 Skill 的全文、脚本或工具依赖。后续若复制第三方原文或文件，应先核对对应来源的许可与署名要求。
- 中英完整对应、附件摘要与具体定位、请求/响应和日志脱敏、缺项合并询问及不编造承诺，是本 Skill 的工作流约束；并非上述各来源都提供或共同要求。
- 外部链接内容可能变化；此文档说明本次采用的具体原则。链接不可用时仍按本地 Skill 执行，维护者再核对来源。
