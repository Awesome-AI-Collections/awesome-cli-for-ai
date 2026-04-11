---
title: "ncm-cli"
slug: "ncm-cli"
info_type: "awesome-cli-for-ai"
entity_type: "tool"
category: "CLI Tools"
featured: false
last_reviewed_at: "2026-04-11T00:00:00+00:00"
---

# ncm-cli

## 一句话总结

一个面向网易云音乐的命令行客户端，支持搜索、播放、歌单管理和 TUI 播放器，并可接入 AI agent。

## 它解决什么问题

- 音乐搜索、播放和歌单管理通常被限制在 App 或网页里，不利于终端自动化
- 想让 Claude Code、OpenClaw 等 agent 自然语言控制音乐时，需要正式命令入口
- 终端用户既想要日常播放控制，也想要全屏 TUI 播放体验

## 适合谁

- 想在终端里操作网易云音乐的用户
- 希望让 AI agent 具备音乐搜索与播放能力的开发者
- 喜欢 TUI 播放器和脚本化音乐控制的人

## 核心能力

- 音乐操作：支持搜索、播放、暂停、切歌、音量和播放状态查询
- 歌单与推荐：支持歌单管理与每日推荐相关能力
- TUI 播放器：提供旋转黑胶、歌词同步和场景切换等终端体验
- Agent 集成：官方 npm 包页直接提供 Claude Code 与 OpenClaw 的 skills 接入方式

## 典型使用场景

- 在终端中搜索歌曲、播放音乐和管理歌单
- 用自然语言让 Claude Code 或 OpenClaw 帮你控制播放
- 在本地用 `mpv` 作为后端运行全屏 TUI 播放器

## 为什么值得关注

- 它不是普通播放器 CLI，而是明确面向 agent 集成设计
- npm 包页已经把配置、二维码登录和 skills 安装路径写得比较完整
- 在中文场景里，这是很有代表性的“消费级服务 + AI CLI”组合

## 类似项目

- [imsg](imsg.md) - 同样把个人消费类应用入口带进终端，但对象是消息通信
- [bird](bird.md) - 同样把平台操作做成 CLI，但对象是社交平台而不是音乐服务

## 官方链接

- **官网:** https://music.163.com/
- **npm:** https://www.npmjs.com/package/@music163/ncm-cli
- **GitHub / Skills:** https://github.com/NetEase/skills

## 标签

- `Music`, `CLI`, `TUI`, `Agent`, `NetEase Music`

## 更新观察点

- 后续重点看命令面、TUI 播放器和 agent skills 能力是否继续扩展
- 优先重新抓取 npm 包页和 NetEase Skills 仓库
- 如果后续出现独立源码仓库或更完整的官方文档，值得补进正文
