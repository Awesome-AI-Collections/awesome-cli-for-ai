---
title: "engraph"
entity_type: "tool"
category: "MCP / Tooling"
last_reviewed_at: "2026-04-11"
---

# engraph

## 一句话总结

一个把 Obsidian vault 变成 AI agent 可调用知识 API 的本地二进制，集成 hybrid search、MCP server、HTTP REST API 和可写回笔记的工具层。

## 它解决什么问题

- AI agent 想访问个人笔记或团队知识库时，往往只能拿到零散文本，缺少结构化检索与写回能力。
- 传统向量检索不理解笔记之间的 wikilink、时间关系和上下文结构，很难真正变成“知识图谱”。
- 团队想给 Claude Code、Cursor 或 Web agents 接本地知识库时，经常缺少一个既能 CLI 使用、又能 MCP / HTTP 暴露的统一入口。

## 适合谁

- 想让 Claude Code、Cursor 或其他 MCP client 直接访问本地笔记库的开发者
- 需要本地 hybrid search、MCP 和 REST API 组合能力的 agent builder
- 使用 Obsidian 做知识管理并偏好 terminal-first 工具链的人

## 核心能力

- 本地索引与 hybrid search：把 Markdown vault 建成支持 embedding、全文、图遍历、时间感知和 rerank 的本地索引。
- MCP server：`engraph serve` 可直接向 AI agents 暴露搜索、读取、section 级编辑、frontmatter 变更等工具。
- HTTP API：可额外开启 REST API，方便 Web agents、脚本和 ChatGPT Actions 接入。
- 笔记写回：支持按 heading 精准改段落、改 frontmatter、创建或删除笔记，而不是只做只读搜索。

## 典型使用场景

- 给 Claude Code 接一个可搜索、可编辑的 Obsidian 知识库，让 agent 直接读取和整理笔记。
- 在终端里用 `engraph search`、`engraph context`、`engraph write` 组合自己的知识工作流。
- 把本地 vault 通过 MCP 或 HTTP 暴露给其他 agent、自动化脚本或 ChatGPT Actions。

## 为什么值得关注

- 它不是单纯的 MCP 包装，而是把索引、搜索、上下文打包、写回和服务层做成了一体化本地二进制。
- README 对 CLI、MCP、REST、Obsidian 集成和模型下载路径都写得很完整，落地感很强。
- 对 `awesome-cli-for-ai` 来说，这种“本地 binary + MCP + HTTP + agent write-back”组合非常有代表性。

## 类似项目

- [Firecrawl CLI](firecrawl-cli.md) - 同样强调给 agent 提供 CLI 与 MCP 能力，但 `engraph` 面向的是本地知识库而不是网页抓取。
- [OpenCLI](opencli.md) - 更像把网站和应用统一包装成命令入口，而 `engraph` 更专注 Obsidian vault intelligence 与知识 API。

## 官方链接

- **GitHub:** https://github.com/devwhodevs/engraph
- **更新记录:** https://github.com/devwhodevs/engraph/releases
- **ChatGPT Actions 指南:** https://github.com/devwhodevs/engraph#chatgpt-actions-optional

## 标签

- `Obsidian`, `CLI`, `MCP`, `Knowledge Graph`, `Hybrid Search`

## 更新观察点

- 后续重点看 5-lane hybrid search、temporal lane 和 reranker 的默认体验是否继续成熟。
- 持续关注 MCP tools、HTTP endpoints 和 write pipeline 的能力边界，尤其是 section 级编辑与身份上下文。
- 优先重抓 README、CHANGELOG 和 releases，确认模型依赖、安装路径和 Obsidian integration 是否变化。
