---
decisionKey: "23e6dcb18860ce16812b5914d4a731362b33ea00ebf5a9338b639e6371f5c2c0"
language: "zh-CN"
title: "GitHub CLI Linux 软件包签名密钥将于 2026 年 9 月 5 日到期"
summary: "GitHub 官方公告，当前用于 GitHub CLI Linux 软件包仓库的 PGP 密钥将于 2026 年 9 月 5 日到期，之后将使用替换密钥进行签名。APT 和 RPM 用户需要在截止日期前更新信任配置，以避免仓库元数据验证失败。"
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

- 当前 GitHub CLI Linux 软件包仓库使用的 PGP 密钥将于 2026 年 9 月 5 日（星期六）到期。
- 自该日期起，APT 和 RPM 仓库的元数据以及新发布的 RPM 软件包将仅使用替换密钥签名。
- 在 2026 年 4 月 8 日之前从官方 APT 或 RPM 仓库安装 gh 且未更新设置的用户，必须在 9 月 5 日前按照公告中的步骤操作，以信任替换密钥。
- 在该日期之后安装、或不确定安装详情、或使用自定义镜像或自动化流程的用户，应按照公告验证其系统信任替换密钥。
