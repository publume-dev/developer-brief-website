---
decisionKey: "7b6f139d532b8d537118173822534f51e4cd5725027cead8520db72d64d3cf8a"
language: "zh-CN"
title: "Netflix 将 Service Topology 管线拆为三阶段，加入 Kafka 背压与 SSE"
summary: "InfoQ 的一篇工程报道描述了 Netflix 如何重构 Service Topology 管线，以应对单实例负载严重不均的问题：解析与富化/持久化分离，并加入用暂停消费者替代丢弃记录的背压机制。"
publishedAt: "2026-08-11T15:30:50.566Z"
score: 0.85
topics:
  - "Streaming Systems"
  - "Backpressure"
  - "Service Topology"
  - "Production Engineering"
topicIds:
  - "streaming-systems-1d7vv7t"
  - "backpressure-1bb9jwd"
  - "service-topology-7j6cjl"
  - "production-engineering-3l0qal"
sourceUrls:
  - "https://www.infoq.com/news/2026/08/netflix-service-topology/"
---

- 据 InfoQ 报道，新管线分三个阶段：先做中间层解析，再做富化，最后持久化。
- 背压从图存储一路传回 Kafka；写入变慢时消费者会被暂停，不会丢弃记录。
- 阶段间的高容量内部传输从 gRPC 改为服务器发送事件（SSE）。
- 处理集群用共享服务注册表上的一致性哈希分配负载，实例加入或退出只会影响对应聚合器，无需单独再平衡流程。
- 为支持按时间点查询，Service Topology 保存分时间窗口的聚合器快照和属性级变更历史，可以在指定时间重建拓扑。
- 旧设计中，热门目标会让部分实例收到高达常规流量 100 倍的请求，同时这些实例还要做 I/O 密集的富化工作。
