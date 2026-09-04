---
decisionKey: "ee4e91c01339c5dbbb39b2f9a169de2dc0d361ccbb6a9effa40996c3bf529fda"
language: "zh-CN"
title: "GitHub Actions 新增运行器弃用 API、漏洞警报权限及可复用工作流作业上下文属性"
summary: "GitHub Actions 在 2026 年 9 月初的更新中推出了三项针对开发者的功能：用于规划运行器升级的新 REST API、GITHUB_TOKEN 的 vulnerability-alerts 权限以及可复用工作流的四个新作业上下文属性。这些更新有助于提升 CI/CD 的安全性和可维护性。"
publishedAt: "2026-09-04T12:05:05.180Z"
score: 0.85
topics:
  - "GitHub Actions"
  - "CI/CD"
  - "API"
  - "Security"
topicIds:
  - "github-actions-7tcwgt"
  - "ci-cd-9jk1ml"
  - "api-fnj3bb"
  - "security-1jtharf"
sourceUrls:
  - "https://github.blog/changelog/2026-09-03-github-actions-early-september-2026-updates"
---

- 新增 REST API 端点 `GET /actions/runners/deprecations/{version}`，支持仓库、组织或企业级，返回 `runner_version`、`runtime_deprecates_at` 和 `registration_deprecates_at` 以帮助规划运行器升级。
- `GITHUB_TOKEN` 现在支持 `vulnerability-alerts` 权限，值为 `read` 或 `none`，允许以只读方式访问 Dependabot 警报，实现最小权限。
- 可复用工作流现在可使用 `job.workflow_ref`、`job.workflow_sha`、`job.workflow_repository` 和 `job.workflow_file_path` 四个新作业上下文属性，这些属性反映定义当前作业的工作流。

新作业上下文属性不适用于 GitHub Enterprise Server，使用该平台的用户需注意。
