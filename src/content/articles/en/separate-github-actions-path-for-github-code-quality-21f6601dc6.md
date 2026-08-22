---
decisionKey: "21f6601dc6af4a0b06ca06ef91039691cb572673010db3c8df0c0856d0cd22a0"
language: "en"
title: "Separate GitHub Actions Path for GitHub Code Quality"
summary: "GitHub now uses a separate Actions path for GitHub Code Quality instead of sharing the code scanning path, affecting workflow run history, usage reports, and requiring updates to scripts and dashboards."
publishedAt: "2026-08-22T13:43:12.485Z"
score: 0.85
topics:
  - "GitHub Actions"
  - "GitHub Code Quality"
  - "Code Quality"
topicIds:
  - "github-actions-7tcwgt"
  - "github-code-quality-2h14ma"
  - "code-quality-1d1hzq5"
sourceUrls:
  - "https://github.blog/changelog/2026-08-20-separate-github-actions-path-for-github-code-quality"
---

- GitHub Code Quality now uses dynamic path `dynamic/github-code-quality/codeql` and the `github-code-quality` actor, instead of the code scanning path `dynamic/github-code-scanning/codeql` and the `github-advanced-security` actor.
- Update usage reports, scripts, dashboards, and workflow run filters to account for the new path and actor.
- The change is available on GitHub Enterprise Cloud, GitHub Team, and GitHub Enterprise Cloud with data residency.
