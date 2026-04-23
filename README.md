# Awesome CLI for AI

面向中文读者整理的 AI CLI 工具、命令行工作流与终端生态。

## 推荐

- [Agent Reach](items/agent-reach.md) - 一个给 AI Agent 补齐跨平台互联网读取能力的开源工具集，统一接入 YouTube、Twitter/X、Reddit、小红书、B站、GitHub 和 RSS 等数据来源。
- [agent-browser](items/agent-browser.md) - Vercel Labs 开源的浏览器自动化 CLI，专门给 AI agents 提供网页导航、点击、表单填写、截图、网络拦截和批处理能力。
- [awesome-connected-cli](items/awesome-connected-cli.md) - 一个把抓取、AI 处理和多平台输出串成一条龙自动化的 CLI 工具箱。
- [bb-browser](items/bb-browser.md) - 一个把真实已登录浏览器直接变成 API / CLI / MCP 接口的工具，让 AI Agent 低成本访问多平台内容与交互能力。
- [CC-Switch CLI](items/cc-switch-cli.md) - 一个统一管理 Claude Code、Codex、Gemini、OpenCode 与 OpenClaw 配置、MCP、提示词和环境检查的跨平台 CLI 工具。
- [CLI-Anything](items/cli-anything.md) - 一个把任意软件快速变成 agent-native CLI 的框架，支持为 Claude Code、Codex、OpenClaw 等代理生成可调用命令层和对应技能定义。
- [jina-cli](items/jina-cli.md) - 一个把任意网页转换成 LLM 友好输入的 CLI，支持 read 与 search，并可直接接入 Claude Code 或 OpenClaw。
- [OpenCLI](items/opencli.md) - 一个把网站、浏览器会话、Electron 应用和本地命令行统一暴露给人类与 AI Agent 的自动化 CLI 中枢。

## 从哪里开始

- 如果你先想找开箱即用的终端工具，先看 `CLI Tools`。
- 如果你更关心终端里的 agent 协作、MCP 和工具链编排，先看 `Agent Shells`、`MCP / Tooling` 或 `Workflow Automation`。

## 分类浏览

### CLI Tools

适合直接在终端里调用的 AI CLI 工具和命令行入口。

