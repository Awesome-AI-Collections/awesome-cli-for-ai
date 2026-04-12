---
title: "notebooklm-py"
entity_type: "tool"
category: "Workflow Automation"
last_reviewed_at: "2026-04-11"
---

# notebooklm-py

## 一句话总结

一个非官方的 NotebookLM Python API 与 CLI，能把 NotebookLM 的笔记本、资料导入、问答、研究和内容生成能力接进终端、脚本与 agent。

## 它解决什么问题

- 官方网页界面不适合批量、自动化和程序化调用
- 团队想把 NotebookLM 接进脚本、agent 或研究流水线时，缺少命令行入口
- 一些导出、批量下载和结构化输出能力在网页端并不直观或并未暴露

## 适合谁

- 想在终端里驱动 NotebookLM 的高级用户
- 需要把研究、内容生成和资料整理做成自动化流程的团队
- 希望让 Claude Code、Codex 等 agent 使用 NotebookLM 能力的人

## 核心能力

- CLI + API 双入口：既支持 shell 命令，也支持 Python 集成
- NotebookLM 全流程调用：覆盖 notebook、sources、chat、research、sharing 等操作
- 产物生成与导出：支持音频、视频、quiz、flashcards、slide deck、mind map 等生成与下载
- Agent 集成：提供面向 Claude Code、Codex 等 agent 的技能和集成说明

## 典型使用场景

- 在终端中批量导入 URL、PDF、YouTube 或 Google Drive 资料
- 用脚本自动生成 Audio Overview、Quiz、Flashcards 或报告
- 把 NotebookLM 能力接给本地 AI agent 作为研究和资料整理后端

## 为什么值得关注

- 它把 NotebookLM 从“网页工具”扩展成了可编排的终端能力
- CLI、Python API 和 agent integration 三条路径一起提供，实用性很强
- 它还覆盖了一些网页端不直接暴露的导出与程序化能力

## 类似项目

- [Obsidian CLI](obsidian-cli.md) - 同样把知识库系统带进终端，但 Obsidian CLI 更偏本地文本知识库与自动化
- [OpenCLI](opencli.md) - 同样强调把多种应用能力暴露给终端与 agent，但不是 NotebookLM 专用入口

## 官方链接

- **GitHub:** https://github.com/teng-lin/notebooklm-py
- **更新记录:** https://github.com/teng-lin/notebooklm-py/releases

## 标签

- `NotebookLM`, `CLI`, `Python`, `Agent`, `Research`

## 更新观察点

- 后续重点看 undocumented API 的稳定性和与网页端能力的差距
- 优先重新抓取 README、CHANGELOG、AGENTS、CLAUDE 和 releases
- 如果后续对官方能力变化的兼容策略更成熟，值得补进正文
