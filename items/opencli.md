---
title: "OpenCLI"
entity_type: "tool"
category: "CLI Tools"
last_reviewed_at: "2026-04-13"
---

# OpenCLI

## 一句话总结

一个把网站、浏览器会话、Electron 应用和本地命令统一变成可调用 CLI 的自动化中枢，适合人类和 AI Agent 共用。

## 快速判断

- 如果你想把“网页操作 + 浏览器登录态 + 本地 CLI + Electron 宿主”统一成一个 agent 可调用表面，它值得优先看
- 如果你只需要单一网站抓取或简单浏览器自动化，它可能比你的需求更大
- 它更像 agent-ready 的统一操作层，而不是单点爬虫或单点 browser automation 工具

## 你会怎么用它

- 接进 AI 开发流：把网页动作、桌面应用接管和本地 CLI passthrough 暴露给 Claude Code、Codex、OpenClaw 等 agent
- 接进日常工作流：把高频网页动作沉淀成确定性命令，而不是每次都开实时浏览器手工操作
- 最小落地方式：先用一个你已经登录的网站 + `opencli browser` + 一个本地 CLI 注册能力验证统一入口是否真的减少切换成本

## 它解决什么问题

- 网站操作、桌面应用控制和本地命令往往分散在不同自动化栈里，终端复用成本高
- Agent 想稳定调用网页、Electron 宿主和本地工具时，通常缺少统一命令层
- 重复操作难以沉淀成稳定、可复用的命令入口

## 适合谁

- 想把网站、浏览器和本地工具统一接给 Agent 的开发者
- 需要在终端里统一编排网页、桌面应用和本地命令的人
- 希望把重复操作沉淀成稳定 CLI 命令的自动化团队

## 核心能力

- Website -> CLI：把网站行为变成确定性的命令接口
- Browser automation：直接驱动浏览器完成点击、输入、提取和检查
- Electron adapters：让桌面应用进入统一接口层
- CLI hub：把本地已有命令也纳入统一的 Agent 可调用表面

## 能力边界

- 明显可用：需要把网站、浏览器桥、Electron 和本地命令放进同一个 agent 工作流
- 效果一般：只想做单站点抓取或轻量自动化，不需要统一命令层的场景
- 不要误用：它不是零摩擦开箱即用的纯云服务，浏览器桥、扩展和本地环境仍然需要配置

## 集成方式

- 作为单独工具：直接把它当统一 CLI 中枢使用，先调用内建 adapters 和 `browser`
- 作为 AI 工作流组件：放在 agent 的工具层，承接网页操作、浏览器控制、Electron 控制和 CLI passthrough
- 作为团队流程节点：把高频网页流程、桌面动作和本地命令收敛成统一命令契约

## 上手建议

- 第一步先跑 `opencli doctor`，确认 daemon、扩展和浏览器桥接都通
- 最值得先试的是你已经登录、且每天都要重复操作的网站
- 如果你只是偶尔做一次性网页点击，先轻量试用 `browser`，不必一上来就设计整套 adapter 流程

## 选型建议

- 如果你的主需求是“给 agent 一套统一且可复用的操作表面”，适合看它
- 如果你的主需求只是“抓网页内容”，更轻量的网页抓取或浏览器工具可能更合适
- 如果你同时需要 skills、CLI hub、Electron adapters 和网页登录态复用，它的价值会更明显

## 典型使用场景

- 给 Claude Code、Codex 或 OpenClaw 配一套可同时读网页、控桌面和调本地命令的终端工具链
- 把常做的网站操作沉淀成可重复执行的 CLI 命令
- 在研究型工作流里复用登录态浏览器，而不是每次从零写脚本

## 最近版本观察

- 2026-04-13 可见最新 release 为 `v1.7.3`
- 当前 README 已经把产品形态写得更完整：Browser Bridge 扩展、`doctor` 自检、skills 包安装、CLI hub、Electron adapters、87+ built-in adapters
- 这说明它不是只在堆适配器数量，而是在把“统一操作层”做成更完整的 agent 使用面

## 为什么值得关注

- 它不是单点工具，而是在做统一的人机共用操作层
- 对多工具、多宿主的 Agent 工作流来说，这种中枢型 CLI 比零散脚本更可持续
- 非常适合作为 `awesome-cli-for-ai` 里的“终端编排层”代表项目

## 类似项目

- [bb-browser](bb-browser.md) - 更聚焦“真实浏览器就是 API”，重点是直接复用登录态
- [Firecrawl CLI](firecrawl-cli.md) - 更偏网页抓取、搜索和 MCP / Skill 安装，不负责 Electron 宿主编排

## 官方链接

- **GitHub:** https://github.com/jackwener/opencli
- **更新记录:** https://github.com/jackwener/opencli/releases

## 标签

- `CLI Hub`, `浏览器自动化`, `Electron`, `Agent`, `终端工作流`

## 更新观察点

- 后续重点看新增了哪些网站适配器、Electron 宿主和 CLI passthrough 能力
- 优先持续观察 README 与 releases，跟踪浏览器桥接和桌面接管功能的演进
- 如果后续出现更成熟的 MCP 集成方式，值得补充到正文
