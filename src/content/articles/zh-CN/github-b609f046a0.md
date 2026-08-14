---
decisionKey: "b609f046a0995000b51c9a4e286401757f7950a47f040902ed362241d2d4747b"
language: "zh-CN"
title: "GitHub 依赖图改进：软件包注册表成为许可证信息的主要来源"
summary: "GitHub 现在优先从软件包注册表（如 npmjs.org 和 PyPI）获取依赖图中的许可证信息，而不是主要依赖 ClearlyDefined，从而将缺失许可证的比例从 45% 降至 24%。这一变化提高了 SBOM、安全警报和合规工具的许可证准确性。"
publishedAt: "2026-08-14T05:45:30.156Z"
score: 0.85
topics:
  - "Dependency Graph"
  - "License Compliance"
  - "SBOM"
  - "GitHub Advanced Security"
topicIds:
  - "dependency-graph-e76q0g"
  - "license-compliance-59bon"
  - "sbom-za515c"
  - "github-advanced-security-1lb7vwq"
sourceUrls:
  - "https://github.blog/changelog/2026-08-13-license-data-quality-improvements"
---

- GitHub 现在将 npmjs.org 和 PyPI 等软件包注册表作为依赖图中许可证信息的主要来源，仅在注册表数据不足时回退到 ClearlyDefined。
- 对于 1.7 亿个被跟踪的软件包，依赖图中缺失许可证的数量从 45% 下降到 24%。
- 依赖图现在按版本范围记录许可证历史，因此新版本自动继承许可证元数据，无需单独的数据库条目。
