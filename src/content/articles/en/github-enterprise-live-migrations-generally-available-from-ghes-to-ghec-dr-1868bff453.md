---
decisionKey: "1868bff45346c38c5d5528b5236c58c1de57b10c271d9ad547cc36a4d023ed9d"
language: "en"
title: "GitHub Enterprise Live Migrations generally available from GHES to GHEC DR"
summary: "GitHub announced general availability of Enterprise Live Migrations, enabling near-zero-downtime migrations from GitHub Enterprise Server to GitHub Enterprise Cloud with Data Residency. Designed for large monorepos with constant activity, it lets cutover happen in minutes rather than days."
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

- Enterprise Live Migrations (ELM) is now generally available, enabling near-zero-downtime repository migrations from GitHub Enterprise Server (GHES) to GitHub Enterprise Cloud with Data Residency (GHEC DR).
- ELM continuously syncs data from source to target, so developers keep working during migration and cutover requires only time to drain in-flight changes, enabling cutover in minutes rather than days.
- ELM is purpose-built for large monorepos with deep git history, large volumes of issues and pull requests, and constant activity, and provides resource-level progress tracking to surface failures before cutover.
- ELM complements GitHub Enterprise Importer (GEI), allowing use of GEI for straightforward migrations with brief downtime and ELM for zero-disruption migrations, and they can run concurrently as part of the same migration strategy.
- ELM is managed through the `gh elm` GitHub CLI extension, which configures credentials and manages the lifecycle through the GHES REST API, with human-readable and JSON output for automation.
- ELM supports migrations from GHES versions 3.17.18+, 3.18.12+, 3.19.9+, 3.20.3+, 3.21.3+, and 3.22.0+, and runs as a service on the GHES appliance driven by the `gh elm` CLI.
