---
decisionKey: "b609f046a0995000b51c9a4e286401757f7950a47f040902ed362241d2d4747b"
language: "en"
title: "GitHub dependency graph now prioritizes package registry license data"
summary: "GitHub now uses package registries like npmjs.org and PyPI as the primary source for license information in the dependency graph, reducing missing licenses from 45% to 24% across 170 million packages. This improves license accuracy in SBOMs, security alerts, and compliance tooling."
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

- GitHub now uses package registries such as npmjs.org and PyPI as the primary source for license information in the dependency graph, falling back to ClearlyDefined only when registry data is insufficient.
- Missing licenses in the dependency graph dropped from 45% to 24% for the 170 million tracked packages.
- The dependency graph now records license history by version ranges, so new versions automatically inherit license metadata without requiring individual database entries.
