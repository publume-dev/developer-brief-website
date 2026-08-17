---
decisionKey: "ec3fe961f89fd5beff499d8d667bf8dbdfb1c42e41c412b8f9d116667c5742c6"
language: "zh-CN"
title: "AWS 开源 Dogwood，将 Cedar 扩展到代理工具调用序列的策略治理"
summary: "AWS 开源了 Dogwood，这是一种扩展 Cedar 的策略语言，用于管理代理工具调用序列，增加了对事件历史的时间条件支持。"
publishedAt: "2026-08-17T03:15:51.896Z"
score: 0.85
topics:
  - "Agent Policy"
  - "Open Source"
  - "Authorization"
topicIds:
  - "agent-policy-jts638"
  - "open-source-17ixijy"
  - "authorization-14ahghq"
sourceUrls:
  - "https://www.infoq.com/news/2026/08/aws-dogwood-agent-policy/"
---

- AWS 以 Apache 2.0 许可证开源了 Dogwood，这是一种针对代理工具调用的策略语言，扩展了 Cedar，增加了时间条件。
- Dogwood 增加了第二种子句类型，其中条件可以使用 `when temporal` 来读取代理的事件历史。
- 时间条件被转换为 Cedar 上下文字段，支持四种运算符：`formerly`、`count_within`、`count_distinct_within` 和 `sum_within`。
- AWS 警告，基于响应事件的速率限制可能会因并发而失效，建议使用基于请求事件的策略。
- 时间条件不支持 Cedar 的自动化推理分析工具，并且评估时间取决于事件日志的长度。
- Dogwood 向后兼容：任何有效的 Cedar 策略也是有效的 Dogwood 策略。
- 参考解释器仅用于探索和测试，不适用于生产授权。

时间条件的限制意味着依赖自动化推理的现有 Cedar 工作流需要调整。

未来路线图项目，如绝对时间窗口和活性属性，尚未实现，缺乏细节。
