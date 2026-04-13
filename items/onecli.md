---
title: "OneCLI"
entity_type: "tool"
category: "MCP / Tooling"
last_reviewed_at: "2026-04-14"
---

# OneCLI

## 一句话总结

一个给 AI agents 统一管理和注入 API 密钥的开源凭据网关，让 agents 用占位符调用服务而不直接接触真实 secrets。

## 快速判断

- 如果你在搭 agent 工具栈，想减少 secrets 暴露面，它值得优先看
- 如果你的 agent 只调用很少量本地工具，不一定需要单独引入凭据网关
- 它更像 agent security gateway，而不是普通密码管理器

## 你会怎么用它

- 接进 AI 工作流：让 agents 通过网关访问外部 API，而不是把真实 key 塞进每个 agent
- 接进日常运维：统一管理 agent token、secret scope 和 host/path 注入规则
- 最小落地方式：先接一个最关键的外部 API，验证 placeholder key 到 real key 的替换链路

## 它解决什么问题

- 给每个 agent 直接发 API key 风险很高
- 多个 agent 访问多个外部服务时，凭据管理容易失控
- secret rotation、访问范围和注入审计需要统一入口

## 适合谁

- 为 AI agents 管理 API 凭据的开发者
- 想减少 secrets 暴露面的 agent 平台团队
- 需要统一 credential injection 与访问控制的基础设施团队

## 核心能力

- 透明注入：agent 用占位符调用，网关在请求时替换真实凭据
- 加密存储：secret 以加密形式存储，仅在请求时解密
- 多 agent 隔离：每个 agent 可有单独 token 和权限范围
- 网关化管理：把 secrets 管理从 agent 本体里抽出来

## 能力边界

- 明显可用：多 agent、多 API 的 secrets 管理与注入
- 效果一般：只跑少量本地工具、不接外部 API 的场景
- 不要误用：它不是全能企业 IAM，也不是只靠 CLI 就完事的轻量脚本

## 集成方式

- 作为单独工具：本地或自托管运行 gateway + dashboard
- 作为 AI 工作流组件：放在 agent 外部 API 调用层，承接 secret injection
- 作为团队流程节点：统一 agent secrets、rotation 和最小权限策略

## 上手建议

- 第一步先只接一个外部服务，确认链路和调试方式
- 最值得先试的是“多个 agent 共用同类 API”的场景
- 如果团队刚开始做 agent 安全治理，先小范围替换最敏感的 key

## 选型建议

- 如果你的主需求是“给 agents 增加安全的 secret gateway”，适合看它
- 如果你的主需求只是“本地存几把 key”，更轻的方案可能足够
- 如果你关心 agent 不直接见到真实凭据，这条很关键

## 为什么值得关注

- AI agents 的 secrets 暴露是非常真实的问题，它正面解决这件事
- 相比把凭据散在各 agent 配置里，网关式设计更易治理
- 很适合作为 agent tooling 栈中的安全层

## 官方链接

- **官网:** https://onecli.sh
- **GitHub:** https://github.com/onecli/onecli

## 标签

- `Secrets`, `Gateway`, `Agent Infrastructure`, `CLI`, `Security`
