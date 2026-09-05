---
decisionKey: "23e6dcb18860ce16812b5914d4a731362b33ea00ebf5a9338b639e6371f5c2c0"
language: "en"
title: "GitHub CLI Linux package signing key expires September 5, 2026"
summary: "GitHub announced that the current PGP key for the GitHub CLI Linux package repositories expires on September 5, 2026, after which the replacement key will be used for signing. APT and RPM users need to update their trust configuration before the deadline to avoid repository metadata verification failures."
publishedAt: "2026-09-05T12:04:28.250Z"
score: 0.85
topics:
  - "GitHub CLI"
  - "Linux Package Signing Key"
  - "Security Update"
topicIds:
  - "github-cli-1vmpf8w"
  - "linux-package-signing-key-2dstrl"
  - "security-update-dksnls"
sourceUrls:
  - "https://github.blog/changelog/2026-09-03-github-cli-linux-package-signing-key-expires-september-5"
---

- The current PGP key for the GitHub CLI Linux package repositories expires on Saturday, September 5, 2026.
- After that date, APT and RPM repository metadata and newly published RPM packages will be signed only with the replacement key.
- Users who installed gh from the official APT or RPM repositories before April 8, 2026, and have not updated the setup since, must follow the announcement instructions before September 5 to trust the replacement key.
- Users who installed after that date, do not remember installation details, or use custom images or automation paths should verify their system trusts the replacement key following the announcement.
