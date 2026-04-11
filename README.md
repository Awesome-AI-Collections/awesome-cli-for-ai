# Awesome CLI for AI

面向中文读者整理的 AI CLI 工具、命令行工作流与终端生态。

## 推荐

- [Agent Reach](items/agent-reach.md) - 一个给 AI Agent 补齐跨平台互联网读取能力的开源工具集，统一接入 YouTube、Twitter/X、Reddit、小红书、B站、GitHub 和 RSS 等数据来源。
- [agent-browser](items/agent-browser.md) - Vercel Labs 开源的浏览器自动化 CLI，专门给 AI agents 提供网页导航、点击、表单填写、截图、网络拦截和批处理能力。
- [bb-browser](items/bb-browser.md) - 一个把真实已登录浏览器直接变成 API / CLI / MCP 接口的工具，让 AI Agent 低成本访问多平台内容与交互能力。
- [OpenCLI](items/opencli.md) - 一个把网站、浏览器会话、Electron 应用和本地命令行统一暴露给人类与 AI Agent 的自动化 CLI 中枢。

## 从哪里开始

- 如果你先想找开箱即用的终端工具，先看 `CLI Tools`。
- 如果你更关心终端里的 agent 协作、MCP 和工具链编排，先看 `Agent Shells`、`MCP / Tooling` 或 `Workflow Automation`。

## 分类浏览

### CLI Tools

适合直接在终端里调用的 AI CLI 工具和命令行入口。

- [GitHub CLI](items/github-cli.md) - GitHub 官方命令行工具，把 PR、Issue、Actions 等 GitHub 工作流直接带进终端。
- [Google Workspace CLI](items/google-workspace-cli.md) - 一个覆盖 Drive、Gmail、Calendar、Sheets、Docs、Chat 等 Google Workspace 能力的统一命令行工具，并内置 AI agent skills。
- [imsg](items/imsg.md) - 一个把 Apple Messages.app 接进终端的 CLI，让 AI agent 能发送和接收短信与 iMessage。
- [Lark CLI](items/lark-cli.md) - 飞书 / Lark 官方 CLI，覆盖消息、文档、Base、Sheets、Calendar、Mail、Tasks、Meetings 等能力，并面向 humans 与 AI Agents 设计。
- [OpenCLI](items/opencli.md) - 一个把网站、浏览器会话、Electron 应用和本地命令行统一暴露给人类与 AI Agent 的自动化 CLI 中枢。
- [Vercel CLI](items/vercel-cli.md) - Vercel 官方命令行工具，用来在终端里完成项目拉取、开发、部署与环境管理。
- [wecom-cli](items/wecom-cli.md) - 企业微信开放平台命令行工具，让人类和 AI Agent 都能在终端中操作企业微信。

### Agent Shells

适合把 AI agent 长时间运行在 shell / terminal 工作流里的工具。

- [agent-browser](items/agent-browser.md) - Vercel Labs 开源的浏览器自动化 CLI，专门给 AI agents 提供网页导航、点击、表单填写、截图、网络拦截和批处理能力。
- [browser-use](items/browser-use.md) - 一个面向 AI agents 的浏览器自动化项目，既提供 Python agent 框架，也提供持久化浏览器 CLI 与 cloud runtime。

### MCP / Tooling

适合在终端里管理 MCP、工具接入和 agent 扩展能力。

- [Agent Reach](items/agent-reach.md) - 一个给 AI Agent 补齐跨平台互联网读取能力的开源工具集，统一接入 YouTube、Twitter/X、Reddit、小红书、B站、GitHub 和 RSS 等数据来源。
- [bb-browser](items/bb-browser.md) - 一个把真实已登录浏览器直接变成 API / CLI / MCP 接口的工具，让 AI Agent 低成本访问多平台内容与交互能力。
- [Firecrawl CLI](items/firecrawl-cli.md) - Firecrawl 的命令行接口，可在终端里完成 scrape、crawl、search，并为 AI agent 安装 skills 与 MCP。

## 后续补充方向

- `Provider Switching / Routing`: 适合统一切模型、切 provider、切路由策略的命令行工具。
- `Prompt / Context Management`: 适合维护提示词、上下文模板和会话输入资产。
- `Workflow Automation`: 适合把终端 AI 能力串进脚本、任务流和批处理流程。
- `Terminal UX`: 适合增强终端交互体验、可视化、多会话与工作区切换。
- `Observability / Usage`: 适合查看 token、成本、日志、使用量和 agent 运行状态。

## 收录标准

- 只收录与 `awesome-cli-for-ai` 对应主题直接相关的公开内容
- 只保留公开可见的官方链接，不保留内部 intake 来源
