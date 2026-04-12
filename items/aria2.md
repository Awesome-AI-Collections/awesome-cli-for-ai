---
title: "aria2"
entity_type: "tool"
category: "CLI Tools"
last_reviewed_at: "2026-04-11"
---

# aria2

## 一句话总结

一个经典的高速下载命令行工具，支持 HTTP(S)、FTP、SFTP、BitTorrent 和 Metalink，并能多源并行拉取文件。

## 它解决什么问题

- 默认下载工具在批量、断点续传和多源拉取场景里不够灵活
- 需要把下载任务接进脚本、守护进程或远程环境时，GUI 工具不方便
- 大文件、镜像和多协议资源经常需要更可控的命令行下载器

## 适合谁

- 经常在终端里下载大文件、数据集或发行包的人
- 需要把下载任务接进自动化脚本和服务端环境的工程团队
- 想用更轻量方式统一处理多协议下载的人

## 核心能力

- 多协议下载：支持 HTTP(S)、FTP、SFTP、BitTorrent 和 Metalink
- 分段并发：可从多个来源同时下载，尽量吃满带宽
- 守护进程接口：提供 JSON-RPC / XML-RPC，适合远程控制与自动化
- 校验与续传：支持 chunk 校验、断点续传和批量 URI 输入

## 典型使用场景

- 在服务器上批量拉取模型、镜像或数据文件
- 用脚本统一调度下载任务并监控状态
- 结合 BitTorrent 与 HTTP 源做更高效的分发下载

## 为什么值得关注

- 它是 CLI 下载器里的老牌基础设施级项目
- 功能不只停留在“下载文件”，而是兼顾自动化和远程控制
- 对终端工作流来说，aria2 往往比浏览器下载更稳、更可编排

## 类似项目

- [yt-dlp](yt-dlp.md) - 同样是强命令行下载工具，但更专注音视频站点和媒体处理
- [rclone](rclone.md) - 同样擅长数据传输，但重点是云存储同步与挂载，不是通用下载

## 官方链接

- **官网:** https://aria2.github.io/
- **GitHub:** https://github.com/aria2/aria2
- **文档:** https://aria2.github.io/manual/en/html/
- **更新记录:** https://github.com/aria2/aria2/releases

## 标签

- `Download`, `CLI`, `BitTorrent`, `HTTP`, `Automation`

## 更新观察点

- 后续重点观察协议支持、RPC 能力和跨平台构建状态
- 优先重新抓取项目主页、在线 manual 和 releases
- 如果后续在守护进程或自动化接口上有明显增强，值得补入正文
