---
decisionKey: "1868bff45346c38c5d5528b5236c58c1de57b10c271d9ad547cc36a4d023ed9d"
language: "zh-CN"
title: "GitHub Enterprise Live Migrations 正式发布，支持从 GHES 迁移到 GHEC DR"
summary: "GitHub 宣布 Enterprise Live Migrations 全面可用，支持从 GitHub Enterprise Server 迁移到 GitHub Enterprise Cloud with Data Residency，提供近零停机迁移。该功能专为大型单仓库和持续活跃的仓库设计，可将切换时间缩短至数分钟。"
publishedAt: "2026-09-02T12:05:26.117Z"
score: 0.85
topics:
  - "GitHub Enterprise Migration"
  - "Platform Engineering"
  - "DevOps"
topicIds:
  - "github-enterprise-migration-136912x"
  - "platform-engineering-uztf0l"
  - "devops-5y6th4"
sourceUrls:
  - "https://github.blog/changelog/2026-09-01-enterprise-live-migrations-from-ghes-to-ghe-com-generally-available"
---

- Enterprise Live Migrations (ELM) 现已全面可用，支持从 GitHub Enterprise Server (GHES) 迁移到 GitHub Enterprise Cloud with Data Residency (GHEC DR)。
- ELM 持续同步源和目标数据，开发者可在迁移期间继续工作，切换仅需排空进行中的变更，从而在数分钟内完成切换，而非数天。
- ELM 专为具有深度 Git 历史、大量 issues 和 pull requests 以及持续活跃的大型单仓库设计，并提供资源级进度跟踪，在切换前揭示失败。
- ELM 补充了 GitHub Enterprise Importer (GEI)：GEI 用于简单且能接受短暂停机的迁移，ELM 用于零中断迁移，两者可作为同一迁移策略的一部分并发运行。
- ELM 通过 `gh elm` GitHub CLI 扩展管理，该扩展配置凭据并通过 GHES REST API 管理生命周期，支持人类可读和 JSON 输出以用于自动化。
- ELM 支持从 GHES 版本 3.17.18+、3.18.12+、3.19.9+、3.20.3+、3.21.3+ 和 3.22.0+ 迁移，并在 GHES 设备上作为服务运行，由 `gh elm` CLI 驱动。
