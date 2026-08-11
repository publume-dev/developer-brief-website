---
decisionKey: "7b6f139d532b8d537118173822534f51e4cd5725027cead8520db72d64d3cf8a"
language: "en"
title: "Netflix Splits Service Topology Pipeline Into Three Stages, Adds Kafka Backpressure and SSE"
summary: "An InfoQ engineering report describes how Netflix redesigned its Service Topology pipeline to address severe per-instance load imbalance, separating resolution from enrichment and persistence and adding backpressure that pauses consumers rather than dropping records."
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

- According to InfoQ, the pipeline now runs in three stages: intermediary resolution, enrichment, then persistence.
- Backpressure travels from graph storage back to Kafka; when writes slow, consumers pause rather than drop records.
- For high-volume transfers between stages, Netflix swapped gRPC for server-sent events (SSE).
- The processing fleet relies on consistent hashing against a shared service registry, so instance joins or leaves only affect the matching aggregators, with no separate rebalancing step.
- For point-in-time queries, Service Topology keeps time-windowed aggregator snapshots and property-level mutation history, enabling topology reconstruction at a specified time.
- In the earlier design, popular destinations caused some instances to receive up to 100 times typical traffic while also doing I/O-heavy enrichment work.
