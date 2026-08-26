---
decisionKey: "eeffff7ba06763e17b2ca66b251fb556b0ececd11054f2a39f4972040ae03a47"
language: "zh-CN"
title: "Java 简报：JDK 27 进入 RC、JDK 28 新增 JEP、BellSoft 安全补丁、Apache Tika 4.0 GA 等"
summary: "JDK 27 已进入 RC 阶段，GA 定于 2026 年 9 月 15 日；JDK 28 新增多个 JEP，包括簡單 JSON API 和弃用 macOS/x64；BellSoft 发布多个版本的安全补丁；Apache Tika 4.0 带来破坏性变更。"
publishedAt: "2026-08-26T14:25:19.922Z"
score: 0.82
topics:
  - "Java"
  - "Release"
  - "Security Patch"
  - "Deprecation"
  - "JSON API"
  - "Apache Tika"
  - "Helidon"
  - "Micrometer"
topicIds:
  - "java-295ahx"
  - "release-4hyb9a"
  - "security-patch-1vamxc5"
  - "deprecation-ywavad"
  - "json-api-17ylx2r"
  - "apache-tika-wc4n1y"
  - "helidon-l65afi"
  - "micrometer-1in0scg"
sourceUrls:
  - "https://www.infoq.com/news/2026/08/java-news-roundup-aug17-2026/"
---

- JDK 27 已发布首个候选版本（Build 35），无未解决的 P1 缺陷，预计于 2026 年 9 月 15 日发布 GA，包含 9 个 JEP。
- JDK 28 新增目标 JEP：JEP 541（弃用 macOS/x64 移植）和 JEP 540（简单 JSON API 孵化器）。
- BellSoft 发布 Liberica JDK 补丁，涵盖 26.0.2.1、25.0.4.1、21.0.12.1、17.0.20.1、11.0.32.1、8u504、7u513 和 6u513，修复 29 个 CVE。
- Apache Tika 4.0.0 GA 引入新的 MarkdownParser，以及用于 Claude、Gemini、OpenAI 和 Tesseract 的推理和 OCR 模块；同时包括分叉进程解析和 JSON 配置等破坏性变更。
- Helidon 4.5.3 维护版为 LRA 参与者回调添加了必需的配置属性，并设置了嵌套 JSON 结构的 1000 层限制。
- Micrometer Metrics 1.18.0-M1 优化了 PrometheusMeterRegistry 和 MicrometerCollector，Tracing 1.8.0-M1 重构了 W3CPropagation 以提升安全性。
