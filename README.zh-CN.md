# 论文打磨技能

[English (primary)](README.md) · 简体中文

四个以英文为主、附中文参考版的独立 AI 技能，帮助检查论文论证、忠实润色、核验证据和准备投稿返修材料。

**按需选一个；明确需要多项产出时再组合。** 短段润色无需跑整篇审计，也无需创建项目账本或启动完整科研流程。

中文参考见 [docs/zh-CN](docs/zh-CN)。实际安装入口使用英文。

## 四个核心技能

| 技能 | 适合解决的问题 | 示例请求 |
| --- | --- | --- |
| [paper-argument-check](paper-argument-check/SKILL.md) | 论证是否连贯，问题、方法、结果和贡献是否对齐 | “检查引言哪里没有回答研究问题，先不重写。” |
| [paper-faithful-edit](paper-faithful-edit/SKILL.md) | 保留原意的润色、翻译与压缩；按明确依据纠错 | “摘要压到250词，保留数字、术语和结论强度。” |
| [paper-evidence-check](paper-evidence-check/SKILL.md) | 数据或引文能否支持主张，书目与数字是否一致 | “核对这句引用：DOI正确是否足以支持17%的结论？” |
| [paper-submission-revision](paper-submission-revision/SKILL.md) | 根据真实材料写投稿文件、逐条审稿回复 | “根据审稿意见和修改稿起草回复，未决定的项目另列。” |

## 安装与使用

每个文件夹都是独立技能，入口为 `SKILL.md`。可直接让支持读取文件的 AI 助手按相应文件执行；在 Codex 中，也可把选中的文件夹复制到个人技能目录。

```sh
git clone https://github.com/XingjianTian/paper-polishing-skills.git
cd paper-polishing-skills
mkdir -p ~/.codex/skills
cp -R paper-faithful-edit ~/.codex/skills/
```

按客户端实际加载方式刷新或开启新聊天，然后点名调用，并提供待处理文本：

```text
使用 $paper-faithful-edit 润色下面的英文摘要。
只返回正文；保留数字、否定、术语、英式拼写和结论强度。
[粘贴摘要]
```

需要核查与润色两项产出时，明确写出两项要求，分别交付。作者已指定正确数值、只需纠正并润色时，单用 `paper-faithful-edit` 即可。完整选择示例见 [使用说明](使用说明.md)。

## 执行边界

- 忠实编辑保留原语言与主张；翻译或事实纠错需要明确请求和依据，证据疑点另列。
- 书目匹配仅确认文献身份；判断论点支持程度还需要原文、结果表格或研究设计。
- 数值不同先核对样本与统计口径，材料不足就指出缺什么，不猜正确值。
- 审稿回复只写已核实的修改；内部待办与作者未决事项单列，不虚构完成情况或承诺。
- 外部检索、全文访问和政策核对取决于运行助手可用的工具；这些文件本身不提供数据库接口。

## 来源与整理方式

本项目参考 Mohd Shahizan Othman 的 [Polishing Your Draft Article Using AI Tools](https://drshahizan.github.io/polishing-ai/) 工作坊材料，进行了任务重组并补充执行边界，提供英文主版与中文参考版。每个技能都保留具体参考页面，汇总见[来源索引](使用说明.md#来源索引)。

本项目为独立整理，非原站官方技能，非整站镜像或逐字译文。原站材料权利归其各自权利人；仓库公开不代表为第三方材料重新授权。

## 验证

中文原版经网页 Pro 审阅、定向修正与局部行为复测；英文版为对应翻译，另做格式与翻译一致性检查。验证针对给定材料下的执行表现，不构成论文质量、录用结果或客户端自动发现能力的保证。
