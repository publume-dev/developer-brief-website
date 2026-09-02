---
decisionKey: "20a5797dd616fea817de428c1bf42bdd2fc2339b7d20c04ba9284e8ea306a1ff"
language: "en"
title: "GitHub CLI v2.99.0 adds --attach for media in issues, PRs, and comments"
summary: "GitHub CLI v2.99.0 introduces a general --attach flag that makes it possible to upload and reference local media in issues, pull requests, and comments. The feature is available to everyone on all plans with no preview."
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

- A repeatable `--attach` flag is added for `gh issue create/edit/comment` and `gh pr create/edit/comment` to upload local images or videos and reference them inline.
- Generally available to all users on all GitHub plans; no preview period.
- Supported attachment formats: PNG, JPEG, GIF, WebP, SVG, MP4, MOV, and WebM.
- Size limits match the web upload flow: 10 MB for images and GIFs; 10 MB for video on Free plans and 100 MB for video on paid plans.
- GitHub Enterprise Server is not supported in this release.
