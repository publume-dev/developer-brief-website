---
decisionKey: "de89c42122a9b80d5bbe4a94f95b62de0a79d4f9149789cc1fbc8461f92d266b"
language: "zh-CN"
title: "Canva 分享基于 S3 的会话撤销架构：支撑数亿活跃会话"
summary: "Canva 将会话撤销记录改为存放在 Amazon S3 的紧凑不可变记录，并分发到应用网关内存索引，覆盖数亿活跃会话，使撤销缓存内存占用减少 87.5%。"
publishedAt: "2026-08-11T15:30:50.566Z"
score: 0.9
topics:
  - "Session Management"
  - "Amazon S3"
  - "Authentication Infrastructure"
topicIds:
  - "session-management-1pt6b6u"
  - "amazon-s3-14p3lpp"
  - "authentication-infrastructure-35y6a0"
sourceUrls:
  - "https://www.infoq.com/news/2026/08/canva-session-revocation-scale/"
---

- Canva 重新设计了会话撤销机制：将紧凑的不可变撤销记录存放在 Amazon S3，并作为内存索引分发到应用网关，支撑数亿活跃会话。
- 撤销数据按 30 分钟的 S3 对象划分，表示 12 小时窗口；每条撤销是包含主体（principal）和时间戳的 16 字节二进制记录，排序数组支持直接内存搜索，使撤销缓存内存占用减少 87.5%。
- 网关使用条件 GET 下载变更的块，并丢弃超过 12 小时的数据；异步 worker 将新撤销合并到最新块，并用条件 PUT 实现乐观并发控制，ZooKeeper 领导者选举可减少冲突，但不是正确性所必需的。
- 迁移后，Canva 将会话撤销数据库缩减为两个只读副本用于冗余，部署速度提升，数据库负载随撤销写入吞吐量和站点流量扩展，而不是随加载缓存的网关实例数量扩展。
- Canva 报告该 worker 每秒可处理超过 2000 条撤销；包含 100 万条撤销的块约占 16 MB 二进制数据。
