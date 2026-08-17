---
decisionKey: "13f51ca3d2076add225191bc8cdbd49b96e969f83780a9e02fc759e10c8c6390"
language: "zh-CN"
title: "AWS 为 DynamoDB 引入原生向量搜索，支持高达 4096 维"
summary: "AWS 现已为 DynamoDB 提供原生向量搜索，允许存储嵌入并利用新的 SearchVectors API 执行近似最近邻查询。该功能支持高达 4096 维的向量索引、多种距离函数以及内联过滤。"
publishedAt: "2026-08-17T03:15:51.896Z"
score: 0.9
topics:
  - "DynamoDB"
  - "Vector Search"
  - "AWS"
topicIds:
  - "dynamodb-uk7cqh"
  - "vector-search-1d59ekm"
  - "aws-7brv06"
sourceUrls:
  - "https://www.infoq.com/news/2026/08/aws-dynamodb-vector-search/"
---

- DynamoDB 现已支持原生向量搜索，允许存储嵌入并使用新的 SearchVectors API 执行近似最近邻查询。
- 向量索引支持高达 4096 维，并支持欧几里得、余弦和点积距离函数，且支持内联过滤。
- 向量索引的定价基于写入的数据、搜索期间处理的数据以及存储的数据，均按字节计量并按 GB 计费，此外还需支付标准的 DynamoDB 费用。

报告提及未来将通过 ExtendDB 适配器提供对本地开发和自托管部署的支持，但具体细节尚未提供。
