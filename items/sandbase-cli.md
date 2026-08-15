---
title: "SandBase CLI"
entity_type: "tool"
category: "MCP / Tooling"
last_reviewed_at: "2026-08-15"
---

# SandBase CLI

## 一句话总结

一个面向 AI 编程 Agent 的开源 CLI 和 MCP bridge，用一个账号把主流客户端接入 2,000+ AI 模型与多类工具。

## 它解决什么问题

- AI Agent 要访问搜索、社交媒体、网页数据、生成式模型和沙箱时，通常要逐个申请与维护 API key
- Cursor、Claude Code、Codex、Windsurf 等客户端的 MCP 配置位置和格式各不相同
- 团队需要在不把长期密钥直接写进客户端配置的前提下，统一接入外部能力

## 适合谁

- 希望快速给 coding agent 增加联网、数据采集和多模态生成能力的开发者
- 同时使用多个 AI 编程客户端，希望统一配置入口的个人或团队
- 需要把模型调用、API 工具和云端沙箱接进 MCP 工作流的 Agent 工程团队

## 核心能力

- MCP 接入：为主流 AI 编程客户端配置本地 bridge，并把调用转发到 SandBase MCP endpoint
- 多类工具：覆盖网页搜索、社交媒体、网页抓取、图像、视频、音频、电商和金融数据
- 模型访问：通过同一平台调用 2,000+ AI 模型
- 客户端兼容：README 列出 17+ 支持的客户端，包含自动配置和手动配置路径
- 凭据管理：浏览器授权后将客户端凭据保存在本地受限权限文件中，不要求逐个配置供应商 API key

## 典型使用场景

- 让 Codex 或 Claude Code 搜索实时网页资料并把结果带回开发流程
- 在 Cursor 等客户端里调用图像、视频或音频生成工具制作产品素材
- 让 Agent 获取社交媒体与公开网页数据，完成调研、监测或内容分析
- 在云端沙箱中执行隔离任务，而不在本机直接运行不受信任代码

## 为什么值得关注

- 它不是单一 MCP server，而是把工具、模型和沙箱能力统一到一个 Agent 接入层
- CLI 会检测客户端并尽量自动完成 MCP 配置，同时提供 doctor 与 unregister 生命周期命令
- 项目使用 Apache-2.0 许可证，npm 包公开发布，仓库包含 MCP bridge 和客户端适配实现

## 类似项目

- [Agent Reach](agent-reach.md) - 更聚焦跨平台互联网内容读取与安装式工具集合
- [OneCLI](onecli.md) - 更聚焦给 Agent 统一管理与注入第三方 API 密钥
- [OpenCLI](opencli.md) - 更聚焦把网站、浏览器会话、Electron 应用和本地 CLI 暴露为自动化接口

## 官方链接

- **GitHub:** https://github.com/sandbaseai/cli
- **npm:** https://www.npmjs.com/package/@sandbaseai/cli
- **官网:** https://www.sandbase.ai

## 标签

- `MCP`, `CLI`, `Agent 工具`, `模型路由`, `多模态`, `云端沙箱`

## 更新观察点

- 关注新增客户端的自动配置与真实客户端验证状态
- 关注工具和模型目录的变化，以及权限范围是否继续细化
- 关注 MCP bridge 的认证、凭据撤销和诊断流程是否继续完善
