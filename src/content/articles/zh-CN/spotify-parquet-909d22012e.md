---
decisionKey: "909d22012ee9e441ffb80d28b9d4483796366b795abb82ca9dbdc9553b389ed2"
language: "zh-CN"
title: "Spotify 推出随机访问 Parquet 架构，实现数据湖上的低延迟点查询"
summary: "Spotify 引入了 Random Access Parquet (RAP) 存储架构，使得点查询能够直接在数据湖上执行，而无需复制数据。该架构在保留分析功能的同时提升了查询性能。"
publishedAt: "2026-08-12T15:30:42.918Z"
score: 0.85
topics:
  - "Data Engineering"
  - "Data Lake"
  - "Apache Iceberg"
topicIds:
  - "data-engineering-cqrk2u"
  - "data-lake-18bx0pw"
  - "apache-iceberg-h1oyqe"
sourceUrls:
  - "https://www.infoq.com/news/2026/08/spotify-data-lake-point-queries/"
---

- Spotify 推出了 Random Access Parquet (RAP)，一种存储架构，无需复制到操作型数据库即可直接对数据湖中的数据进行低延迟点查询。
- RAP 在 Apache Parquet 文件之上增加了一个外部索引层，支持交互式查找，同时保持分析和 AI 兼容性。
- 索引将查找键直接映射到 Parquet 文件和行位置，避免全表扫描，支持针对性的范围读取。
- 当新数据写入 Iceberg 表时，索引构建器会生成追加式索引片段，不改动不可变的 Parquet 文件。
- 存储布局优化包括按查找键排序、对相关记录分组、交错排布值列以及覆盖索引，使某些点查询通过一次仅几 KB 的范围读取即可完成。
- RAP 支持多个查找维度的二级索引，例如买家 ID 或卖家 ID，其中哈希索引用于精确查找，排序索引用于范围查询。
