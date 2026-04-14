---
title: "Khazix Skills"
entity_type: "tool"
category: "Prompt / Context Management"
last_reviewed_at: "2026-04-15"
---

# Khazix Skills

## 一句话总结

一个把深度研究与长文写作方法论沉淀成 prompts 和可安装 skills 的开源仓库，适合给 Claude Code、Codex、OpenClaw 等 agent 直接装配方法论能力。

## 快速判断

- 如果你想把“研究怎么做”“长文怎么写”直接装进 agent，而不是每次手写提示词，它值得优先看
- 如果你要的是现成 SaaS 内容工具，而不是可安装的 prompt / skill 资产，先看别的方案
- 它更像方法论 skill 仓库和上下文资产包，不是单一 AI 产品

## 你会怎么用它

- 接进 AI 开发流：把研究和写作技能装进 Claude Code、Codex、OpenClaw 等 agent，当作可复用的 prompt / skill 层
- 接进日常工作流：把深度研究、公众号长文写作等高频任务从“临时发挥”变成固定方法论入口
- 最小落地方式：先挑一个 prompt 或一个 skill 装进去，验证它是否真的比你现有提示词更稳

## 它解决什么问题

- 很多方法论只存在于个人脑子里或零散 prompt 里，难以长期复用
- 同一套研究或写作套路，换到不同 agent 工具里往往又要重新整理
- 用户想把个人经验沉淀成 agent 可自动加载的资产，但缺少统一格式和示范仓库

## 适合谁

- 想给 Claude Code、Codex、OpenClaw 安装现成 skills 的用户
- 需要把研究与写作方法论做成可复用 agent 资产的人
- 想在多 agent 工具之间复用 prompts 与 structured skills 的实践者

## 核心能力

- Prompt + Skill 双形态：既提供可复制 prompt，也提供更结构化的 skill 包
- 安装面明确：README 直接给出 Claude Code、Codex、OpenClaw 的安装路径与安装方式
- 方法论沉淀：当前重点覆盖深度研究与长文写作两类高价值场景
- 开放标准兼容：skills 遵循 Agent Skills 开放标准，便于在不同 agent 环境里复用

## 能力边界

- 明显可用：想把研究和写作方法论沉淀成 agent 可加载资产的场景
- 效果一般：只想找一个即开即用的内容产品，或者不使用 skill 生态的场景
- 不要误用：不要把它理解成“自动帮你写好所有内容”的成品工具；它更像高质量方法论资产包

## 集成方式

- 作为单独工具：直接复制 prompts，或把 skills 安装到目标 agent 工具中
- 作为 AI 工作流组件：放在 prompt / context / skill 层，给不同 agent 复用同一套方法论
- 作为团队流程节点：适合把个人研究和写作经验固化为团队可共享的 skill 资产

## 上手建议

- 第一步先选一个最贴近你当前需求的入口，比如 `hv-analysis` 或 `khazix-writer`
- 最值得先试的是你本来就重复在做、但质量不稳定的研究或写作任务
- 如果你还不确定 skill 格式是否适合自己，先从 prompt 版本轻量试用，不要一开始大规模迁移

## 选型建议

- 如果你的主需求是把方法论做成可安装的 agent skills，适合看它
- 如果你的主需求是直接找研究结果或成品文章，它不是那种交付型工具
- 如果你最看重的是跨 Claude Code、Codex、OpenClaw 复用 prompt / skill 资产，这个仓库的价值会比较明显

## 为什么值得关注

- 它展示了怎样把个人方法论从“会用”变成“可安装、可复用、可迁移”
- 同时覆盖 prompt 和 skill 两种形态，参考价值比只有 prompt 的仓库更高
- 对 skill 生态来说，这类既有内容方法论、又有安装路径的仓库很适合做样板

## 类似项目

- [gstack](../../awesome-ai-for-coding/items/gstack.md) - 更偏完整软件工厂和工程流程 skills；Khazix Skills 更偏研究与写作方法论资产。
- [FlowMind for Claude](flowmind-for-claude.md) - 更偏把外部系统接进 agent；Khazix Skills 更偏把方法论本身做成可加载 skill。

## 官方链接

- **GitHub:** https://github.com/KKKKhazix/khazix-skills
- **更新记录:** https://github.com/KKKKhazix/khazix-skills/releases

## 标签

- `Skills`, `Prompts`, `Claude Code`, `Codex`, `OpenClaw`

## 参考依据

- 这条说明主要依据项目 README、安装说明和 releases 页面整理而成
- 关于“归入 CLI 而不是 life”的判断，来自它的产品本体首先是可安装 skill / prompt 资产，而不是单纯面向读者的研究或写作内容

## 更新观察点

- 后续优先观察新 skill 类型是否继续扩展，而不只是增加 prompt 数量
- 关注 releases 中 `.skill` 安装包是否保持更新，以及是否支持更多 agent 工具
- 如果后续补充更多方法论模块或更细的 skill 说明，值得继续更新条目
