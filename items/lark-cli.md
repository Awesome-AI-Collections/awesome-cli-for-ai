---
title: "Lark CLI"
entity_type: "tool"
category: "CLI Tools"
last_reviewed_at: "2026-04-11"
---

# Lark CLI

## 一句话总结

飞书 / Lark 官方 CLI，覆盖消息、文档、Base、Sheets、Calendar、Mail、Tasks、Meetings 等能力，并面向 humans 与 AI Agents 设计。

## 它解决什么问题

- 飞书开放平台能力很多，但对终端自动化和 agent 来说入口过于分散
- 团队想在 shell 里处理消息、文档、日历、审批和会议时，缺少统一命令层
- AI agent 场景需要更友好的参数、默认值和结构化输出，而不是直接撞原始 API

## 适合谁

- 想在终端里操作飞书 / Lark 的开发者
- 需要把飞书接进 AI agent 工作流的团队
- 希望统一处理消息、Docs、Base、Calendar、Mail 等业务域的人

## 核心能力

- 广覆盖：覆盖 12 个业务域、200+ 命令和 20 个 AI Agent Skills
- Agent-Native：README 明确强调 humans 与 AI Agents 双端使用
- 三层命令系统：Shortcut、API Commands、Raw API 分层清晰
- 安全与易用性：强调交互登录、智能默认值和结构化输出

## 典型使用场景

- 在终端里收发消息、查日程、读写 Docs/Base/Sheets
- 让 AI agent 通过 skills 和 shortcut 快速操作飞书
- 把飞书协作流程接进内部自动化和运维脚本

## 为什么值得关注

- 它是平台方维护的官方 CLI，而不是第三方薄封装
- 明确为 AI Agents 做了技能、参数设计和输出优化
- 对中文团队来说，这是非常强的本土协作平台 CLI 入口

## 类似项目

- [Google Workspace CLI](google-workspace-cli.md) - 同样是大型协作套件 CLI，但面向 Google Workspace
- [wecom-cli](wecom-cli.md) - 同样面向企业协作平台，不过更偏企业微信开放平台

## 官方链接

- **GitHub:** https://github.com/larksuite/cli
- **更新记录:** https://github.com/larksuite/cli/releases

## 标签

- `Lark`, `Feishu`, `CLI`, `Agent Skills`, `协作平台`

## 更新观察点

- 后续重点观察业务域覆盖和 Skills 数量是否继续增长
- 持续跟踪 README、AGENTS、releases 和安全说明
- 如果后续开放更多团队级部署或非交互式认证方式，值得补进正文
