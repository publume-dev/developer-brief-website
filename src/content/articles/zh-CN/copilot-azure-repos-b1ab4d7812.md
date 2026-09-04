---
decisionKey: "b1ab4d78127b1453adf5b28eb0f317fc30d78a14584b595ab7afd79fd91bc765"
language: "zh-CN"
title: "Copilot 代码评审扩展至 Azure Repos，按次计费且用量报告延迟两天"
summary: "GitHub Copilot 代码评审现已面向所有 Azure DevOps 客户开放，无需注册，按评审次数计费，并支持组织、项目及仓库级别的启用控制。"
publishedAt: "2026-09-04T12:05:05.180Z"
score: 0.85
topics:
  - "Azure DevOps"
  - "GitHub Copilot"
  - "Code Review"
  - "Developer Tooling"
  - "Billing"
topicIds:
  - "azure-devops-pjzhht"
  - "github-copilot-mbl6jy"
  - "code-review-ig4nr4"
  - "developer-tooling-q9uwan"
  - "billing-i5mxng"
sourceUrls:
  - "https://www.infoq.com/news/2026/09/copilot-code-review-azure-repos/"
---

- GitHub Copilot 代码评审现已面向所有 Azure DevOps 客户开放，无需申请，此前自 6 月起处于有限预览状态。
- 该功能在拉取请求上发布评审评论，并通过关联的 Azure 订阅按评审次数计费，使用情况报告延迟 48 小时。
- 8 月发布的版本增加了组织、项目和仓库级别的启用控制，并支持 Managed DevOps Pools、自定义指令（支持按路径定向）以及通过分支策略进行自动评审。
- 费用显示在 Azure Cost Management 中的 'GitHub Copilot for AzDO' 下，带有 Azure DevOps 项目标签，并在评审完成后 48 小时出现；预算仅发送通知，不会阻止评审。
- 并发限制：每个组织 5 个并发评审，每个用户 2 个，每个拉取请求 1 个。该功能运行在 Azure Pipelines 基础设施上，使用默认代理池或使用 Ubuntu Server 的 Managed DevOps Pools；不支持自托管代理。
- Copilot 始终留下“评论”评审，从不批准或请求更改；除非被要求，否则不会在新提交后重新评审，也不会阻止合并。已知问题包括评审在计划工具阶段后停止，以及约 60 分钟后被取消，修复程序将在一周内推出。
- 功能限制：仓库最大 10 GB，拉取请求更改文件数 ≤100 且无合并冲突，不支持 TFVC，区域分阶段推出持续两到三周。
