---
title: "bird"
slug: "bird"
info_type: "awesome-cli-for-ai"
entity_type: "tool"
category: "CLI Tools"
featured: false
last_reviewed_at: "2026-04-11T00:00:00+00:00"
---

# bird

## 一句话总结

一个面向 X / Twitter 的命令行工具，可在终端里发帖、回复、读取推文、搜索和查看线程，并适合脚本或 agent 调用。

## 它解决什么问题

- 社交平台操作通常被困在网页或 App 里，不利于脚本化
- agent 想读取或发布推文时，需要一个更轻量的命令行入口
- 终端自动化场景往往既想读内容，也想做轻量交互和发布

## 适合谁

- 想在终端里操作 X / Twitter 的高级用户
- 希望让 agent 具备基础社交平台读写能力的开发者
- 需要把社交平台动作接进脚本的人

## 核心能力

- 推文操作：支持 tweet、reply、read、replies、thread、search 等命令
- 凭证来源灵活：支持 CLI 参数、环境变量、Firefox / Chrome cookies 等认证路径
- 双引擎模式：可走 GraphQL cookies，也可走 Sweetistics API
- 配置文件支持：可为全局或项目定义持续生效的默认行为

## 典型使用场景

- 让 agent 在终端中读取某条推文、线程或搜索结果
- 用脚本自动发布状态、回复和查 mentions
- 在本地快速检查当前账号身份与可用凭证来源

## 为什么值得关注

- 它直接把社交平台入口做成了终端原语
- 对 agent workflow 来说，读写社交平台是很实用但不常见的能力层
- 它在 cookies、本地浏览器和 API 之间做了相对明确的接入设计

## 类似项目

- [imsg](imsg.md) - 同样把消息 / 社交通道带进终端，但对象是 Apple Messages
- [Agent Reach](agent-reach.md) - 更偏多平台内容读取与聚合，而不是直接做平台写操作

## 官方链接

- **GitHub:** https://github.com/jawond/bird
- **更新记录:** https://github.com/jawond/bird/releases

## 标签

- `X`, `Twitter`, `CLI`, `Social`, `Agent`

## 更新观察点

- 后续重点观察认证方式、引擎选择和媒体上传能力怎么演进
- 优先重新抓取 README、CHANGELOG 和 releases
- 如果后续补齐更多平台动作或更稳定的 API / cookies 兼容策略，值得补进正文
