---
title: "Agent Payment Node"
entity_type: "tool"
category: "MCP / Tooling"
last_reviewed_at: "2026-10-26"
---

# Agent Payment Node

## 一句话总结

Nuanu AI 的开源本地支付运行时，通过 CLI 与 stdio MCP 为 AI agent 提供 x402 报价检查、受限支付准备、操作状态和回执查询。

## 适合谁

- 需要在终端 agent 工作流中接入 x402 买方支付能力的开发者。
- 能自行管理本地钱包、支付策略与明确授权范围的使用者。

## 核心能力

- 检查支持的 x402 报价，并按所有者配置的策略准备受限支付操作。
- 查询操作状态、回执以及文档描述的恢复路径。
- 通过本地 CLI 或 stdio MCP 接入工具链；它不是 LLM 聊天前端或托管 MCP 服务。

## 安装与配置

仅支持 Apple Silicon macOS 与 Node 24；不应按 Linux、Windows 或 Intel Mac 工具安装。

```bash
brew install nuanu-ai/tap/apn
apn mcp config
apn mcp serve
```

`apn mcp config` 输出实际启动描述符，`apn mcp serve` 是本地 stdio 启动命令。不要替换为不存在的 npm 包、Docker 镜像或远程 endpoint。

## 能力与授权边界

APN 能触发支付，不是只读工具或通用沙箱。直接转账与 EVM x402 签名需要所有者在前台批准；Solana exact x402 只能在所有者已接纳的策略范围内运行。

本地软件钱包的保管、受损主机与恢复限制仍适用。不要把私钥、助记词或 provider 凭据放进提示词或公开配置。软件免费，但网络与 provider 费用另计。

这条目不声称通过独立安全审计、真实资金支付测试或具体客户端的端到端兼容性复测。

## 官方链接

- **项目与文档:** https://github.com/nuanu-ai/agent-payment-node
- **发布记录:** https://github.com/nuanu-ai/agent-payment-node/releases

## 标签

- `CLI`, `MCP`, `x402`, `支付`, `macOS`, `TypeScript`

## 更新观察点

- 关注平台支持、支付授权边界和 CLI/MCP 配置方式的实际变化。
- 以官方 README 与发布记录为准，不据工具发现结果推断支付或安全审计结论。
