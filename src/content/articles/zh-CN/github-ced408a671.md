---
decisionKey: "ced408a6711a69cd8198c8f0267424f02f6d61b39050525265359727bc7a3dfb"
language: "zh-CN"
title: "GitHub 发布替代文本质量插件，内置五个确定性规则和可选模型检查"
summary: "GitHub 为其无障碍扫描器发布了新的替代文本质量插件，默认启用五个确定性规则，并提供一个可选的基于模型的检查功能。该插件旨在帮助开发者识别缺失或低质量的替代文本，改善网页可访问性。"
publishedAt: "2026-08-25T14:27:51.056Z"
score: 0.85
topics:
  - "Accessibility"
  - "Developer Tooling"
  - "GitHub"
topicIds:
  - "accessibility-tz69kv"
  - "developer-tooling-q9uwan"
  - "github-9o7vw2"
sourceUrls:
  - "https://github.blog/engineering/user-experience/your-alt-text-passes-automated-checks-that-doesnt-mean-its-any-good/"
---

- GitHub 为其无障碍扫描器发布了替代文本质量插件，默认启用五个确定性规则，并包含一个可选的基于模型的检查功能。
- 确定性规则可检测缺失替代文本、文件名、占位符、通用词和重复替代文本；重复规则使用布局临近性而非 DOM 顺序，并设置间隙阈值以确定相邻图像何时构成重复序列。
- 可选的模型规则默认关闭，需要具有 GitHub Models 访问权限的令牌，仅发送图像和经过处理后的上下文（剥离查询和片段的 URL），并使用四步决策流程将替代文本分类为装饰性、冗余性、功能性或信息性。
