---
title: "Google Workspace CLI"
entity_type: "tool"
category: "CLI Tools"
last_reviewed_at: "2026-04-11"
---

# Google Workspace CLI

## 一句话总结

一个覆盖 Drive、Gmail、Calendar、Sheets、Docs、Chat 等 Google Workspace 能力的统一命令行工具，并内置 AI agent skills。

## 它解决什么问题

- Google Workspace 各产品 API 分散，终端自动化和脚本接入成本高
- AI agent 想直接操作 Gmail、Drive、Calendar 等服务时，缺少统一命令面
- 团队需要结构化 JSON 输出和可复用技能层，而不是反复拼接原始 REST 调用

## 适合谁

- 想在终端里统一操作 Google Workspace 的开发者
- 需要把 Workspace 接进 AI agent 工作流的团队
- 希望用官方 discovery 驱动命令生成而不是手写 API 封装的人

## 核心能力

- Workspace 一体化：覆盖 Drive、Gmail、Calendar、Sheets、Docs、Chat 等核心服务
- 动态命令面：基于 Google Discovery Service 在运行时构建命令接口
- Agent Skills：自带大量面向 AI agent 的技能文件
- 结构化输出：强调 JSON 输出，方便脚本和模型消费

## 典型使用场景

- 在终端里列文件、发邮件、建日历事件、查聊天消息
- 让 AI agent 统一调用 Google Workspace 能力
- 在自动化流程里用一个 CLI 代替多套零散 API 封装

## 为什么值得关注

- 它把“大量 Workspace API”压成了一个统一终端入口
- 对 agent 场景来说，动态生成命令面和内置 skills 很有吸引力
- 是典型的“平台 API -> AI CLI”路线项目

## 类似项目

- [Lark CLI](lark-cli.md) - 同样是大型协作平台 CLI，但面向飞书 / Lark 生态
- [wecom-cli](wecom-cli.md) - 同样把协作平台能力带进终端，但聚焦企业微信开放平台

## 官方链接

- **GitHub:** https://github.com/googleworkspace/cli
- **更新记录:** https://github.com/googleworkspace/cli/releases

## 标签

- `Google Workspace`, `CLI`, `Agent Skills`, `自动化`, `JSON`

## 更新观察点

- 后续重点看支持的 Workspace 服务范围和命令生成机制是否继续扩展
- 持续跟踪 README、AGENTS、CHANGELOG 和 releases
- 如果后续增强认证与 team setup 体验，值得补进正文
