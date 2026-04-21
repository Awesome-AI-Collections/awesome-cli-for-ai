---
title: "Browser Harness"
entity_type: "tool"
category: "Agent Shells"
last_reviewed_at: "2026-04-21"
---

# Browser Harness

## 一句话总结

一个直接连 Chrome CDP 的自愈式浏览器 harness，允许 Claude Code / Codex 在任务中动态补 helper，适合真实浏览器网页任务。

## 它解决什么问题

- 很多浏览器自动化工具要么太底层，要么把 agent 能做的事情预先写死，不够贴近“让模型自己补缺口”的工作方式
- AI agent 在真实网页登录态和真实浏览器上下文里做任务时，常常缺少足够薄、足够直接的执行层
- 团队想让 Claude Code / Codex 在网页任务中边做边改工具时，不想再套一层厚框架

## 适合谁

- 想让 Claude Code、Codex 直接操控真实浏览器的开发者
- 需要浏览器任务执行面但不想引入厚重 agent framework 的工程团队
- 想把网页交互能力做成 agent shell 一部分的人

## 核心能力

- 直接连 CDP：核心路径是一条 websocket 直连 Chrome，执行面很薄
- 自愈 helper：agent 可以在任务中直接修改 `helpers.py`，把缺失动作补出来
- 真实浏览器接入：优先连接用户自己的真实浏览器，而不是只跑隔离脚本环境
- Claude Code / Codex 友好：README 直接给了面向这些 agent 的 setup prompt

## 典型使用场景

- 让编码 agent 在真实网页登录态里完成表单、上传文件和页面操作
- 给本地 agent 工作流补一个可迭代的浏览器执行层
- 把浏览器技能沉淀成 domain skills，逐步减少重复摸索

## 为什么值得关注

- 它的差异化不在“会不会点页面”，而在“允许 agent 在做任务时把缺的工具现场补出来”
- README 明确强调 no framework / no rails，更接近一个极薄的 agent browser harness
- 和 browser-use 主仓形成互补：这里更像执行面和技能沉淀层，而不是完整产品栈

## 类似项目

- [agent-browser](agent-browser.md) - 更像完整的浏览器自动化 CLI 命令层，而 Browser Harness 更强调让 agent 动态扩展 helper
- [browser-use](browser-use.md) - 更偏完整 agent 框架 + CLI + cloud runtime，而 Browser Harness 更聚焦真实浏览器执行面

## 官方链接

- **官网:** https://browser-use.com/
- **GitHub:** https://github.com/browser-use/browser-harness
- **更新记录:** https://github.com/browser-use/browser-harness/releases

## 标签

- `Browser Automation`, `CDP`, `Agent`, `Claude Code`, `Codex`

## 更新观察点

- 后续重点观察 `helpers.py`、`domain-skills/` 和安装流程如何演进
- 持续跟踪 README、`install.md`、`SKILL.md` 和 releases
- 如果后续补了更明确的多浏览器或远程运行模型，值得继续更新条目
