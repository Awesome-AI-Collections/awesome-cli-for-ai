---
title: "wecom-cli"
entity_type: "tool"
category: "CLI Tools"
last_reviewed_at: "2026-04-11"
---

# wecom-cli

## 一句话总结

企业微信开放平台命令行工具，让人类和 AI Agent 都能在终端中操作企业微信。

## 它解决什么问题

- 企业微信开放平台能力通常分散在 API 和后台界面里，终端调用门槛高
- AI Agent 想操作企业微信通讯录、消息、待办、会议和日程时，缺少统一 CLI 层
- 团队希望把企业微信自动化能力直接接进 shell、脚本和 Agent 工作流

## 适合谁

- 需要在终端里操作企业微信开放平台能力的开发者
- 想把企业微信接进 AI Agent 工作流的团队
- 有企业内协作自动化需求的运维、工具和效率团队

## 核心能力

- 平台能力覆盖：支持通讯录、待办、会议、消息、日程、文档和智能表格等能力
- CLI + Skill：除了命令行入口，还提供可给 Agent 安装的 skill
- 交互式初始化：适合先完成凭证配置，再进入批处理自动化
- 人机共用：同时面向人类终端操作和 AI Agent 调用场景

## 典型使用场景

- 在终端里自动处理企业微信消息、待办和会议协同
- 让 Agent 调用企业微信数据与操作接口
- 把企业微信自动化接进内部脚本和运营流程

## 为什么值得关注

- 它不是泛用聊天 CLI，而是企业微信开放平台的终端能力层
- README 直接把“让人类和 AI Agent 都能在终端中操作企业微信”写成目标
- 对中文团队来说，这类本土协作平台 CLI 非常有实际价值

## 类似项目

- [imsg](imsg.md) - 同样把消息能力接进终端，但面向的是 Apple Messages.app
- [GitHub CLI](github-cli.md) - 同样是平台官方 CLI，但围绕代码协作而不是企业协作平台

## 官方链接

- **GitHub:** https://github.com/WecomTeam/wecom-cli
- **更新记录:** https://github.com/WecomTeam/wecom-cli/releases

## 标签

- `CLI`, `企业微信`, `Agent`, `自动化`, `协作平台`

## 更新观察点

- 后续重点看它覆盖的企业微信能力边界是否继续扩展
- 优先重新抓取 README 和 releases，跟踪 skill 安装方式和认证要求变化
- 如果后续补了更清晰的权限模型和团队接入示例，值得补进正文
