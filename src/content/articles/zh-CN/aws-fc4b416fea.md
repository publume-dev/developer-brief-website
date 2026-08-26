---
decisionKey: "fc4b416fea24781091dfd7a43436c65b22b1a6a3325189cf5a2901d53600e127"
language: "zh-CN"
title: "AWS 引入规范驱动的组合模式，用于灵活的数据工作流"
summary: "AWS 推出了一种规范驱动的组合模式，通过将工作流意图与处理逻辑分离，减少重复的管道代码并简化验证与治理。该模式适用于监管报告、多源集成和可复用的 ETL 工作流。"
publishedAt: "2026-08-26T14:25:19.922Z"
score: 0.84
topics:
  - "AWS"
  - "Data Engineering"
  - "Software Architecture"
topicIds:
  - "aws-7brv06"
  - "data-engineering-cqrk2u"
  - "software-architecture-1lxq17v"
sourceUrls:
  - "https://www.infoq.com/news/2026/08/aws-spec-driven-data-workflow/"
---

- AWS 引入了规范驱动的组合模式，将工作流意图与处理逻辑分离，以减少重复管道代码并简化验证与治理。
- 该模式包含三层：意图层（规范）、组合层（验证规范并组装管道）、处理层（执行转换步骤）。
- 无服务器实现使用 AWS Lambda、AWS Step Functions、Amazon S3 和 Amazon OpenSearch Service，规范存储于 S3，能力元数据存储于 OpenSearch。
- 该模式支持能力发现、版本化的能力引用以保证可重现性，并可纳入数据分类以进行敏感度标记和脱敏。
- 该模式适用于监管报告、多源集成和可复用的 ETL 工作流，但对于简单转换或少量工作流则无必要。
