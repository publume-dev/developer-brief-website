---
decisionKey: "21f6601dc6af4a0b06ca06ef91039691cb572673010db3c8df0c0856d0cd22a0"
language: "zh-CN"
title: "GitHub Code Quality 现使用独立的 GitHub Actions 路径"
summary: "GitHub 已为 GitHub Code Quality 推出独立的 Actions 路径，不再与代码扫描共享路径，这会影响工作流运行历史、使用量报告，并需要更新脚本和仪表盘。"
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

- GitHub Code Quality 现在使用动态路径 `dynamic/github-code-quality/codeql` 和 `github-code-quality` actor，而非代码扫描路径 `dynamic/github-code-scanning/codeql` 和 `github-advanced-security` actor。
- 使用量报告、脚本、仪表盘及工作流运行过滤器需更新，以同时考虑新的路径和 actor。
- 该更改适用于 GitHub Enterprise Cloud、GitHub Team 以及支持数据驻留的 GitHub Enterprise Cloud。
