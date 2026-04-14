---
title: "gh-stack"
entity_type: "tool"
category: "CLI Tools"
last_reviewed_at: "2026-04-15"
---

# gh-stack

## 一句话总结

一个面向 stacked PR 工作流的 GitHub CLI extension，帮助开发者把大改动拆成多层可审查 PR，并自动处理分支、rebase、push 和 PR 基线关系。

## 快速判断

- 如果你想在终端里把 stacked PR workflow 跑顺，它值得优先看
- 如果你几乎不用 stacked PR，或者团队只靠单 PR 流程就够，不一定需要它
- 它更像 GitHub 协作命令面和 stacked PR CLI，而不是 AI 产品本体

## 你会怎么用它

- 接进 AI 开发流：让 Claude Code、Codex 等 coding agent 在 stacked PR 规则下更稳定地创建、同步和提交多层改动
- 接进日常工作流：把 branch stack、rebase、submit、sync 和 review 导航变成固定终端命令流，而不是手工维护
- 最小落地方式：先拿一个原本就准备拆成 2 到 3 层 PR 的改动试跑 `init -> add -> push -> submit`

## 它解决什么问题

- 大改动如果塞进一个 PR，review 很重；拆成多个 PR 又很容易手工维护崩掉
- stacked PR 需要频繁处理 base branch、rebase、顺序和 PR 状态，同步成本高
- coding agent 在多层分支提交里很容易搞错顺序和基线，影响 review 体验

## 适合谁

- 使用 stacked PR 工作流的开发者与团队
- 想把大改动拆成多层可审查 PR 的工程团队
- 希望让 AI coding agent 更好配合 GitHub 提交流程的实践者

## 核心能力

- Stack 初始化与扩展：支持创建、收养和扩展 branch stack
- Rebase / sync 自动化：集中处理整个 stack 的 fetch、rebase、push 和 PR 状态同步
- GitHub PR 基线管理：自动把每层 PR 的 base 指向下层分支
- 本地 stack 跟踪：把 stack 元数据写在 `.git/gh-stack`，不污染仓库提交
- Agent 集成：提供 gh-stack skill，让 coding agent 理解 stacked PR 工作流

## 能力边界

- 明显可用：大功能拆层、长链路重构、多人 review、AI 辅助提交和 stacked PR 协作
- 效果一般：小型仓库、极轻变更、团队根本不使用 stacked PR 的场景
- 不要误用：不要把它看成 AI 编码产品；它首先是 GitHub CLI extension 和 stacked PR 命令面

## 集成方式

- 作为单独工具：直接通过 `gh stack` 管理 stack 的 init、add、checkout、rebase、sync、submit
- 作为 AI 工作流组件：放在 coding agent 的提交流程层，让 agent 不只是改代码，还能按 stack 组织交付
- 作为团队流程节点：适合团队把“大改动拆层 review”规范化，而不是靠人工记忆分支关系

## 上手建议

- 第一步先让一个真实的中型改动按 2 到 3 层 PR 来试，不要一开始就拉很长的 stack
- 最值得先试的是“逻辑相关但 reviewer 需要分层看”的改动
- 如果团队当前还没形成 stacked PR 习惯，先轻量试用，不要立刻要求所有人改工作流

## 选型建议

- 如果你的主需求是让 stacked PR 真正可操作、可维护，适合看它
- 如果你的主需求只是普通 GitHub CLI 或单 PR 提交流程，它未必是高优先级
- 如果你最在意的是 AI coding agent 如何和 GitHub stacked PR workflow 协同，gh-stack 的价值会比较明显

## 为什么值得关注

- 它解决的是“怎么在终端里交付大改动”这个高频且很容易出错的工程问题
- 由 GitHub 官方做的 stacked PR CLI extension，和 `gh` 生态天然贴近
- 对 AI coding 场景来说，stacked PR 这种强结构工作流很适合让 agent 配合执行

## 类似项目

- [GitHub CLI](github-cli.md) - GitHub 官方通用命令入口；gh-stack 更聚焦 stacked PR 工作流。
- [onecli](onecli.md) - 更偏 agent credentials 和命令能力协调；gh-stack 更偏 GitHub PR 协作命令面。

## 官方链接

- **GitHub:** https://github.com/github/gh-stack
- **更新记录:** https://github.com/github/gh-stack/releases

## 标签

- `GitHub`, `CLI`, `Pull Requests`, `Stacked PRs`, `Developer Workflow`

## 参考依据

- 这条说明主要依据项目 README 和 releases 页面整理而成
- 关于“归入 CLI 而不是 coding”的判断，基于它本身不是 AI 项目，而是可被 AI coding workflow 利用的 GitHub CLI extension

## 更新观察点

- 后续优先观察 private preview 是否开放，以及 GitHub 上 Stack 视图能力是否继续增强
- 关注 agent skill 是否继续完善，尤其是对 Claude Code / Codex 的协作支持
- 如果后续功能明显扩展成更完整的开发工作台，需要重新复核 repo 归属
