---
title: "Defuddle"
entity_type: "tool"
category: "CLI Tools"
last_reviewed_at: "2026-04-11"
---

# Defuddle

## 一句话总结

一个能从网页或本地 HTML 中提取正文并输出干净 HTML、Markdown 或 JSON 的内容抽取工具，既可嵌进程序，也能直接在终端里用 CLI 跑。

## 它解决什么问题

- 网页正文常被评论区、侧栏、导航和脚注等噪音包围，不适合直接送给模型或知识库。
- 许多内容抓取工具只返回原始 HTML，后续还得自己做一轮清洗和格式转换。
- 需要在 shell 或 agent 流程里快速把网页转成 Markdown 时，自己拼脚本很麻烦。

## 适合谁

- 想把网页转成 Markdown 或结构化 JSON 的 CLI 用户
- 在 agent 工作流里做网页抓取、清洗和摘要前处理的开发者
- 需要可替代 Readability 的正文提取组件的人

## 核心能力

- 正文提取：自动移除评论、侧栏、页头页脚和其他非核心元素，只保留主要内容。
- 多输出格式：支持干净 HTML、Markdown、JSON 以及单属性抽取。
- 多环境使用：可在浏览器、Node.js 和 CLI 三种环境下运行。
- 元数据补全：除正文外还能返回标题、作者、描述、发布日期、schema.org 数据和字数等信息。

## 典型使用场景

- 在终端里用 `npx defuddle parse <url> --markdown` 快速把文章转成 Markdown。
- 给 agent 的网页抓取链路加一个“正文净化”步骤，减少无效上下文。
- 为知识库或剪藏工具准备更稳定的网页正文和元数据。

## 为什么值得关注

- 它不只是“读取网页”，而是把网页整理成更适合模型和笔记工具消费的形式。
- README 把浏览器、Node 和 CLI 三种使用方式都写得很清楚，落地成本低。
- 对 `awesome-cli-for-ai` 来说，这类“terminal-first content extraction” 是非常实用的基础工具。

## 类似项目

- [browser-use](browser-use.md) - 更偏让 agent 操作浏览器完成任务，而 `Defuddle` 更聚焦网页内容提取和清洗。
- [Mozilla Readability](https://github.com/mozilla/readability) - 同样做正文提取，但 `Defuddle` 更强调 Markdown、CLI 和更丰富的元数据输出。

## 官方链接

- **GitHub:** https://github.com/kepano/defuddle
- **npm:** https://www.npmjs.com/package/defuddle
- **更新记录:** https://github.com/kepano/defuddle/releases

## 标签

- `CLI`, `Markdown`, `Web Extraction`, `Content Parsing`, `HTML`

## 更新观察点

- 后续重点看 CLI 选项、输出格式和 debug 信息是否继续增强。
- 持续关注正文抽取准确率、数学公式处理和 schema.org 元数据提取能力。
- 优先重抓 README、CLI 示例和 releases，确认默认 bundle 与安装方式是否变化。
