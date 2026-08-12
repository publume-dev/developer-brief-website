---
decisionKey: "b7a85a093382619f217f9dc3a9f85a5a10f4cca2416078640e8ca3817b7eeb77"
language: "en"
title: "Netflix Adopts Cloud-Native Job Queueing System Kueue to Replace an In-House Solution"
summary: "Netflix is migrating its batch workloads to the open-source cloud-native system Kueue, replacing its in-house Compute Managed Batch (CMB), and is already managing millions of production jobs."
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

- Netflix migrated most of its batch workloads onto Kueue, an open-source cloud-native batch job execution system, replacing its in-house Compute Managed Batch (CMB) solution.
- Engineers mapped CMB's capabilities to Kueue, using API parity to derisk the migration and enable a gradual, seamless transition for existing users.
- Netflix is currently managing millions of batch workloads in production using Kueue, with the migration still underway.
- The migration team improved average resource utilization by leveraging preemption-based fair sharing to maintain reservation semantics while lending idle capacity to other tenants.
- The production migration lasted only 4 weeks, attributed to migrating the largest and most complex customer first, maintaining API parity, and running load tests in the non-prod environment.
