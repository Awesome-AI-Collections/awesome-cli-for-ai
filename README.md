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

- [aria2](items/aria2.md) - 一个支持 HTTP、FTP、SFTP、BitTorrent 和 Metalink 的轻量级命令行下载工具。
- [bird](items/bird.md) - 一个面向 Twitter/X 的 CLI，让人类和 AI agents 能在终端里发推、读流和执行社交操作。
- [GitHub CLI](items/github-cli.md) - GitHub 官方命令行工具，把 PR、Issue、Actions 等 GitHub 工作流直接带进终端。
- [Google Workspace CLI](items/google-workspace-cli.md) - 一个覆盖 Drive、Gmail、Calendar、Sheets、Docs、Chat 等 Google Workspace 能力的统一命令行工具，并内置 AI agent skills。
- [imsg](items/imsg.md) - 一个把 Apple Messages.app 接进终端的 CLI，让 AI agent 能发送和接收短信与 iMessage。
- [Lark CLI](items/lark-cli.md) - 飞书 / Lark 官方 CLI，覆盖消息、文档、Base、Sheets、Calendar、Mail、Tasks、Meetings 等能力，并面向 humans 与 AI Agents 设计。
- [OpenCLI](items/opencli.md) - 一个把网站、浏览器会话、Electron 应用和本地命令行统一暴露给人类与 AI Agent 的自动化 CLI 中枢。
- [rclone](items/rclone.md) - 一个覆盖大量云存储与对象存储后端的命令行同步工具，适合在终端里统一做传输、备份、挂载和自动化数据流转。
- [Vercel CLI](items/vercel-cli.md) - Vercel 官方命令行工具，用来在终端里完成项目拉取、开发、部署与环境管理。
- [wecom-cli](items/wecom-cli.md) - 企业微信开放平台命令行工具，让人类和 AI Agent 都能在终端中操作企业微信。
- [wttr.in](items/wttr-in.md) - 一个面向终端和脚本的天气服务，可通过 curl 等命令直接返回 ANSI、纯文本、JSON、PNG 和指标格式天气信息。
- [yt-dlp](items/yt-dlp.md) - 一个功能很全的命令行音视频下载器，适合自动化拉取网页媒体内容。

### Agent Shells

适合把 AI agent 长时间运行在 shell / terminal 工作流里的工具。

- [agent-browser](items/agent-browser.md) - Vercel Labs 开源的浏览器自动化 CLI，专门给 AI agents 提供网页导航、点击、表单填写、截图、网络拦截和批处理能力。
- [browser-use](items/browser-use.md) - 一个面向 AI agents 的浏览器自动化项目，既提供 Python agent 框架，也提供持久化浏览器 CLI 与 cloud runtime。

### MCP / Tooling

适合在终端里管理 MCP、工具接入和 agent 扩展能力。

- [Agent Reach](items/agent-reach.md) - 一个给 AI Agent 补齐跨平台互联网读取能力的开源工具集，统一接入 YouTube、Twitter/X、Reddit、小红书、B站、GitHub 和 RSS 等数据来源。
- [bb-browser](items/bb-browser.md) - 一个把真实已登录浏览器直接变成 API / CLI / MCP 接口的工具，让 AI Agent 低成本访问多平台内容与交互能力。
- [Firecrawl CLI](items/firecrawl-cli.md) - Firecrawl 的命令行接口，可在终端里完成 scrape、crawl、search，并为 AI agent 安装 skills 与 MCP。

### Workflow Automation

适合把终端 AI 能力串进脚本、任务流和批处理流程。

- [1Password SSH](items/onepassword-ssh.md) - 1Password 的 SSH 与 Git 集成功能，可把密钥管理、签名和终端认证流程整合进开发者与 agent 的命令行工作流。
- [notebooklm-py](items/notebooklm-py.md) - NotebookLM 的非官方 Python API 与 CLI，支持程序化访问、agentic skill 和本地自动化。
- [Obsidian CLI](items/obsidian-cli.md) - Obsidian 官方命令行接口，把知识库读写、TUI、无头同步和自动化工作流带进终端与脚本环境。

### Terminal UX

适合增强终端交互体验、可视化、多会话与工作区切换。

- [Mosh](items/mosh.md) - 一个面向不稳定网络环境的移动终端 shell，用更稳的远程会话、漫游和本地回显体验替代传统交互式 SSH。

## 后续补充方向

- `Provider Switching / Routing`: 适合统一切模型、切 provider、切路由策略的命令行工具。
- `Prompt / Context Management`: 适合维护提示词、上下文模板和会话输入资产。
- `Observability / Usage`: 适合查看 token、成本、日志、使用量和 agent 运行状态。

## 收录标准

- 只收录与 `awesome-cli-for-ai` 对应主题直接相关的公开内容
- 只保留公开可见的官方链接，不保留内部 intake 来源
