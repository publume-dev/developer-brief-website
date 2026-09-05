---
decisionKey: "d7b48152f5d95c53c4e298e7ce85e4a701cc8744302653c241164257f11b5e9e"
language: "en"
title: "npm packages can now have multiple trusted publishing (OIDC) configurations"
summary: "npm packages can now have multiple trusted publishing (OIDC) configurations, each independent and additive, with opt-in direct publishing per configuration and staged publishing by default."
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

- npm packages can now have more than one trusted publishing (OIDC) configuration, each independent and additive with its own repository, workflow, and environment criteria.
- Direct publishing is opt-in per trusted publishing configuration; every configuration can stage a package by default.
- In staged publishing, the approval button is disabled while a package is being malware scanned and becomes available once the scan completes; the status refreshes every minute.
- The versions tab on npmjs.com now shows maintainers a detailed history for each version, including approved, rejected, or still staged.
