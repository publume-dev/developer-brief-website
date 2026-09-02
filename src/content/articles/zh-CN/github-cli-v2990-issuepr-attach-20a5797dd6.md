---
decisionKey: "20a5797dd616fea817de428c1bf42bdd2fc2339b7d20c04ba9284e8ea306a1ff"
language: "zh-CN"
title: "GitHub CLI v2.99.0 为 issue、PR 和评论新增 --attach 媒体上传"
summary: "GitHub CLI v2.99.0 引入通用的 --attach 标志，支持在 issue、PR 和评论中直接上传并引用本地媒体。该功能对所有用户和所有计划开放，无需预览。"
publishedAt: "2026-09-02T12:05:26.117Z"
score: 0.9
topics:
  - "GitHub CLI"
  - "Developer Tooling"
  - "CLI Features"
topicIds:
  - "github-cli-1vmpf8w"
  - "developer-tooling-q9uwan"
  - "cli-features-86zhdw"
sourceUrls:
  - "https://github.blog/changelog/2026-09-01-github-cli-media-in-issues-pull-requests-and-comments"
---

- 新增可重复的 `--attach` 标志，适用于 `gh issue create/edit/comment` 和 `gh pr create/edit/comment`，用于上传本地图片或视频并在内联引用。
- 一般可用，适用于所有 GitHub 计划的所有用户，无预览期。
- 支持的附件格式：PNG、JPEG、GIF、WebP、SVG、MP4、MOV 和 WebM。
- 大小限制与 Web 上传流程一致：图片和 GIF 为 10 MB；Free 计划视频为 10 MB；付费计划视频为 100 MB。
- 本次发布不支持 GitHub Enterprise Server。
