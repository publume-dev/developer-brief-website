---
decisionKey: "1c8604b6f31775531d0a0d2d7992bdfa0000b14811a04e552988f864a7bf3537"
language: "en"
title: "Track GitHub Code Quality enablement changes in the audit log"
summary: "GitHub announces new audit log events to track repository-level enablement, disablement, and setting changes for Code Quality, helping organizations see billing scope."
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

- GitHub Code Quality now writes audit log events when someone enables, disables, or changes its settings on a repository, with three new event types: `repo.code_quality_enabled`, `repo.code_quality_disabled`, and `repo.code_quality_updated`.
- Each audit log event captures the repository, the actor who made the change, and when it happened, letting organizations see exactly when a repository entered or left the scope of Code Quality billing.
- These audit log events are available in the organization audit log, enterprise audit log, and can be queried with the audit log API.
- Code Quality is available on GitHub Enterprise Cloud, GitHub Enterprise Cloud with data residency, and GitHub Team.
