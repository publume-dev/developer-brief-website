---
decisionKey: "d7b48152f5d95c53c4e298e7ce85e4a701cc8744302653c241164257f11b5e9e"
language: "zh-CN"
title: "npm 包现支持多个可信发布（OIDC）配置"
summary: "npm 包现在可以配置多个可信发布（OIDC）配置，每个配置独立且可叠加，并支持按配置选择直接发布或默认的分阶段发布。"
publishedAt: "2026-09-05T12:04:28.250Z"
score: 0.85
topics:
  - "npm"
  - "trusted publishing"
  - "OIDC"
  - "package publishing"
  - "GitHub"
topicIds:
  - "npm-dzkzh6"
  - "trusted-publishing-1fhgmip"
  - "oidc-xsdu80"
  - "package-publishing-1dlhxik"
  - "github-9o7vw2"
sourceUrls:
  - "https://github.blog/changelog/2026-09-03-multiple-trusted-publishing-configurations-for-npm"
---

- npm 包现在可以有多个可信发布（OIDC）配置，每个配置独立且可叠加，包含各自的仓库、工作流和环境条件。
- 直接发布是按每个可信发布配置选择加入的，默认情况下每个配置都会分阶段发布包。
- 在分阶段发布中，当包正在进行恶意软件扫描时，批准按钮被禁用，并在扫描完成后变为可用；状态每分钟刷新一次。
- npmjs.com 上的版本选项卡现在向维护者显示每个版本的详细历史，包括已批准、已拒绝或仍处于分阶段状态。
