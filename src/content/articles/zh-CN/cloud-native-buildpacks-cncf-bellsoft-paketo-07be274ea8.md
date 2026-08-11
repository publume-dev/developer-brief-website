---
decisionKey: "07be274ea8a7d5c8a9929e5c0b639b06b379f4a36341b4f515a9ba9c02447e96"
language: "zh-CN"
title: "Cloud Native Buildpacks 在 CNCF 毕业，BellSoft 发布加固版 Paketo 构建器"
summary: "Cloud Native Buildpacks 于 2026 年 7 月 17 日在 CNCF 毕业；7 月 21 日，BellSoft 宣布其基于 Alpaquita Linux 的加固版 Paketo 构建器正式可用，让团队无需完整重建即可通过 rebase 更新运行时基础镜像。"
publishedAt: "2026-08-11T18:42:58.614Z"
score: 0.8
topics:
  - "Container Security"
  - "Cloud Native Buildpacks"
  - "Supply Chain Security"
topicIds:
  - "container-security-1ffi472"
  - "cloud-native-buildpacks-uz45a1"
  - "supply-chain-security-1fqvp23"
sourceUrls:
  - "https://www.infoq.com/news/2026/08/buildpacks-dockerfile-patching/"
---

- Cloud Native Buildpacks 于 2026 年 7 月 17 日在 CNCF 内毕业。
- 2026 年 7 月 21 日，BellSoft 宣布基于 Alpaquita Linux 的加固版 Paketo 构建器正式可用。
- rebase 命令通过重写 OCI manifest 和配置，将应用镜像更新到更新的运行时基础镜像，从而绕过重建。
- rebase 只替换兼容的 run-image 层；应用依赖中的漏洞仍需要重建。
- BellSoft 的 Standard 层级宣称对严重漏洞提供 7 天修复 SLA，对其他漏洞提供 14 天；免费 Community 层级没有列出 SLA。
- 2025 年 12 月，Docker 以 Apache 2.0 协议免费提供其加固镜像目录，Select 层级承诺对严重 CVE 进行 7 天修复。
