---
title: "GitHub CLI"
slug: "github-cli"
info_type: "awesome-cli-for-ai"
entity_type: "tool"
category: "CLI Tools"
featured: false
last_reviewed_at: "2026-04-11T00:00:00+00:00"
---

# GitHub CLI

## 一句话总结

GitHub 官方命令行工具 `gh`，把 PR、Issue、Actions、Codespaces 和仓库协作能力直接带进终端。

## 它解决什么问题

- 开发者在终端里工作时，经常还要频繁切回浏览器处理 GitHub 协作动作
- GitHub 上的 PR、Issue、Release、Workflow 操作分散，脚本化成本高
- AI Agent 想参与 GitHub 协作时，需要一个稳定、官方、可脚本化的命令入口

## 适合谁

- 日常在终端里管理 GitHub 工作流的开发者
- 想把 PR、Issue 和 Actions 接进自动化脚本的团队
- 需要让 AI Agent 调用官方 GitHub CLI 能力的人

## 核心能力

- 仓库协作：处理 PR、Issue、Review 和 Release 等常见 GitHub 操作
- 官方命令层：覆盖 GitHub 核心概念，适合长期脚本化
- 多平台支持：适用于 macOS、Windows、Linux 以及 GitHub Enterprise 场景
- 自动化友好：非常适合 shell 脚本、CI 和本地 Agent 工作流

## 典型使用场景

- 在终端里发起和检查 PR、Issue、Release
- 让本地脚本或 Agent 自动读取和更新 GitHub 协作状态
- 在 CI、Codespaces 或开发容器里统一使用 GitHub 官方命令接口

## 为什么值得关注

- 它是 GitHub 官方维护的 CLI，稳定性和长期可用性更强
- 对终端工作流来说，`gh` 基本属于基础设施级工具
- 很多更上层的 AI CLI 工作流，最终都会把 GitHub CLI 当底座

## 类似项目

- [Vercel CLI](vercel-cli.md) - 同样是官方平台 CLI，但侧重点是部署和环境管理
- [wecom-cli](wecom-cli.md) - 同样把平台能力带进终端，但面向的是企业微信操作

## 官方链接

- **官网:** https://cli.github.com/manual/
- **GitHub:** https://github.com/cli/cli
- **更新记录:** https://github.com/cli/cli/releases

## 标签

- `GitHub`, `CLI`, `终端`, `协作`, `自动化`

## 更新观察点

- 后续重点观察 `gh` 新增了哪些 GitHub 原生概念和子命令
- 优先重新抓取 README、manual 和 releases
- 如果后续增强对 agent 场景更友好的非交互式能力，值得补进正文
