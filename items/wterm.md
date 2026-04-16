---
title: "wterm"
entity_type: "tool"
category: "Terminal UX"
last_reviewed_at: "2026-04-16"
---

# wterm

## 一句话总结

一个面向浏览器和 agent shell 场景的 Web 终端渲染组件，适合给 AI CLI、终端工作台和 Web IDE 提供可嵌入的终端界面。

## 快速判断

- 如果你正在做浏览器里的终端、agent shell 或 AI coding 工作台，它值得优先看
- 如果你要的是开箱即用的 AI CLI 产品，而不是终端基础件，先看别的方案
- 它更像 terminal UX 基础件和可嵌入终端层，不是 AI 产品本体

## 你会怎么用它

- 接进 AI 开发流：把它作为 Web IDE、agent shell 或浏览器工作台里的终端渲染层，承接命令执行、日志流和交互输入
- 接进日常工作流：把本地或远端 shell 会话嵌进团队内部工具、运维面板或调试工作台
- 最小落地方式：先用 `@wterm/react` 或 `@wterm/dom` 接一个最小 WebSocket PTY 后端，验证输入、渲染和滚动体验

## 它解决什么问题

- 很多 AI 工作台和 Web IDE 需要终端能力，但直接自己做终端渲染成本高
- 传统 canvas 终端虽然成熟，但选择、复制、查找和可访问性体验不总是理想
- agent shell 场景需要一个能嵌入浏览器、又足够轻量的终端界面层

## 适合谁

- 在做 Web IDE、AI coding 工作台和 agent shell 的团队
- 需要把终端能力嵌进浏览器产品的前端或平台工程师
- 关心选择、复制、查找和可访问性体验的终端产品设计者

## 核心能力

- DOM 渲染：直接渲染到 DOM，天然拥有文本选择、复制粘贴、浏览器查找和辅助功能支持
- Zig + WASM 核心：用 Zig 编写终端核心并编译成 WASM，兼顾体积和性能
- 多封装形态：同时提供 headless core、vanilla JS、React 组件和 hook
- WebSocket 传输：适合接 PTY 后端或远程 shell 会话
- 终端兼容性：支持常见 escape sequence、alternate screen、scrollback、主题和自动 resize

## 能力边界

- 明显可用：浏览器终端、agent shell、Web 运维面板、在线调试工具、AI coding 工作台
- 效果一般：只需要一个本地终端 App 的场景，或不打算做浏览器终端嵌入的团队
- 不要误用：不要把它当成 AI CLI、终端 App 或完整 agent 平台；它主要是终端界面基础件

## 集成方式

- 作为单独工具：直接把 `@wterm/dom` 或 `@wterm/react` 嵌到 Web 页面中
- 作为 AI 工作流组件：放在 agent shell / Web IDE 的终端展示层，下接 PTY、容器或远程执行后端
- 作为团队流程节点：适合给内部平台提供统一终端交互层，减少各产品重复造终端 UI

## 上手建议

- 第一步先用最小 PTY 或回显后端验证渲染、输入和滚动表现
- 最值得先试的是“浏览器里跑 agent shell”或“Web IDE 内嵌终端”场景
- 如果你只是想找现成 CLI，不要一开始就投入集成，它不是终端产品终态

## 选型建议

- 如果你的主需求是给 Web 里的 agent shell 或终端工作台提供终端界面，适合看它
- 如果你的主需求是直接给开发者提供完整 AI 编码产品，更适合看 `awesome-ai-for-coding`
- 如果你最在意的是浏览器终端里的原生选择、复制和查找体验，它的 DOM 渲染路线值得关注

## 为什么值得关注

- 它切的不是“再做一个终端 App”，而是“给 Web 终端和 agent shell 做更顺手的界面层”
- DOM 渲染路线让浏览器原生交互能力成为优势，而不是额外补丁
- 对正在搭 AI coding 工作台或 agent shell 的团队来说，这类基础件能明显降低前端终端实现成本

## 类似项目

- [GhostVM](ghostvm.md) - 更偏 agent 可调用的 workspace 控制面；wterm 更偏浏览器终端界面层。
- [bb-browser](bb-browser.md) - 更偏 browser tool surface；wterm 更偏 terminal UX 和 shell 展示层。

## 官方链接

- **GitHub:** https://github.com/vercel-labs/wterm
- **更新记录:** https://github.com/vercel-labs/wterm/releases

## 标签

- `Terminal UX`, `Web Terminal`, `WASM`, `Zig`, `Agent Shell`

## 参考依据

- 这条说明主要依据项目 README、GitHub 项目页和 releases 页面整理而成
- 关于“归入 CLI 而不是 coding”的判断，基于它的核心价值是 terminal UX 基础件，主要服务 agent shell 和终端工作台，而不是直接面向开发者的 AI 产品

## 更新观察点

- 后续优先观察 PTY 后端接入示例、协议稳定性和 React 集成深度
- 关注兼容性、性能和无障碍能力是否继续增强
- 如果后续从基础件明显扩展成完整终端产品，需要重新复核 repo 归属