- [aria2](items/aria2.md) - 一个支持 HTTP、FTP、SFTP、BitTorrent 和 Metalink 的轻量级命令行下载工具。
- [AutoCLI](items/autocli.md) - 一个让 AI Agent 通过单条命令读取网站、桌面应用和本地 CLI 的 Rust 工具。
- [bird](items/bird.md) - 一个面向 Twitter/X 的 CLI，让人类和 AI agents 能在终端里发推、读流和执行社交操作。
- [CLI-Anything](items/cli-anything.md) - 一个把任意软件快速变成 agent-native CLI 的框架，支持为 Claude Code、Codex、OpenClaw 等代理生成可调用命令层和对应技能定义。
- [Defuddle](items/defuddle.md) - 一个可从网页或 HTML 中提取正文并输出干净 HTML 或 Markdown 的内容抽取工具，支持浏览器、Node.js 和 CLI 使用。
- [DingTalk Workspace CLI](items/dingtalk-workspace-cli.md) - 钉钉官方的企业工作台 CLI，可让人类和 AI agents 以结构化方式访问企业数据、自动化工作流并保持审计边界。
- [Dreamina CLI](items/dreamina-cli.md) - 一个面向 AI agent 的创作命令行工具，可用即梦 / Dreamina 账号完成文生图、文生视频、图生图和图生视频任务。
- [FFmpeg](items/ffmpeg.md) - 一个功能极强的开源音视频处理工具，支持转码、剪辑、合并、滤镜和流媒体处理。
- [gh-stack](items/gh-stack.md) - 一个面向 stacked PR 工作流的 GitHub CLI extension，帮助开发者把大改动拆成多层可审查 PR，并自动处理分支、rebase、push 和 PR 基线关系。
- [GhostVM](items/ghostvm.md) - 一个通过 GhostVM 工作区与 `vmctl` 命令面管理隔离 macOS 环境的工具，适合给 AI agents 和开发任务分配独立 workspace。
- [GitHub CLI](items/github-cli.md) - GitHub 官方命令行工具，把 PR、Issue、Actions 等 GitHub 工作流直接带进终端。
- [Google Workspace CLI](items/google-workspace-cli.md) - 一个覆盖 Drive、Gmail、Calendar、Sheets、Docs、Chat 等 Google Workspace 能力的统一命令行工具，并内置 AI agent skills。
- [ImageMagick](items/imagemagick.md) - 一个支持 200 多种格式的图片处理套件，适合在终端里做转换、裁剪、合成和批量自动化处理。
- [imsg](items/imsg.md) - 一个把 Apple Messages.app 接进终端的 CLI，让 AI agent 能发送和接收短信与 iMessage。
- [jina-cli](items/jina-cli.md) - 一个把任意网页转换成 LLM 友好输入的 CLI，支持 read 与 search，并可直接接入 Claude Code 或 OpenClaw。
- [Lark CLI](items/lark-cli.md) - 飞书 / Lark 官方 CLI，覆盖消息、文档、Base、Sheets、Calendar、Mail、Tasks、Meetings 等能力，并面向 humans 与 AI Agents 设计。
- [ncm-cli](items/ncm-cli.md) - 一个面向网易云音乐的命令行客户端，支持搜索、播放、歌单管理和 TUI 播放器，并可接入 AI agent。
- [OfficeCLI](items/officecli.md) - 一个让 AI agents 直接读取、编辑和生成 Word、Excel、PowerPoint 文件的 Office 自动化 CLI，无需安装 Microsoft Office。
- [OpenCLI](items/opencli.md) - 一个把网站、浏览器会话、Electron 应用和本地命令行统一暴露给人类与 AI Agent 的自动化 CLI 中枢。
- [Pandoc](items/pandoc.md) - 一个通用文档格式转换器，支持 Markdown、HTML、LaTeX、PDF、DOCX、EPUB 等多种格式互转。
- [rclone](items/rclone.md) - 一个覆盖大量云存储与对象存储后端的命令行同步工具，适合在终端里统一做传输、备份、挂载和自动化数据流转。
- [ripgrep](items/ripgrep.md) - 一个极快的递归文本搜索工具，默认尊重 .gitignore，适合在大型代码库中替代 grep 做模式搜索。
- [rtk](items/rtk.md) - 一个面向 Claude Code、Cursor、Gemini CLI 等工具的 CLI 代理层，可压缩常见开发命令输出，减少进入模型上下文的 token 开销。
- [textutil](items/textutil.md) - macOS 自带的文档与富文本转换 CLI，可在终端里查看、拼接并转换 TXT、HTML、RTF、DOCX、ODT 等格式。
- [Vercel CLI](items/vercel-cli.md) - Vercel 官方命令行工具，用来在终端里完成项目拉取、开发、部署与环境管理。
- [wecom-cli](items/wecom-cli.md) - 企业微信开放平台命令行工具，让人类和 AI Agent 都能在终端中操作企业微信。
- [wttr.in](items/wttr-in.md) - 一个面向终端和脚本的天气服务，可通过 curl 等命令直接返回 ANSI、纯文本、JSON、PNG 和指标格式天气信息。
- [xurl](items/xurl.md) - 一个面向 X API 的 curl 风格命令行客户端，支持多 app、多账号和 OAuth 流程，适合把社交平台接口接进 agent 或终端自动化流程。
- [yt-dlp](items/yt-dlp.md) - 一个功能很全的命令行音视频下载器，适合自动化拉取网页媒体内容。

### Agent Shells

适合把 AI agent 长时间运行在 shell / terminal 工作流里的工具。

- [agent-browser](items/agent-browser.md) - Vercel Labs 开源的浏览器自动化 CLI，专门给 AI agents 提供网页导航、点击、表单填写、截图、网络拦截和批处理能力。
- [Browser Harness](items/browser-harness.md) - 一个直接连 Chrome CDP 的自愈式浏览器 harness，允许 Claude Code / Codex 在任务中动态补 helper，适合真实浏览器网页任务。
- [browser-use](items/browser-use.md) - 一个面向 AI agents 的浏览器自动化项目，既提供 Python agent 框架，也提供持久化浏览器 CLI 与 cloud runtime。

### Provider Switching / Routing

适合统一切模型、切 provider、切路由策略的命令行工具。

- [CC-Switch CLI](items/cc-switch-cli.md) - 一个统一管理 Claude Code、Codex、Gemini、OpenCode 与 OpenClaw 配置、MCP、提示词和环境检查的跨平台 CLI 工具。

### MCP / Tooling

适合在终端里管理 MCP、工具接入和 agent 扩展能力。

