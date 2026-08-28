---
decisionKey: "ee2b749883519114682ac4d5f3f81d3bd3db2780daed4267acdfa78aad82b7c2"
language: "zh-CN"
title: "Uber 构建 GitFarm，将 Git 操作作为服务运行以支持大规模 Monorepo"
summary: "Uber 开发了 GitFarm，将 Git 操作集中到后端集群，消除了客户端本地克隆的需求，并显著减少了大型 monorepo 的冷启动时间。"
publishedAt: "2026-08-28T21:50:05.617Z"
score: 0.85
topics:
  - "Git Infrastructure"
  - "Monorepo"
  - "Uber Engineering"
topicIds:
  - "git-infrastructure-1a46aiq"
  - "monorepo-17t0ptq"
  - "uber-engineering-1rropw2"
sourceUrls:
  - "https://www.infoq.com/news/2026/08/uber-gitfarm-git-as-a-service/"
---

- GitFarm 是一个 Git as a Service 平台，集中执行 Git 操作，客户端无需维护本地仓库克隆。
- 它提供完整的 Git checkout，耗时不到 500 毫秒，而以前冷启动大型 monorepo（如 Go monorepo）需要 10 到 15 分钟。
- 它利用预热的 checkout 和沙盒池，将提供可用 checkout 的开销降至不到一秒。
- Uber 的一个代码所有权服务采用 GitFarm 后，取消了六个主机上的本地 checkout，CPU 从超过 70 核降至 16 核，内存从 400 GB 降至 32 GB，启动时间从 15-20 分钟降至不到 1 分钟。（这些指标来自 Uber 的自述，未经独立验证。）
- 一个合规审计服务处理 9,000 个仓库中每小时 10,000 至 20,000 个事件，使用 GitFarm 后，中位延迟从使用 Buildkite 时的 110-160 秒降至 20-30 秒。（这些指标来自 Uber 的自述，未经独立验证。）
- GitFarm 自 2025 年初投入生产，其路线图包括流式 Git 输出、稀疏 checkout、裸工作区、更长时间的会话、仓库镜像以及 SubmitQueue 集成。
