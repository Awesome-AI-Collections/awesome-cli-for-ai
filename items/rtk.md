---
title: "rtk"
entity_type: "tool"
category: "CLI Tools"
last_reviewed_at: "2026-04-11"
---

# rtk

## 一句话总结

一个面向 Claude Code、Cursor、Gemini CLI 等工具的 Rust CLI 代理层，会在命令输出进入模型上下文前先做过滤、分组和压缩，减少常见开发命令的 token 开销。

## 它解决什么问题

- AI coding agent 在 `git status`、`rg`、测试输出和构建日志上很容易浪费大量上下文。
- 很多 shell 命令本身对人类可读，但对模型来说噪音太多，既贵又影响后续推理空间。
- 团队想统一优化多种 AI CLI 的终端输出时，不想自己为每个宿主单独维护一套 hook 和过滤脚本。

## 适合谁

- 重度使用 Claude Code、Codex、Cursor、Gemini CLI 等工具的开发者
- 希望降低命令输出 token 成本的 AI coding agent 用户
- 想把 shell 输出压缩层接进终端 agent 工作流的团队

## 核心能力

- 命令输出压缩：针对 `git`、测试、lint、`ls`、`grep`、`docker`、`aws` 等常见命令做定制化压缩。
- 多宿主集成：支持通过 hook 或插件接入 Claude Code、Cursor、Gemini CLI、OpenCode 等工具。
- 透明代理：把原始命令自动改写为 `rtk` 版本，尽量不改变日常使用习惯。
- 节省分析：自带 `rtk gain` 等统计命令，帮助查看 token 节省情况和命令覆盖率。

## 典型使用场景

- 在 Claude Code 里把 `git status`、`pytest`、`npm test` 这类高噪声输出压成更适合模型消费的摘要。
- 在多种 AI CLI 工具之间统一安装一层终端压缩代理，减少每个宿主都单独调优。
- 给团队的 agent 工作流做上下文成本治理，避免日志和构建输出挤占有效推理空间。

## 为什么值得关注

- 它不是另一个 coding agent，而是给现有 agent 补了一层非常实用的终端输出优化层。
- README 对支持命令、hook 方式和多宿主集成都写得很具体，落地门槛低。
- 对 `awesome-cli-for-ai` 来说，这类“CLI proxy + context compression”是很有代表性的基础设施型工具。

## 类似项目

- [OpenCLI](opencli.md) - 更偏统一网站、应用和本地命令的自动化中枢，而 `rtk` 更专注命令输出压缩和 token 节流。
- [Mosh](mosh.md) - 同样改善终端体验，但 `Mosh` 解决的是弱网远程交互，`rtk` 解决的是模型上下文浪费。

## 官方链接

- **官网:** https://www.rtk-ai.app
- **GitHub:** https://github.com/rtk-ai/rtk
- **架构文档:** https://github.com/rtk-ai/rtk/blob/master/docs/contributing/ARCHITECTURE.md
- **更新记录:** https://github.com/rtk-ai/rtk/releases

## 标签

- `CLI`, `Token Optimization`, `Claude Code`, `Cursor`, `Gemini CLI`

## 更新观察点

- 后续重点看支持的宿主、hook 机制和命令覆盖范围是否继续扩大。
- 持续关注 `rtk gain`、`discover` 这类统计能力会不会进一步演化成团队级上下文治理工具。
- 优先重抓 README、CHANGELOG 和 releases，确认各 AI CLI 的接入方式是否有变化。
