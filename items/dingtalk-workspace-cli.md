---
title: "DingTalk Workspace CLI"
entity_type: "tool"
category: "CLI Tools"
last_reviewed_at: "2026-04-14"
---

# DingTalk Workspace CLI

## 一句话总结

钉钉官方的企业工作台 CLI，可让人类和 AI agents 以结构化方式访问企业数据、自动化工作流并保持审计边界。

## 快速判断

- 如果你想把钉钉企业工作台能力接进终端和 agents，它值得看
- 如果你不在钉钉企业生态里，它的价值会明显下降
- 它更像企业工作台 CLI，而不是泛聊天或泛业务自动化工具

## 你会怎么用它

- 接进 AI 工作流：让 agents 通过 JSON、skills 和命令式调用访问钉钉工作台能力
- 接进日常终端流：用 `dws` 做认证、查询、升级、dry-run 和组织级操作
- 最小落地方式：先完成授权和登录，再跑一条最简单的只读命令验证权限链路

## 它解决什么问题

- 企业工作台数据对 agents 不够友好，缺少稳定 CLI 接入层
- 企业级自动化需要明确的鉴权、审计和最小权限控制
- 人类与 agents 共用同一接口时，需要一个清晰、结构化的命令面

## 适合谁

- 需要在终端里操作 DingTalk Workspace 的用户
- 想把钉钉企业数据接入 agents 的组织与团队
- 重视企业审计和权限边界的 CLI 用户

## 核心能力

- 官方 CLI：直接面向 DingTalk Workspace 能力
- Agent 友好：JSON 输出、skills、dry-run 和结构化命令设计
- 安全设计：OAuth、allowlisting、least privilege 和审计边界明确
- 自升级能力：内置升级、回滚、版本校验和 skill 分发

## 能力边界

- 明显可用：DingTalk Workspace 的 terminal-first 自动化
- 效果一般：不在钉钉生态或只想做泛企业自动化的场景
- 不要误用：它不是 coding agent，也不是通用办公平台

## 集成方式

- 作为单独工具：直接用 `dws` 管理和调用工作台能力
- 作为 AI 工作流组件：放在企业数据 CLI 接入层，给 agents 提供结构化入口
- 作为团队流程节点：适合企业内部审批、查询和工作台自动化

## 上手建议

- 第一步先完成组织授权与 CLI access 开启
- 最值得先试的是只读查询与 `--dry-run`
- 如果组织权限很复杂，先从最小范围试点，不要一开始就放大权限

## 选型建议

- 如果你的主需求是“钉钉工作台 CLI + agent 接入”，适合看它
- 如果你的主需求只是“找一个 AI CLI”，它不是这类项目
- 如果你处在钉钉企业生态里，它会比通用工具更直接

## 为什么值得关注

- 它是少见把企业工作台能力真正做成 agent-friendly CLI 的项目
- 官方背景和安全设计让它更适合企业环境
- 对 terminal-first enterprise automation 很有代表性

## 官方链接

- **GitHub:** https://github.com/DingTalk-Real-AI/dingtalk-workspace-cli
- **更新记录:** https://github.com/DingTalk-Real-AI/dingtalk-workspace-cli/releases

## 标签

- `DingTalk`, `Enterprise`, `CLI`, `Operations`, `Agents`
