---
title: "DESIGN.md"
entity_type: "tool"
category: "Prompt / Context Management"
last_reviewed_at: "2026-04-23"
---

# DESIGN.md

## 一句话总结

Google Labs 推出的开放设计规范与配套 CLI，用一份 `DESIGN.md` 把机器可读 design tokens 和人类可读设计 rationale 合在一起，让 coding agents 持续理解同一套视觉系统。

## 快速判断

- 如果你想减少 agent 在 UI 生成里“自己猜品牌色、间距和组件风格”的情况，它非常值得关注
- 如果你现在只需要一个现成 UI 组件库，而不是一份可移植的设计语义规范，先看别的工具
- 它当前更像“设计上下文标准 + 验证 CLI”，不是已经被所有 coding agents 原生支持的通用协议

## 你会怎么用它

- 做设计约束：在项目根目录维护一份 `DESIGN.md`，给 agent 提供稳定的视觉上下文
- 做规范校验：用 `npx @google/design.md lint DESIGN.md` 检查结构、token 引用和 WCAG 对比度
- 做版本回归：用 `diff` 看设计 token 或 prose 有没有退化
- 做生态对接：用 `export` 导出 Tailwind theme 或 W3C DTCG `tokens.json`

## 它解决什么问题

- 现在很多 agent 做前端时，能看懂自然语言风格描述，但拿不到精确设计 token
- 单纯给一张截图或一句“做得高级一点”，很难稳定复用同一套品牌视觉
- 设计系统常常分散在 Figma、样式文件、口头要求和 prompt 里，agent 很难长期继承

## 适合谁

- 想让 AI coding agents 持续遵守同一套视觉语言的前端团队
- 想把品牌设计、组件约束和 UI 风格写成可版本化文本资产的人
- 需要在设计生成、代码生成和主题导出之间保留统一 token 源的人

## 核心能力

- 双层格式：YAML front matter 负责精确 token，Markdown body 负责解释为什么这样设计
- 固定章节顺序：规范正文以 `Overview`、`Colors`、`Typography`、`Layout`、`Elevation & Depth`、`Shapes`、`Components`、`Do's and Don'ts` 为主轴
- CLI 工具链：内置 `lint`、`diff`、`export`、`spec`
- 结构化输出：CLI 默认输出 JSON，方便 agent 或脚本继续消费

## 能力边界

- 它定义的是“怎么描述设计系统”，不是直接替代 Figma、组件库或视觉审美判断
- 当前官方仓库明确标注格式仍处于 `alpha`，规范和 CLI 还在演进
- 截至 2026-04-23，官方仓库提供的是开放标准和 CLI；Codex、Claude Code、Cursor 的原生消费支持仍要看各家后续跟进

## 集成方式

- 作为单独工具：直接在项目里维护 `DESIGN.md`，再用 CLI 验证、对比和导出
- 作为 agent 上下文层：把 `DESIGN.md` 连同 `AGENTS.md` 一起作为项目长期上下文
- 作为设计到代码桥梁：把设计 token 从一份文本规范导出到 Tailwind 或 DTCG token 文件

## 上手建议

- 第一步先写最小可用版本：`colors`、`typography`、`rounded`、`spacing` 和关键 `components`
- 最值得先试的场景是：现有项目经常让 agent 改 UI，但每次风格都漂移
- 如果你在团队里引入它，先把“哪些 token 是规范值，哪些 prose 是解释”这条边界讲清楚

## 选型建议

- 如果你的主需求是“让 agent 稳定继承同一套视觉系统”，它很合适
- 如果你的主需求是“马上拿现成设计组件”，它不是那种现成 UI 库
- 如果你更看重的是 CLI 校验、规范 diff 和多格式导出，这个项目的工程价值会很明显

## 为什么值得关注

- 它把“设计规范给人看”和“设计 token 给机器读”合成了同一份文本资产
- 对 AI 辅助前端来说，这比只给截图或 prompt 更容易稳定复现品牌风格
- 它还自带验证、diff 和导出链路，不只是一个静态规范文档

## 类似项目

- [Khazix Skills](khazix-skills.md) - 更偏方法论 skill 资产；DESIGN.md 更偏把视觉规范做成 agent 可读上下文标准
- [Logo Generator Skill](logo-generator-skill.md) - 更偏直接生成品牌视觉方案；DESIGN.md 更偏把既定视觉系统固化为长期规范

## 官方链接

- **Spec Repo:** https://github.com/google-labs-code/design.md
- **Specification:** https://stitch.withgoogle.com/docs/design-md/specification

## 标签

- `Design System`, `Design Tokens`, `CLI`, `Prompt / Context`, `Google Labs`, `Tailwind`

## 参考依据

- 这条说明主要依据官方 README 与规范页面整理
- 其中关于 YAML front matter、章节顺序、`lint / diff / export / spec` 命令、`alpha` 状态和 DTCG / Tailwind 导出，来自当前官方公开文档

## 更新观察点

- 后续优先观察规范版本是否从 `alpha` 进入更稳定阶段
- 关注 `@google/design.md` CLI 是否补充更多导出目标和 lint 规则
- 如果 Codex、Claude Code、Cursor 后续出现原生消费 `DESIGN.md` 的公开支持，值得及时补充正文
