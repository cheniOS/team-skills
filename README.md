# Team Skills

可复用的团队协作 Skill。当前包含 **team-email（团队邮件规范）**。

## team-email

适用于产品、后端开发、App 开发、测试、QA、设计、项目管理及客服等岗位。

- 根据发件角色、收件对象和邮件目的选择场景；只询问必要的缺失信息。
- 分析来信的情绪倾向、原文依据、判断把握、紧迫度和回复策略；区分最新正文与历史引用，只分析时不自动生成回复稿。
- 起草或修改时，默认生成完整英文发送稿及内容对应的中文核对稿。
- 支持只检查、固定五维评分、最小修改和结构重写；已有草稿默认最小修改，评分附扣分依据及待核对范围。
- 统一标题、行动请求、附件摘要、来源定位和签名。
- 提供接口问题反馈模板及请求、响应、日志的脱敏规则。
- 核对技术值、字段类型、调用关联和正文结论；保留冲突待确认，精简报文时明确标为相关字段摘录。
- 首段前置结论、影响及请求；方案决策列出取舍和有依据的推荐。
- 跨时区明确日期、时间及 UTC 偏移；故障跟进区分修复时间与下一次进展更新时间。
- 区分决策人、执行人、协作人和知情人，按技术同事、管理者、业务客户或外部合作方调整表达。
- 包含请求、确认、澄清、协查、评审、进度、交付、会议、跟进、短回复、引介交接、变更、验证关闭等 13 类场景。
- 项目汇报强调结果、实际影响及有依据的状态；收到、批准、部署、复测和关闭分别表述。
- 按请求分析、起草和检查邮件，不自动发送或修改邮箱。

## 下载与安装

1. [下载 team-email.zip](https://github.com/cheniOS/team-skills/raw/refs/heads/main/downloads/team-email.zip)。
2. 解压得到完整的 `team-email` 目录。
3. 将目录放入个人的 `~/.agents/skills/`，保持以下结构：

```text
~/.agents/skills/team-email/
├── SKILL.md
├── agents/openai.yaml
└── references/
```

也可从本仓库复制 [team-email](team-email) 完整目录。需要保留 `references` 和 `agents`，不要只复制 `SKILL.md`。

安装后在 Codex 中使用 `$team-email`。若未识别，重启 Codex。安装位置和调用方式参见 [Codex 官方文档](https://learn.chatgpt.com/docs/build-skills)。

## 使用示例

```text
使用 $team-email

发件角色：产品
收件对象：业务团队
邮件目的：确认通知设置需求
原始要点：……
附件：……（可选，提供文件或可访问路径）
期望对方动作：逐项确认方案，或提出修改意见
回复期限：……（如有）
```

```text
使用 $team-email，以 App 开发身份向后端反馈接口异常。
环境：UAT
问题与影响：……
请求、响应和日志：……
附件：……
请给出英文发送稿和中文核对稿，并列明需要后端协助的事项。
```

信息足够时直接生成；缺少关键需求时先提问。日志和附件应先移除凭据、无关个人信息及其他不应共享的内容，再提供给工具处理。

```text
使用 $team-email，检查并给以下原文评分，按最小修改模式修改。
保留技术值和原有问题顺序，给英文发送稿及完整中文核对稿。
邮件：……
```

只需点评时写“只检查，不改稿”；希望调整结构时写“重写/重组”。评分采用目的与行动、结构与定位、事实与证据、语言与一致性、隐私与共享五维，各 20 分。不适用或无法核实项标 N/A，按适用满分折算，并列出扣分依据。高分不替代发送前的关键问题处理；详见审查指南。

```text
使用 $team-email，分析以下来信的情绪倾向，列出原文依据、判断把握（高/中/低）、紧迫度和回复建议。区分最新正文与历史引用，只分析，不生成回复稿。
邮件：……
```

有已授权且身份匹配的邮件工具时，也可以明确要求“读取我收件箱最近 5 封邮件并按上述字段分析”。本 Skill 不提供邮箱连接或 OAuth 配置，没有工具时需提供正文。语气分析不证明真实心理；紧迫度单独判断，不把催促直接当作不满。

## 内容边界

仓库内示例使用占位符或明确虚构内容，不包含真实邮件来源、联系信息、公司内部链接、实际项目版本或原始业务附件。规范不代表任何公司的官方制度；实际使用须遵从所在团队的流程。

脱敏规则属于操作指导，不保证输入或输出已经自动完成脱敏。发送前仍需核对事实、收件人、附件、敏感信息与中英文一致性。

## 目录

- [Skill 入口](team-email/SKILL.md)
- [场景模板与附件摘要](team-email/references/templates.md)
- [审查、评分与最小修改](team-email/references/review-and-scoring.md)
- [来信情绪、紧迫度与回复策略分析](team-email/references/incoming-analysis.md)
- [虚构行为评估用例](team-email/evals/cases.json)
- [收件角色与事项选择](team-email/references/audiences-and-scenarios.md)
- [接口问题与日志脱敏](team-email/references/backend-api-issue.md)
- [通用示例与适用边界](team-email/references/observations.md)
- [参考来源与采用范围](team-email/references/sources.md)
- [安装包](downloads/team-email.zip)

更新 Skill 后，应同步更新 `downloads/team-email.zip`，保持源文件与下载包一致。

## 参考来源

本 Skill 参考以下公开沟通框架，并按本工作流重新撰写规则和模板：

- [Softaworks professional-communication](https://github.com/softaworks/agent-toolkit/tree/main/skills/professional-communication)：开发者邮件、读者适配、决策请求与异步沟通。
- [Anthropic internal-comms](https://github.com/anthropics/skills/tree/main/skills/internal-comms)：按沟通目的选格式，采用可选的 Progress / Plans / Problems 进展结构。
- [Rampstack stakeholder-communication](https://github.com/rampstackco/claude-skills/tree/main/skills/stakeholder-communication)：结论先行、业务影响、延期说明与明确决策请求。

详细采用范围及调整见 [参考来源](team-email/references/sources.md)。这些是阅读参考，不是运行依赖；无需额外安装第三方 Skill。

## English

Reusable team collaboration skills. **team-email** analyzes incoming email tone, quoted evidence, confidence, urgency, and reply strategy. It also drafts professional emails with matching English and Chinese versions, role-aware templates, attachment summaries, and API/log redaction guidance, and supports evidence-based scoring, minimal editing, and technical evidence checks. Analysis-only requests do not produce reply drafts. Extract the ZIP into `~/.agents/skills/`, then invoke `$team-email` in Codex. Mailbox access requires a separately available authorized tool; the skill does not send email or modify the mailbox automatically.
