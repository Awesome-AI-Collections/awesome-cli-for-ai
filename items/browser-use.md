---
title: "browser-use"
entity_type: "tool"
category: "Agent Shells"
last_reviewed_at: "2026-04-11"
---

# browser-use

## 一句话总结

一个面向 AI agents 的浏览器自动化项目，既提供 Python agent 框架，也提供持久化浏览器 CLI 与 cloud runtime。

## 它解决什么问题

- 许多浏览器自动化库更偏底层脚本，不够贴近 agent 工作流
- 团队想同时要本地开源框架、CLI 和可扩展的 cloud runtime 时，通常得自己拼栈
- AI agent 做网页任务时，既需要浏览器操作层，也需要更高层的 agent 能力和模板

## 适合谁

- 想给 AI agent 配一套更完整浏览器执行栈的开发者
- 需要浏览器 CLI、开源框架和云端运行时组合方案的团队
- 想把网页自动化扩展成 agent 产品或基础设施的人

## 核心能力

- Agent 框架：提供面向网页任务的 browser agent 抽象
- 持久化 CLI：支持在终端里保持浏览器进程并逐步执行命令
- Cloud 运行时：提供更偏产品化的浏览器云能力
- 模板与技能：支持 quickstart、templates 和 Claude Code skill

## 典型使用场景

- 用 CLI 快速做浏览器状态查看、点击、输入和截图
- 用 Python agent 框架构建更复杂的网页任务自动化
- 在需要规模化浏览器自动化时，转向 cloud runtime

## 为什么值得关注

- 它不是单纯 CLI，也不是单纯库，而是在做完整的 agent 浏览器产品栈
- 官方站点和 GitHub 同时强调 open source + cloud 的组合路线
- 对 CLI repo 来说，它很适合作为“agent shell + browser runtime”代表项目

## 类似项目

- [agent-browser](agent-browser.md) - 更纯粹地强调浏览器自动化 CLI 命令层
- [bb-browser](bb-browser.md) - 更强调真实浏览器与登录态复用，而不是完整 agent/cloud 栈

## 官方链接

- **官网:** https://browser-use.com/
- **GitHub:** https://github.com/browser-use/browser-use
- **更新记录:** https://github.com/browser-use/browser-use/releases

## 标签

- `Browser Automation`, `CLI`, `Agent`, `Cloud`, `Python`

## 更新观察点

- 后续重点观察开源 agent、CLI 和 cloud 功能边界如何演进
- 持续跟踪官网、README、AGENTS 和 releases
- 如果后续把 CLI 和 cloud 的协作模型做得更清晰，值得补进正文
