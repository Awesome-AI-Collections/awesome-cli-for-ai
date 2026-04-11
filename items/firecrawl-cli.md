---
title: "Firecrawl CLI"
slug: "firecrawl-cli"
info_type: "awesome-cli-for-ai"
entity_type: "tool"
category: "MCP / Tooling"
featured: false
last_reviewed_at: "2026-04-11T00:00:00+00:00"
---

# Firecrawl CLI

## 一句话总结

Firecrawl 的命令行接口，可在终端里完成 scrape、crawl、search，并为 AI coding agents 安装 skills 与 MCP。

## 它解决什么问题

- 网页抓取、搜索和结构化提取通常要在多个工具之间切换
- Agent 想直接用 Firecrawl 能力时，还需要额外处理 skills 和 MCP 安装
- 团队希望把网页数据获取能力变成终端里可复用的统一命令

## 适合谁

- 需要在终端里抓网站、搜网页并输出 LLM-ready 数据的开发者
- 想给 Claude Code、Cursor 等 Agent 快速装上 Firecrawl 能力的人
- 需要把网页提取能力接入脚本和自动化链路的团队

## 核心能力

- 抓取与搜索：在终端里直接 scrape、crawl、search 网站内容
- 多格式输出：支持 markdown、HTML、links、images、summary 等输出
- 技能安装：可为主流 coding agents 安装 Firecrawl skill
- MCP 接入：能把 Firecrawl MCP server 配进编辑器和 agent 工具链

## 典型使用场景

- 在终端里快速抓网页并输出给 LLM 或 RAG 流程
- 给本地 AI agent 一键加上网页搜索与抓取能力
- 把网页提取、搜索和 MCP 安装串成自动化 setup 流程

## 为什么值得关注

- 它不是单纯的抓取 CLI，还主动面向 AI coding agent 场景设计
- Skill 和 MCP 安装入口让它比普通网页抓取 CLI 更贴近 agent 工作流
- 对 `awesome-cli-for-ai` 来说，它是很典型的“CLI + agent tooling”项目

## 类似项目

- [bb-browser](bb-browser.md) - 更强调复用真实浏览器与登录态，而不是 Firecrawl 云抓取能力
- [Agent Reach](agent-reach.md) - 更强调给 Agent 补整套联网能力，而不是围绕 Firecrawl 能力层展开

## 官方链接

- **GitHub:** https://github.com/firecrawl/cli
- **更新记录:** https://github.com/firecrawl/cli/releases

## 标签

- `Firecrawl`, `CLI`, `MCP`, `Skill`, `网页抓取`

## 更新观察点

- 后续重点观察它的 scrape/search/crawl 子命令和输出格式演进
- 优先重新抓取 README 和 releases，跟踪 skill 与 MCP setup 的变化
- 如果后续补了更多非交互式和团队级安装方式，值得补进正文
