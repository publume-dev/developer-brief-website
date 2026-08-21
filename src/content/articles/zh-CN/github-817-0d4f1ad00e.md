---
decisionKey: "0d4f1ad00e262db220e1af06239ff7c802627b76980aff7194f216da623ce330"
language: "zh-CN"
title: "GitHub 8月17日中断：根因、缓解措施与未来扩展计划"
summary: "GitHub 遭受了持续7小时47分钟的中断，影响了核心服务，起因是Central US数据中心的关键组件未能随流量峰值扩展。GitHub已实施立即缓解措施，并计划推出线性读取扩展架构。"
publishedAt: "2026-08-21T14:06:07.365Z"
score: 0.9
topics:
  - "Incident Response"
  - "Platform Reliability"
  - "Capacity Planning"
topicIds:
  - "incident-response-ld2rq6"
  - "platform-reliability-jp0p8i"
  - "capacity-planning-brpogi"
sourceUrls:
  - "https://github.blog/news-insights/company-news/the-august-17-outage-and-the-work-ahead/"
---

- 8月17日，GitHub发生7小时47分钟的中断，影响github.com、认证、Actions、API、PR、issue和Copilot。
- 根因是Central US数据中心的关键基础设施组件未能随新流量峰值扩展，导致容量压力和级联故障。
- 恢复过程包括流量重新路由、隔离受影响基础设施，并缓解Copilot服务中的客户端重试循环，该循环增加了恢复期间的流量。
- 自今年早些时候的可靠性承诺以来，GitHub已增加超过300万CPU核心、120PB高速存储和大量网络容量。
- 目前，Azure承载约58%的GitHub平台负载和一半的Git操作，而五月份仅为12%。
- GitHub的下一步目标是实现读取容量随读者数量线性扩展的架构，支持无限读取操作，首先从最大的monorepo开始逐步推出。
- 立即实施的变更包括在服务间交互中应用一致的重试限制、重试预算和可变超时，并审查低优先级CPU和内存警报。
