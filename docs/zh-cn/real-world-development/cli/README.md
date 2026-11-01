---
slug: zh-cn/real-world-development/cli
title: "GitHub Copilot CLI"
authors:
  - geektrainer
lastUpdated: 2026-09-18
---

**[GitHub Copilot CLI](https://docs.github.com/copilot/concepts/agents/about-copilot-cli)** 将 GitHub Copilot 作为代理式编码助手带入终端。它可以探索代码库、生成代码、运行命令，并连接外部工具——全部通过命令行完成，无需切换到图形化编辑器即可保持工作流畅。

本研讨会将带你完成 Tailspin Toys 的连续工作流：在 GitHub Codespaces 中准备项目，安装 Copilot CLI，为游戏添加星级评分，然后创建第一个拉取请求。接着从筛选 issue 入手，规划方案、实现功能并审查结果。你还将更新仓库说明、自定义质量检查技能、使用 Playwright MCP 测试行为，并创建 QA 智能体。最后，审查完整更改，在筛选拉取请求中使用 Agent Merge，并探索实用的斜杠命令。你还可以学习[使用 GitHub Copilot CLI 和 Foundry 的可选系列课程][foundry]。

为了聚焦研讨会内容，你将创建两个拉取请求：一个用于星级评分，另一个用于筛选功能，其中包括说明、技能、QA 配置和测试的更新。筛选和质量工作共享同一对话和分支，让你在探索各项工具时能够继续已有工作。

## 课程

| 练习 | 主题 | 说明 |
|----------|-------|-------------|
| [0. 先决条件][ex0] | 设置 | 创建存储库和 Codespace |
| [1. 安装 Copilot CLI][ex1] | 安装 | 安装并验证 Copilot CLI，然后熟悉其基本用法 |
| [2. 添加星级评分：快速改进][ex2] | 首次更改 | 显示现有评分和空值时的提示，然后合并第一个拉取请求 |
| [3. 智能体模式：Plan 和 Autopilot][ex3] | 智能体模式 | 根据 issue 规划功能，使用 Autopilot 构建，再用 Interactive 模式审查 |
| [4. 使用自定义说明指导 Copilot][ex4] | 上下文 | 查看并更新说明，然后将其用于筛选功能 |
| [5. 自定义并使用 quality-checks 技能][ex5] | 可重复检查 | 查看现有技能、更改报告格式并运行检查 |
| [6. 使用 Playwright MCP 验证功能][ex6] | 浏览器观察 | 在 CLI 中配置 MCP 并检查筛选行为 |
| [7. 创建和使用 QA 智能体][ex7] | 需求和覆盖范围 | 创建并选择专用配置，然后收集最终验证证据 |
| [8. 创建并合并功能拉取请求][ex8] | 审查和合并 | 审查完整更改、创建拉取请求并使用 Agent Merge |
| [9. GitHub Copilot CLI 斜杠命令][ex9] | CLI 功能 | 探索上下文、模型、共享和可选的云智能体委派 |
| [10. 总结和后续步骤][ex10] | 总结 | 回顾工作流、可复用自定义项和其他资源 |
| [可选：集成 Foundry][foundry] | 托管智能体 | 准备模型、部署基于目录的智能体并将其连接到网站 |

## 先决条件

参加本工作坊前，请确保已具备以下条件：

- [ ] 拥有 GitHub 账户，并已启用 **Copilot Student、Pro、Pro+、Business 或 Enterprise** 计划
- [ ] 有权限创建存储库和 Codespace
- [ ] 了解终端或命令行的基本操作

> [!TIP]
> 没有付费计划？已验证学生可通过 [GitHub Education][callout-student-plan-education] 免费使用 GitHub Copilot。**Copilot Student** 计划包含本工作坊所用的智能体、MCP、代码审查和 Copilot CLI 功能。

[callout-student-plan-education]: https://github.com/education/students

> [!NOTE]
> 如果使用的是 Copilot Business 或 Copilot Enterprise，请确认管理员已启用 Copilot CLI。

## 开始

**[从练习 0：先决条件开始 →][ex0]**

[ex0]: 0-prerequisites/
[ex1]: 1-install-copilot-cli/
[ex2]: 2-add-star-rating/
[ex3]: 3-agent-modes/
[ex4]: 4-custom-instructions/
[ex5]: 5-agent-skills/
[ex6]: 6-mcp-playwright/
[ex7]: 7-qa-agent/
[ex8]: 8-create-pull-request/
[ex9]: 9-cli-power-tools/
[ex10]: 10-review/
[foundry]: 8-foundry-agent/
