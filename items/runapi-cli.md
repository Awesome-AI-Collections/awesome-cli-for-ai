---
title: "RunAPI CLI"
entity_type: "tool"
category: "CLI Tools"
last_reviewed_at: "2026-06-25"
---

# RunAPI CLI

## 一句话总结

一个用 JSON-first 命令运行 AI 图片、视频、音乐、语音和 LLM 任务的统一模型 CLI，适合脚本、CI 和 AI agent 调用。

## 它解决什么问题

- 多模态模型任务分散在不同 provider、SDK 和网页里，不利于终端自动化
- agent 需要稳定的命令行入口来创建任务、轮询结果和读取结构化输出
- 开发者想把图片、视频、音乐、语音和 LLM 生成流程接进脚本或 CI

## 适合谁

- 需要在终端里跑多模态模型任务的开发者
- 想给 Claude Code、Codex、OpenClaw 等 agent 提供模型执行入口的人
- 正在把生成式内容、批处理任务或模型 API 调用接进自动化流水线的团队

## 核心能力

- 统一模型入口：覆盖图片、视频、音乐、语音和 LLM 等任务类型
- JSON-first：输出适合脚本、CI 和 agent runtime 继续处理
- 多安装方式：支持 install script、Homebrew 和 Go install
- 面向自动化：适合任务创建、状态查询和结果消费这类命令式流程

## 典型使用场景

- 在终端里批量生成图片、短视频或音乐素材
- 让 agent 用一个 CLI 发起模型任务并读取结构化结果
- 把模型 API jobs 接进 CI、脚本或内部工具链

## 为什么值得关注

- 它把多模态模型执行收敛到一个终端入口
- 对 agent 工作流来说，JSON-first CLI 比网页操作更容易稳定复用
- 它适合放在“AI CLI 工具”和“终端模型任务执行”这一类场景里

## 类似项目

- [Dreamina CLI](dreamina-cli.md) - 更聚焦单一创作平台的图片 / 视频生成
- [jina-cli](jina-cli.md) - 更聚焦网页读取和搜索，而不是模型任务执行

## 官方链接

- **GitHub:** https://github.com/runapi-ai/cli
- **文档:** https://runapi.ai/docs#runapi-cli

## 标签

- `AI Models`, `Image Generation`, `Video Generation`, `Music Generation`, `LLM`, `CLI`, `Agent`

## 更新观察点

- 后续重点观察新增模型类型、任务命令和输出格式
- 优先持续观察 README、docs 和 releases
