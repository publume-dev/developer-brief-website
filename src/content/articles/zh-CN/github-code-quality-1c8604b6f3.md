---
decisionKey: "1c8604b6f31775531d0a0d2d7992bdfa0000b14811a04e552988f864a7bf3537"
language: "zh-CN"
title: "GitHub Code Quality 启用变更现已在审计日志中跟踪"
summary: "GitHub 宣布新的审计日志事件，用于跟踪 Code Quality 在仓库级别的启用、禁用和设置变更，帮助组织明确计费范围。"
publishedAt: "2026-08-23T13:44:57.509Z"
score: 0.9
topics:
  - "GitHub"
  - "Code Quality"
  - "Audit Log"
topicIds:
  - "github-9o7vw2"
  - "code-quality-1d1hzq5"
  - "audit-log-gc1voq"
sourceUrls:
  - "https://github.blog/changelog/2026-08-20-track-github-code-quality-enablement-changes-in-the-audit-log"
---

- GitHub Code Quality 现在会在仓库上启用、禁用或更改设置时写入审计日志事件，新增三种事件类型：`repo.code_quality_enabled`、`repo.code_quality_disabled` 和 `repo.code_quality_updated`。
- 每个审计日志事件捕获仓库、操作者及发生时间，使组织能够确切看到仓库何时进入或离开 Code Quality 计费范围。
- 这些审计日志事件可在组织审计日志、企业审计日志中查看，并可通过审计日志 API 查询。
- Code Quality 适用于 GitHub Enterprise Cloud、带数据驻留的 GitHub Enterprise Cloud 以及 GitHub Team。
