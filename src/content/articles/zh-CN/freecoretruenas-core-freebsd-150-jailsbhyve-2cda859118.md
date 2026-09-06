---
decisionKey: "2cda859118d954672352e3356cbbb18caa24ee107058eb50cc93b08f2a9106ff"
language: "zh-CN"
title: "FreeCORE：TrueNAS CORE 社区分支，将基础升级至 FreeBSD 15.0 并保留 Jails、bhyve 与插件"
summary: "FreeCORE 是一个新的 TrueNAS CORE 社区分支，将已弃用的 13.3 基础升级至 FreeBSD 15.0，同时保留 FreeBSD Jails、bhyve 与原生插件，为依赖这些特性的用户提供稳定的升级路径。"
publishedAt: "2026-09-06T14:38:26.492Z"
score: 0.82
topics:
  - "Storage Systems"
  - "Open Source"
  - "FreeBSD/TrueNAS"
topicIds:
  - "storage-systems-1fak6ig"
  - "open-source-17ixijy"
  - "freebsd-truenas-1y8zwx9"
sourceUrls:
  - "https://www.infoq.com/news/2026/09/freecore-truenas-fork/"
---

- FreeCORE（TrueNAS CORE 的社区分支）将 13.3 基础升级至 FreeBSD 15.0，当前稳定版本为 15.0-U1，预计后续将发布 15.1。
- 与上游转向 Linux 版 TrueNAS SCALE 不同，FreeCORE 保留了 FreeBSD Jails、原生插件和 bhyve 虚拟机，而这些已被上游 iXsystems 弃用。
- FreeCORE 提供从 TrueNAS CORE 13.3 基础到 FreeBSD 15.0 的就地升级路径。
- 该项目目前由单一维护者驱动，其在实现和审查中广泛使用 AI 编码代理。
- 社区讨论指出，OpenZFS 原生加密缺乏专门的上游维护者，因此除非必须使用原生 ZFS 加密，否则一些用户倾向于使用 Linux LUKS。

FreeCORE 的长期可行性尚未证实；它依赖单一维护者和社区支持，这对企业采用构成风险。

报告未提供指向官方 FreeCORE 项目或发布说明的直接链接；细节仅基于 InfoQ 文章，可能需从主要来源核实。
