---
title: "n8n-MCP"
entity_type: "tool"
category: "MCP / Tooling"
last_reviewed_at: "2026-05-05"
---

# n8n-MCP

## 一句话总结

一个把 n8n 节点文档、模板、校验和工作流操作暴露给 Claude、Codex、Cursor、Windsurf 等客户端的 MCP server 和 agent 工具层。

## 快速判断

- 如果你想让 Claude Code、Codex 或 Cursor 更懂 n8n 的节点、模板和工作流校验，它值得优先看
- 如果你要的是完整自动化平台本体，而不是给 agent 接一层 n8n 能力，先看别的方案
- 它更像 n8n 的 agent command surface 和 MCP 工具层，不是自动化平台本体替代品

## 你会怎么用它

- 接进 AI 开发流：把它接到 Claude Code、Codex、Cursor、Windsurf 等客户端，让 agent 在对话里搜索 n8n 节点、模板并校验工作流
- 接进日常工作流：让团队在设计、修改和部署 n8n 流程时，先通过 MCP 工具获取模板、节点配置和校验反馈
- 最小落地方式：先连上它的托管 dashboard 或自托管实例，试一次模板搜索、节点查询和 workflow validation 的闭环

## 它解决什么问题

- 让 AI 帮你搭 n8n 流程时，模型往往不够了解节点参数、默认值、模板和真实可用配置
- 即使 agent 会写 JSON，也经常在节点字段、表达式和连接结构上踩坑
- 团队想把 n8n 设计与更新接进 MCP 客户端，但不想自己维护一整层节点知识、校验和模板索引

## 适合谁

- 想让 Claude Code、Codex、Cursor、Windsurf 等工具更懂 n8n 的开发者
- 需要让 agent 搜索 n8n 节点、模板并校验工作流配置的自动化团队
- 希望把 n8n 工作流设计和更新接进 MCP 客户端的人

## 核心能力

- 节点知识层：覆盖大量 n8n core / community nodes、属性 schema、操作说明和官方文档映射
- 模板搜索：不仅能搜节点，还能查模板库、真实配置示例和按任务筛选的候选流程
- 校验链路：README 明确强调多级 validate 流程，降低“看起来像对的 JSON 其实跑不起来”的概率
- IDE / agent 接入：提供 Claude Code、Cursor、Windsurf、Codex 等客户端的 setup 路径
- 部署与操作：同时支持 npm、npx、Docker、Railway 和托管 dashboard 入口

## 能力边界

- 明显可用：让 agent 更准确地设计、修改、校验和部署 n8n 工作流
- 效果一般：只想做最轻量的单次节点查询，或者根本不使用 n8n 的场景
- 不要误用：它不是 Zapier / n8n / Activepieces 这类自动化平台本体；它首先是给 agent 使用的 n8n 工具面

## 集成方式

- 作为单独工具：直接把 MCP server 连接到目标客户端，按自然语言调用它的节点、模板和校验能力
- 作为 AI 工作流组件：放在 agent 的外部工具接入层，让模型能理解并操作 n8n 生态
- 作为团队流程节点：适合放在 workflow design、review、preflight validation 和 deployment 前检查环节

## 上手建议

- 第一步先跑模板搜索和节点查询，不要一上来就让 agent 直接改生产工作流
- 最值得先试的是“模板搜索 -> 节点配置 -> validate_node / validate_workflow”这一条最短闭环
- 如果你已经有 n8n 实例，先在开发环境或副本里试，不要直接让 AI 改生产流

## 选型建议

- 如果你的主需求是让 agent 深度理解并操作 n8n，适合看它
- 如果你的主需求是完整自动化平台本体，而不是 agent 工具层，先看 [Activepieces](../../awesome-ai-for-everything-in-life/items/activepieces.md) 或 n8n 本身
- 如果你的主需求是把某个外部系统接进 Claude 的自然语言工作流，而不是围绕 n8n，像 [FlowMind for Claude](flowmind-for-claude.md) 这种更贴近

## 典型使用场景

- 用 Claude Code 或 Codex 辅助搭建新的 n8n 工作流
- 在 workflow review 前做模板检索、节点参数核查和结构校验
- 让团队里的 agent 共享同一套 n8n 节点知识和 validation 入口

## 为什么值得关注

- 它不是只给几个文档链接，而是在做 n8n 的知识层、模板层和校验层
- README 和 changelog 都很强调验证、模板、默认值风险和多客户端接入，这比普通“某平台 MCP server”更工程化
- 最近 changelog 和 releases 更新频率很高，说明它还在快速迭代节点覆盖、模板元数据和安全修正

## 类似项目

- [FlowMind for Claude](flowmind-for-claude.md) - 更偏把外部 productivity 系统接进 Claude；n8n-MCP 更偏让 agent 理解并操作 n8n 自动化平台。
- [Firecrawl CLI](firecrawl-cli.md) - 更偏网页抓取与搜索能力的 CLI / MCP 接入；n8n-MCP 更偏 workflow automation 平台知识与校验层。
- [Activepieces](../../awesome-ai-for-everything-in-life/items/activepieces.md) - Activepieces 是自动化平台本体；n8n-MCP 是给 agent 使用的 n8n 工具面。

## 官方链接

- **官网:** https://dashboard.n8n-mcp.com
- **GitHub:** https://github.com/czlonkowski/n8n-mcp
- **更新记录:** https://github.com/czlonkowski/n8n-mcp/releases

## 标签

- `n8n`, `MCP`, `Workflow Automation`, `Claude Code`, `Codex`, `Cursor`

## 参考依据

- 这条说明主要依据 README、CHANGELOG、`CLAUDE.md` 和 releases 页面整理而成
- 关于“归入 CLI 而不是 life”的判断，基于它的主价值是给 AI agent 暴露 n8n 的节点知识、模板搜索、校验和工作流操作工具面，而不是直接面向用户的自动化平台本体

## 更新观察点

- 优先观察节点覆盖率、模板元数据质量和 workflow validation 能力是否继续增强
- 持续看 CHANGELOG、README 和 releases，尤其留意安全修正、回滚机制和多客户端 setup 变化
- 如果后续把云端 dashboard、自托管和本地 n8n 集成边界做得更清晰，值得继续补进正文
