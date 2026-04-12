---
title: "textutil"
entity_type: "tool"
category: "CLI Tools"
last_reviewed_at: "2026-04-12"
---

# textutil

## 一句话总结

macOS 自带的文档与富文本转换 CLI，可在终端里查看、拼接并转换 TXT、HTML、RTF、DOCX、ODT 等格式。

## 它解决什么问题

- macOS 上很多文档格式互转默认依赖 GUI，批处理和脚本接入不方便
- AI 工作流经常要把 Word、RTF 或 HTML 材料转成更易处理的纯文本或中间格式
- 本地知识整理、归档和导出流程需要一个系统自带、无需额外安装的转换工具

## 适合谁

- 需要在 macOS 上批量处理文档格式的人
- 想把文本清洗和格式转换接进 shell 脚本或 AI agent 工作流的人
- 经常处理富文本、Word 文档和 HTML 材料的人

## 核心能力

- 格式转换：支持 `txt`、`html`、`rtf`、`rtfd`、`doc`、`docx`、`wordml`、`odt` 和 `webarchive`
- 文件拼接：可用 `-cat` 把多份输入合并成单个目标文件
- 元数据控制：支持设置标题、作者、主题、关键字和时间字段
- 编码与格式指定：可显式控制输入编码、输出编码、扩展名和解释格式
- HTML 处理：支持 `-noload`、`-nostore`、`-baseurl` 等网页相关选项

## 典型使用场景

- 把 `.docx` 或 `.rtf` 批量转成纯文本，作为后续摘要、索引或 RAG 输入
- 把多份富文本材料拼接成一份 HTML 或 RTF 归档文件
- 在本地脚本里做文档清洗、转存和标准化输出，而不打开 GUI 应用

## 为什么值得关注

- 它是 macOS 原生自带工具，开箱即用，适合直接进终端自动化
- 对 AI agent 来说，这类“先规范化文档再交给模型”的工具很实用
- 相比另装大而全的转换器，`textutil` 很适合处理轻量级本地文档整理任务

## 类似项目

- [Pandoc](pandoc.md) - 更通用、跨平台、格式覆盖更广；`textutil` 更轻量，也更偏 macOS 原生
- [ImageMagick](imagemagick.md) - 同样适合批处理和格式转换，但对象是图像而不是文本文档

## 官方链接

- **官网:** https://ss64.com/mac/textutil.html

## 标签

- `macOS`, `CLI`, `Documents`, `Conversion`, `Rich Text`

## 更新观察点

- 后续重点看 Apple 是否扩展支持格式、编码选项或元数据处理能力
- 如果未来 macOS 版本补充更适合 Markdown / plain text 工作流的参数，值得更新条目
