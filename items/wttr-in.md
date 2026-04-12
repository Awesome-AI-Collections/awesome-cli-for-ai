---
title: "wttr.in"
entity_type: "tool"
category: "CLI Tools"
last_reviewed_at: "2026-04-11"
---

# wttr.in

## 一句话总结

一个面向终端和脚本的天气服务，可通过 `curl` 等命令直接返回 ANSI、纯文本、JSON、PNG 和指标格式天气信息。

## 它解决什么问题

- 在终端里查看天气时，很多方案要么太重，要么不适合脚本调用
- 状态栏、监控面板和自动化脚本需要一个轻量天气接口
- 同时想兼顾人类终端输出和程序消费格式时，普通网页不够顺手

## 适合谁

- 想在 shell 里快速看天气的人
- 需要把天气信息接进脚本、状态栏和自动化任务的用户
- 希望用简单 HTTP 请求拿到天气文本、JSON 或图片的人

## 核心能力

- curl 友好：直接通过 URL 获取当前位置或指定地点天气
- 多格式输出：支持 ANSI、纯文本、HTML、PNG、JSON 和 Prometheus 指标
- 灵活地点查询：支持城市、机场代码、特殊地点、IP 和域名查询
- 状态栏友好：支持单行输出与自定义 format 参数

## 典型使用场景

- 在终端里快速查看当前或某地天气
- 给 tmux、weechat、状态栏和监控面板提供轻量天气信息
- 在脚本中拉取 JSON 或指标格式天气数据

## 为什么值得关注

- 它把天气服务做成了极简但极顺手的命令行入口
- 对终端用户来说，`curl wttr.in` 已经是经典体验之一
- 同一套服务同时照顾了人类阅读和程序消费两类需求

## 类似项目

- [aria2](aria2.md) - 同样是经典终端工具，但解决的是下载而不是信息查询
- [rclone](rclone.md) - 同样服务于脚本和自动化场景，但面向存储同步与数据流转

## 官方链接

- **官网:** https://wttr.in/
- **GitHub:** https://github.com/chubin/wttr.in
- **更新记录:** https://github.com/chubin/wttr.in/releases

## 标签

- `Weather`, `CLI`, `curl`, `JSON`, `Terminal`

## 更新观察点

- 后续重点观察输出格式、查询参数和服务稳定性说明
- 优先重新抓取 README、在线帮助页和 releases
- 如果后续新增更适合监控或自动化系统的接口格式，值得补进正文
