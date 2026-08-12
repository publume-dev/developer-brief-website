---
decisionKey: "b7a85a093382619f217f9dc3a9f85a5a10f4cca2416078640e8ca3817b7eeb77"
language: "zh-CN"
title: "Netflix 采用云原生作业队列系统 Kueue 替代自研方案"
summary: "Netflix 正将其批量作业迁移到开源云原生系统 Kueue，以替换自研的 Compute Managed Batch (CMB)，并已管理数百万生产作业。"
publishedAt: "2026-08-12T15:30:42.918Z"
score: 0.85
topics:
  - "Kubernetes"
  - "Batch Processing"
  - "Platform Engineering"
  - "Netflix"
topicIds:
  - "kubernetes-wdjqe5"
  - "batch-processing-1v95tvm"
  - "platform-engineering-uztf0l"
  - "netflix-1sq77mz"
sourceUrls:
  - "https://www.infoq.com/news/2026/08/netflix-kueue-kubernetes-batch/"
---

- Netflix 将大部分批量作业迁移到开源云原生批量作业执行系统 Kueue，替代自研的 Compute Managed Batch (CMB)。
- 工程师通过 API 对齐来降低迁移风险，实现渐进、无缝的用户过渡。
- 生产环境目前管理数百万批量作业，迁移仍在进行中。
- 利用基于抢占的公平共享，保持预留语义的同时将空闲容量借给其他租户，提高了平均资源利用率。
- 生产迁移仅耗时 4 周，归因于先迁移最大最复杂的客户、保持 API 对齐、以及在非生产环境进行负载测试。
