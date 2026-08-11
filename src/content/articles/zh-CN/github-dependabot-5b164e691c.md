---
decisionKey: "5b164e691c42ece4e4f529768f9b3ea96a23ee0bd716300a6f28fc54f454aa9e"
language: "zh-CN"
title: "GitHub 将 Dependabot 恶意软件警报扩展到八个包生态系统"
summary: "Dependabot 现在会在八个包生态系统中提供选择启用的恶意软件警报，并以 OpenSSF 恶意包报告为数据源，帮助更多供应链防范恶意软件。"
publishedAt: "2026-08-11T11:20:58.949Z"
score: 0.9
topics:
  - "Supply Chain Security"
  - "Dependabot"
  - "Malware Advisories"
  - "OpenSSF"
  - "Package Ecosystems"
topicIds:
  - "supply-chain-security-1fqvp23"
  - "dependabot-izuspz"
  - "malware-advisories-g0u4mz"
  - "openssf-1libmlv"
  - "package-ecosystems-1eljpak"
sourceUrls:
  - "https://github.blog/security/supply-chain-security/how-we-took-malware-advisories-beyond-npm/"
---

- Dependabot 现在会在八种包生态系统中生成恶意软件警报：npm、PyPI、Maven、RubyGems、NuGet、Go、crates.io 和 PHP Composer。
- GitHub Advisory Database 通过新的导入器接收 OpenSSF malicious-packages 仓库的恶意软件报告，并在发布前验证 OSV 记录。
- 恶意软件警报为选择启用，启用时会根据现有公告进行回填。
- 导入管道包含批次上限、到上游提交的溯源追踪以及回滚机制，以缓解上游不良数据的影响。
