---
decisionKey: "8c635bc3d801896d76dc40a182b71fd3350afb3bf48b012d4a91a10cd9d6891b"
language: "zh-CN"
title: "Pinterest 用 RPP 集中化 AWS Terraform 管线"
summary: "Pinterest 的 Resource Provisioner Pipeline 集中执行 AWS Terraform，让跨多个仓库的基础设施变更获得最小权限访问和双人复核。它把 plan 和 apply 变成可分别审计的 PR 步骤，而不是依赖各仓库各自的 CI 配置。"
publishedAt: "2026-08-11T18:42:58.614Z"
score: 0.8
topics:
  - "Terraform"
  - "AWS"
  - "CI/CD"
  - "Security"
topicIds:
  - "terraform-16y9a1j"
  - "aws-7brv06"
  - "ci-cd-9jk1ml"
  - "security-1jtharf"
sourceUrls:
  - "https://www.infoq.com/news/2026/08/pinterest-secures-aws-infra/"
---

- Pinterest 公布了 Resource Provisioner Pipeline（RPP），这是一个面向 AWS 基础设施的集中式 Terraform 执行引擎，强制最小权限访问和双人复核。
- RPP 以一组复合 GitHub Actions 的形式运行在 GitHub 拉取请求事件上，将 PR 拆分为每个受影响的 Terraform 工作区各自的 plan/apply 运行。
- 它采用链式角色模型：工作流先通过 OIDC 假定中央 RPPActionsRole，读取将工作区映射到仓库和 IAM 角色的源配置，并在假定工作区团队角色前验证 Terraform 代码路径与该工作区的 S3 后端和 KMS 密钥一致。
- 变更需要所属仓库的已批准复核人签署同意；apply 仅由 PR 上明确的人工评论触发，使 plan 和 apply 保持为独立可审计的操作。
- 集中式管线为系统性修复提供单一控制点，并运行一致的 PR 触发检查，包括使用自定义 Semgrep 规则的静态分析、AI 辅助扫描，以及可选的基于 LocalStack 的 dry run。
- RPP 是私有系统，未开源。
- 报道局限：InfoQ 的文章未提供 Pinterest 原始博客文章或演讲，因此这些细节未经主要来源独立核实。