- [Agent Reach](items/agent-reach.md) - 一个给 AI Agent 补齐跨平台互联网读取能力的开源工具集，统一接入 YouTube、Twitter/X、Reddit、小红书、B站、GitHub 和 RSS 等数据来源。
- [bb-browser](items/bb-browser.md) - 一个把真实已登录浏览器直接变成 API / CLI / MCP 接口的工具，让 AI Agent 低成本访问多平台内容与交互能力。
- [Cloudflare Browser Rendering](items/cloudflare-browser-rendering.md) - Cloudflare Browser Rendering 新增 CDP endpoint 与 MCP client 支持，让现有 Puppeteer、Playwright 和 chrome-devtools-mcp 工具能直接连到 Cloudflare 的远程浏览器。
- [engraph](items/engraph.md) - 一个把 Obsidian vault 变成可供 AI agent 调用的本地知识图谱二进制，集成 hybrid search、MCP server 和 HTTP API。
- [Firecrawl CLI](items/firecrawl-cli.md) - Firecrawl 的命令行接口，可在终端里完成 scrape、crawl、search，并为 AI agent 安装 skills 与 MCP。
- [FlowMind for Claude](items/flowmind-for-claude.md) - 一个把 FlowMind 任务与笔记系统接进 Claude Code 和 MCP 客户端的 skill / MCP 工具，让你在终端里直接管理 goals、tasks、notes 与 people。
- [KBB](items/kbb.md) - 一个面向 Claude Code 的知识库文章生成 CLI / MCP：把研究、资料采集、MarkItDown 转换、画图和发布串成一条命令式流水线。
- [OneCLI](items/onecli.md) - 一个给 AI agents 统一管理和注入 API 密钥的开源凭据网关，让 agents 用占位符调用服务而不直接接触真实 secrets。
- [Shopify AI Toolkit](items/shopify-ai-toolkit.md) - Shopify 官方的 AI 工具接入方案，支持通过 plugin、skills 或 MCP 把平台文档、API schema、代码校验和店铺操作能力接入 agent 工具链。

### Prompt / Context Management

适合维护提示词、上下文模板和会话输入资产。

- [DESIGN.md](items/design-md.md) - Google Labs 推出的开放设计规范与 CLI，用一份 `DESIGN.md` 同时描述 design tokens 和设计 rationale，帮助 coding agents 更稳定地继承同一套视觉系统。
- [AI Agent Skills](items/ai-agent-skills.md) - 一个跨 agent 的 skill 发现与安装 CLI，用 `npx ai-agent-skills` 就能搜索、浏览并安装适配 Claude Code、Codex、Cursor、VS Code 等环境的 skills。
- [Khazix Skills](items/khazix-skills.md) - 一个把深度研究与长文写作方法论沉淀成 prompts 和可安装 skills 的开源仓库，适合给 Claude Code、Codex、OpenClaw 等 agent 直接装配方法论能力。

### Workflow Automation

适合把终端 AI 能力串进脚本、任务流和批处理流程。

- [1Password SSH](items/onepassword-ssh.md) - 1Password 的 SSH 与 Git 集成功能，可把密钥管理、签名和终端认证流程整合进开发者与 agent 的命令行工作流。
- [awesome-connected-cli](items/awesome-connected-cli.md) - 一个把抓取、AI 处理和多平台输出串成一条龙自动化的 CLI 工具箱。
- [Logo Generator Skill](items/logo-generator-skill.md) - 一个面向 Claude Code 等宿主的品牌设计 skill，可让 agent 直接生成 SVG logo 方案和展示图。
- [notebooklm-py](items/notebooklm-py.md) - NotebookLM 的非官方 Python API 与 CLI，支持程序化访问、agentic skill 和本地自动化。
- [Obsidian CLI](items/obsidian-cli.md) - Obsidian 官方命令行接口，把知识库读写、TUI、无头同步和自动化工作流带进终端与脚本环境。
- [Show Me The Money](items/show-me-the-money.md) - 一个给 Claude Code 和 Codex CLI 用的商业变现技能包，用 `/money` 等 workflow 把点子推进到客户与收入动作。

### Terminal UX

适合增强终端交互体验、可视化、多会话与工作区切换。

- [Mosh](items/mosh.md) - 一个面向不稳定网络环境的移动终端 shell，用更稳的远程会话、漫游和本地回显体验替代传统交互式 SSH。
- [wterm](items/wterm.md) - 面向浏览器和 agent shell 场景的 Web 终端渲染组件，适合给 AI CLI 或终端工作台提供可嵌入终端界面。

## 后续补充方向

- `Observability / Usage`: 适合查看 token、成本、日志、使用量和 agent 运行状态。

## 收录标准

- 只收录与 `awesome-cli-for-ai` 对应主题直接相关的公开内容
- 只保留公开可见的官方链接，不保留内部 intake 来源
