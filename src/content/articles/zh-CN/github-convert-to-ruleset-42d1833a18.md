---
decisionKey: "42d1833a18985a9f8da716ca486cd17ed82c00e3781e1e23c7e31be44fb3080b"
language: "zh-CN"
title: "GitHub 新增 Convert to ruleset，可将分支保护规则迁移为规则集"
summary: "GitHub 仓库管理员现在可以将经典分支保护规则转换为仓库规则集，并保留必需的审查、状态检查和推送限制等设置。这为希望使用跨分支规则、规则分层和更细粒度绕过权限的团队提供了一条迁移路径。"
publishedAt: "2026-08-12T05:45:50.677Z"
score: 0.9
topics:
  - "GitHub"
  - "Repository Management"
  - "Developer Tooling"
topicIds:
  - "github-9o7vw2"
  - "repository-management-lf9x50"
  - "developer-tooling-q9uwan"
sourceUrls:
  - "https://github.blog/changelog/2026-08-11-automatically-migrate-branch-protection-rules-to-repository-rulesets"
---

- GitHub 在仓库设置中新增 **Convert to ruleset** 选项，可将现有分支保护规则转换为仓库规则集。
- 转换会将分支保护配置（包括必需的审查、状态检查和推送限制）映射为等效的规则集规则。
- 所有支持规则集的仓库均可使用该转换功能。
- 使用方法：进入 **Settings → Branches**，在 **Branch protection rules** 下找到经典规则，然后点击 **Convert to ruleset**。
- 规则集提供分支保护之外的能力：通过模式匹配将规则应用到多个分支、叠加多个规则集、在组织或企业级管理规则集，以及配置精细的绕过权限。
- 更新日志未说明转换是否删除原始分支保护规则，也不确定该操作能否撤销。
