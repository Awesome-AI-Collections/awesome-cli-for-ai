---
title: "KBB"
entity_type: "tool"
category: "MCP / Tooling"
last_reviewed_at: "2026-04-14"
---

# KBB

## 一句话总结

一个面向 Claude Code 的知识库文章生成 CLI / MCP，把研究、文件采集、格式转换、画图和发布压成一条命令式流水线。

## 快速判断

- 如果你想在 Claude Code 里一句命令把“搜资料 -> 整理 -> 出图 -> 发文章”跑完，它值得优先看
- 如果你只想找通用知识管理 SaaS，而不是 terminal-first 的 agent 工作流，先看别的方案
- 它更像知识文章生产流水线的 MCP 工具面，不是普通笔记软件

## 你会怎么用它

- 接进 AI 开发流：给 Claude Code 一套 research、ingest、diagram、publish 的命令面，让 agent 能直接产出知识文章
- 接进日常工作流：在终端里把专题研究、资料整理、图文输出和公开分享串起来
- 最小落地方式：先用一个熟悉主题跑一次研究模式，看看输出文章和图表质量是否足够

## 它解决什么问题

- 知识整理经常卡在搜集资料、转格式、画图和发布之间来回切换
- Claude Code 虽然能写，但缺少一条稳定的研究到成文流水线
- 多格式资料很难在不折腾脚本的情况下快速汇总成可分享文章

## 适合谁

- 想在 Claude Code 里用命令完成研究到成文发布的人
- 需要把多格式资料整理成知识文章的个人与团队
- 想把检索、转换、制图和发布串成 terminal workflow 的用户

## 核心能力

- 研究模式：Claude 自身知识加网络搜索补充，快速生成研究底稿
- 多格式 ingest：能把 PDF、DOCX、PPTX、XLSX 等资料统一转成 Markdown
- 图表生成：可调用 Draw.io 产出流程图、对比图等插图
- 发布链路：支持把最终文章发到 FlowMind，并生成分享链接
- 命令入口清晰：既有 slash command，也有对应 MCP 工具集合

## 能力边界

- 明显可用：专题研究、知识文章、图文整理、agent 辅助写作流水线
- 效果一般：只想做轻量笔记记录或只想要一个 Markdown 转换器的场景
- 不要误用：它不是通用知识库平台本体，也不是每个环节都做到最强的专精工具

## 集成方式

- 作为单独工具：直接在 Claude Code 里用 `/kbb` 跑单次研究或单文件整理
- 作为 AI 工作流组件：放在 research、ingest、diagram、publish 串联层
- 作为团队流程节点：适合把“信息整理成可读文章”这一步做成可复用命令流

## 上手建议

- 第一步先用研究模式处理一个你本来就熟悉的主题，方便判断内容质量
- 最值得先试的是“你已经有资料、但一直懒得整理成结构化文章”的场景
- 如果你对发布链路还没准备好，先用 `--no-pub` 轻量验证，不要立刻把外部分享接进流程

## 选型建议

- 如果你的主需求是让 Claude Code 直接产出带图的知识文章，适合看它
- 如果你的主需求只是文件转 Markdown，MarkItDown 一类工具更轻
- 如果你的主需求是完整知识管理平台，而不是 agent-friendly command surface，FlowMind 本体或别的笔记系统更合适

## 为什么值得关注

- 它把研究、采集、转换、可视化和发布做成了一个清晰的命令面
- 这类为 Claude Code 设计的“内容生产流水线型 MCP”还不算多
- 对需要频繁整理专题内容的人来说，它比手工在多个工具间切换更有复用价值

## 类似项目

- [FlowMind for Claude](flowmind-for-claude.md) - 更偏把任务、笔记和目标管理接进 Claude；KBB 更偏把资料整理成知识文章。
- [MarkItDown](../../awesome-ai-for-coding/items/markitdown.md) - 更偏统一文件转换层；KBB 会把转换能力接进更完整的研究与发布流水线。

## 官方链接

- **GitHub:** https://github.com/haohappy/kbb
- **更新记录:** https://github.com/haohappy/kbb/releases

## 标签

- `Claude Code`, `MCP`, `Knowledge Base`, `Research`, `Publishing`

## 参考依据

- 这条说明主要依据项目 README、命令示例、工具列表和 releases 页面整理而成
- 关于“归入 CLI 而非内容平台”的判断，来自它的主使用面明确是 Claude Code 的 slash command 与 MCP 工具面

## 更新观察点

- 后续优先观察研究质量、图表能力和发布链路是否继续增强
- 关注它对更多资料来源、更多图表模板和更细粒度发布控制的支持
- 继续跟踪它与 FlowMind、Draw.io、MarkItDown 的耦合是否变得更稳
