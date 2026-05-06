---
title: "Ruflo"
entity_type: "tool"
category: "Agent Shells"
last_reviewed_at: "2026-05-06"
---

# Ruflo

## 一句话总结

一个围绕 Claude Code 的多 agent orchestration shell，提供 CLI、MCP、hooks、plugins、memory、swarm 和 federation，把单 agent 会话扩成可持续协作的终端系统。

## 快速判断

- 如果你想把 Claude Code、Codex 之类单 agent coding 会话升级成多 agent 协作流，它值得优先看
- 如果你只想找一个轻量、单用途的 MCP server 或几个补充命令，先看别的方案
- 它更像一个给 agent 宿主加控制平面和执行编排层的 shell / orchestration system，不是普通独立 AI 应用

## 你会怎么用它

- 接进 AI 开发流：把 Ruflo 挂到 Claude Code 或 Codex 的终端工作流里，让 agent 能调用 memory、spawn、swarm、hooks 和 federation 能力
- 接进日常工作流：把多 agent 协作、背景 worker、插件化命令和任务路由沉淀成长期可复用的本地流程
- 最小落地方式：先区分 plugin install 和完整 `npx ruflo init` 两条路径，再用一个小型 coding 任务验证 hooks、spawn 和 memory 是否真的形成闭环

## 它解决什么问题

- 单个 coding agent 一旦任务变长、角色变多、上下文变重，就容易缺少稳定的协作与记忆层
- 许多团队想把 Claude Code 接到 MCP、hooks、background workers 和多 agent 分工，但自己搭控制平面的维护成本很高
- 即使有 agent shell，跨机器协作、持续记忆、插件扩展和策略控制也常常是分散拼装的

## 适合谁

- 想把 Claude Code、Codex 之类单 agent 会话升级成多 agent 协作流的开发者
- 需要在终端里把 hooks、memory、MCP、plugin 和 swarm orchestration 串起来的 AI 工程团队
- 想自托管 agent orchestration 能力，并逐步试用 plugin / full install 两条路径的人

## 核心能力

- 双安装路径：README 明确区分轻量 plugin install 和完整 CLI install，减少“装上去却调不到核心工具”的误解
- 多 agent 编排：强调 swarm、spawn、background worker、goal planning 和 agent team 协作能力
- MCP 工具面：提供大规模 MCP tool surface，把记忆、协调、训练和调度能力暴露给宿主 agent
- 持续记忆层：把 memory、AgentDB、向量检索和跨会话学习做成内建能力，而不是额外拼装
- 插件与扩展：支持 marketplace、官方插件和插件化 hooks 布局，适合逐步加能力
- 联邦协作：把跨机器、跨团队、跨信任边界的 agent communication 当成一等能力来设计

## 能力边界

- 明显可用：已经把 Claude Code 当长期工作台，希望加上多 agent 分工、记忆、路由和插件层的场景
- 效果一般：只需要一两个 MCP 工具、或者只是想偶尔让 agent 多开几个任务的轻量场景
- 不要误用：它不是“零配置就稳定接管一切”的极简工具；README 里自己也把 plugin install 和 full install 的能力差异写得很重

## 集成方式

- 作为单独工具：直接用 `npx ruflo init` 或 plugin marketplace 安装，给 Claude Code 加一层 orchestration shell
- 作为 AI 工作流组件：适合放在 agent 宿主外侧，承接 memory、spawn、swarm、hooks、federation 和 tool routing
- 作为团队流程节点：可以把任务拆解、并行 worker、跨机器协作和状态记忆沉淀成统一的终端协作面

## 上手建议

- 第一步先确认你要的是 plugin install 还是 full install，不要混淆两条路径的能力边界
- 最值得先试的是一个需要拆角色的小型 coding 任务，观察 hooks、spawn、memory 和 worker 协作是否真的减轻了主会话负担
- 如果你现在只是验证概念，先从单机、小任务、少插件开始，不要一上来就把全套 orchestration 压进生产流程

## 选型建议

- 如果你的主需求是给 Claude Code / Codex 增加长期运行的多 agent orchestration shell，它很值得看
- 如果你的主需求只是把某个外部系统暴露成 MCP 或 agent 工具，像 [n8n-MCP](n8n-mcp.md) 这类更轻、更聚焦
- 如果你的主需求是把不同软件快速变成 agent-native CLI，像 [CLI-Anything](cli-anything.md) 这种更偏工具面生成，而不是完整编排控制平面

## 典型使用场景

- 给 Claude Code 增加多 agent 分工、memory 和记忆回收能力
- 在终端里做带 hooks、worker 和 plugin 的持续 coding 流水线
- 让不同机器上的 agent 以联邦方式协作，而不是各自孤立运行

## 为什么值得关注

- 它不是只加几个 slash commands，而是在做一个完整的 agent orchestration shell
- README 和 changelog 都反复强调安装路径、hooks、生效边界和工具差异，说明它在快速补真实使用中的工程问题
- 除了 CLI / MCP 本体，它还把插件市场、goal planner、hosted UI 和 federation 串成了一条更大的 agent 协作路线

## 类似项目

- [n8n-MCP](n8n-mcp.md) - 更偏把 n8n 能力暴露成 agent 工具面；Ruflo 更偏为 Claude Code / Codex 增加完整 orchestration shell。
- [CLI-Anything](cli-anything.md) - 更偏快速把软件生成为 agent-native CLI；Ruflo 更偏管理已经接入宿主后的多 agent 协作与控制平面。
- [OpenCLI](opencli.md) - 更偏统一网页、浏览器、Electron 和本地命令的调用表面；Ruflo 更偏 agent 协调、记忆和任务编排层。

## 官方链接

- **官网:** https://flo.ruv.io/
- **GitHub:** https://github.com/ruvnet/ruflo
- **更新记录:** https://github.com/ruvnet/ruflo/releases

## 标签

- `Claude Code`, `Codex`, `MCP`, `Multi-Agent`, `Agent Orchestration`, `Hooks`

## 参考依据

- 这条说明主要依据 README、CHANGELOG、`AGENTS.md`、`CLAUDE.md` 和 releases 页面整理而成
- 关于“归入 CLI 而不是 coding 产品”的判断，基于它的主价值是给 Claude Code / Codex 提供 CLI、MCP、hooks、plugins、memory 和 swarm/federation 工具面，而不是单独面向终端用户的成品 AI 应用

## 更新观察点

- 优先关注 plugin install 与 full install 的能力边界是否继续收敛，避免 README 与真实可用面再次脱节
- 持续观察 releases 对 hooks、生效路径、spawn、MCP 配置和 package 体积的修正节奏
- 如果后续 Web UI、goal planner 和本地 orchestration shell 的边界更清晰，值得继续更新正文
