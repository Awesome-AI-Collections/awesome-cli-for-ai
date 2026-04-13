---
title: "Ghostty"
entity_type: "tool"
category: "Terminal UX"
last_reviewed_at: "2026-04-13"
---

# Ghostty

## 一句话总结

一个强调原生 UI、性能和现代终端体验的终端应用，适合承载 AI agent TUI、长会话 shell 与 terminal-first 工作流。

## 快速判断

- 如果你把 Claude Code、Codex、Gemini CLI 这类 agent 长时间跑在终端里，它值得看
- 如果你只想找一个“能开 shell 就行”的最基础终端，不一定需要它的现代终端体验
- 它更像 AI CLI 工作台的运行底座，而不是 AI 能力本身

## 你会怎么用它

- 接进 AI 开发流：把它作为 Claude Code、Codex、Gemini CLI、`tmux` 和各类 agent TUI 的长期运行环境
- 接进日常工作流：把多标签、多窗口和 shell 集成组合成固定的终端工作台
- 最小落地方式：先用它承载你最常开的 1 到 2 个 agent CLI 会话，看体验是否明显优于现有终端

## 它解决什么问题

- 很多 AI CLI 会长时间占据终端，需要更顺手的窗口、标签和输入体验
- agent TUI、日志流和长会话 shell 对性能与渲染质量比较敏感
- terminal-first 用户希望减少在终端工作台上的摩擦，而不是只关注单个命令

## 适合谁

- 长时间在终端里跑 AI agent 和开发工作流的开发者
- 把终端当作主工作台的人
- 重视现代终端体验、性能和集成能力的重度 CLI 用户

## 核心能力

- 现代终端体验：强调流畅、原生且长期可用的桌面终端体验
- AI agent TUI 友好：适合承载长时间运行的 CLI agent 和交互式 TUI
- shell 集成：方便把提示、目录、会话上下文和终端习惯串起来
- 工作台属性强：适合形成固定的 terminal-first 使用环境

## 能力边界

- 明显可用：作为 AI CLI 和多会话 shell 的日常终端底座
- 效果一般：如果你只把终端当临时启动器，它的价值不会特别明显
- 不要误用：它不是 AI agent、本身也不负责 provider 路由、MCP 或自动化编排

## 集成方式

- 作为单独工具：直接替换当前终端应用，作为日常主终端
- 作为 AI 工作流组件：放在最外层承载 `tmux`、agent CLI、日志观察和远程会话
- 作为团队流程节点：适合团队成员统一一套更稳定的终端工作台习惯

## 上手建议

- 先不要一开始就迁移全部工作流，优先让 1 个主力 agent CLI 和 1 个 `tmux` 工作区落在里面
- 最值得先试的是长时间运行的 agent 或监控型终端任务
- 如果你当前终端已经很顺手，可以先把它当增量试用，而不是立刻全量切换

## 选型建议

- 如果你的主需求是“给 AI agent TUI 找一个更好的运行底座”，适合看它
- 如果你的主需求是“获得 AI 能力”，它不是这类工具
- 如果你在选的是终端基础设施而不是具体 agent，本条目有价值

## 为什么值得关注

- 对重度 AI CLI 用户来说，终端本身就是生产环境的一部分
- 它收录的理由不是“是终端”，而是“直接影响 AI agent TUI 的长期使用体验”
- 这类基础设施往往比单个技巧更影响每天的真实摩擦成本

## 类似项目

- [Mosh](mosh.md) - 同样属于终端体验基础设施，但核心问题是弱网远程会话而不是本地终端工作台
- [iTerm2](iterm2.md) - 同样是终端工作台，但更偏成熟稳定的 macOS 老牌方案

## 官方链接

- **官网:** https://ghostty.org/
- **GitHub:** https://github.com/ghostty-org/ghostty

## 标签

- `Terminal`, `TUI`, `CLI`, `Agent`, `Workspace`

## 更新观察点

- 后续重点看平台支持、shell integration、窗口体验和配置能力的演进
- 优先重新抓取官网、文档和 releases
- 如果后续对 AI agent TUI、远程会话或可观测性支持出现新变化，值得补进正文
