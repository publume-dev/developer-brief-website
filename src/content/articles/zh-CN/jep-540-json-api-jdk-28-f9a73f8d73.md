---
decisionKey: "f9a73f8d73765ca9dccebf10e057ec1118bc7f7ad2ca1bfe80f35b8c27ed4737"
language: "zh-CN"
title: "JEP 540 提议将简单 JSON API 纳入 JDK 28"
summary: "JEP 540 已进入 Proposed to Target 阶段，计划在 JDK 28 中引入一个简单的 JSON API。该 API 将通过 incubator 模块提供，强调严格的 JSON 语法，并拒绝重复键等扩展。"
publishedAt: "2026-08-18T03:10:40.287Z"
score: 0.85
topics:
  - "JDK"
  - "Java"
  - "JSON API"
topicIds:
  - "jdk-1pug780"
  - "java-295ahx"
  - "json-api-17ylx2r"
sourceUrls:
  - "https://www.infoq.com/news/2026/08/java-native-json-api/"
---

- JEP 540 的 Simple JSON API 状态从 Candidate 变为 Proposed to Target，面向 JDK 28，并计划在 jdk.incubator.json 孵化模块中提供。
- API 核心是 Json 类和 sealed 接口 JsonValue，其实例不可变且线程安全。
- API 设计上拒绝重复的对象成员名、注释和尾随逗号等语法扩展。
- 对于类路径应用程序，需要使用 --add-modules jdk.incubator.json 来解析孵化模块。
