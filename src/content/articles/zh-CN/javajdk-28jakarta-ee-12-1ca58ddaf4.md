---
decisionKey: "1ca58ddaf43cce8d1a11d8731704e896b947341f5e54ea2c825fb6aaf0dfc53b"
language: "zh-CN"
title: "Java生态周报：JDK 28新提案、Jakarta EE 12进展及多项工具更新"
summary: "本周Java生态迎来多项更新：JDK 28的Simple JSON API提案进入Target状态，Jakarta EE 12多个规范推进，GlassFish、GraalVM、Open Liberty等工具发布新版本，修复了安全漏洞并带来新功能。"
publishedAt: "2026-08-17T03:15:51.896Z"
score: 0.82
topics:
  - "Java"
  - "JDK"
  - "Jakarta EE"
  - "GlassFish"
  - "GraalVM"
  - "NoSQL"
  - "Open Liberty"
  - "LangChain4j"
  - "Groovy"
topicIds:
  - "java-295ahx"
  - "jdk-1pug780"
  - "jakarta-ee-ce5u99"
  - "glassfish-29ugah"
  - "graalvm-1971dfv"
  - "nosql-jtymsm"
  - "open-liberty-1ll92cu"
  - "langchain4j-1y1hg2c"
  - "groovy-klgetr"
sourceUrls:
  - "https://www.infoq.com/news/2026/08/java-news-roundup-aug10-2026/"
---

- JEP 540（Simple JSON API，孵化器）已从Candidate提升至Proposed to Target，面向JDK 28，定义符合RFC 8259的JSON解析与生成标准API。
- JEP 541（弃用macOS/x64端口）已从Candidate提升至Proposed to Target，面向JDK 28，评审预计于2026年8月21日（周五）结束。
- Jakarta EE 12规范进展：CDI 5.0进入发布评审，JSON Binding 3.1发布M1并推进M2，JSON Processing 2.2计划很快发布M1，RESTful Web Services 5.0等待PR #1340的必要+1。
- GlassFish 9.0.0-M3完整实现Jakarta Security 5.0-M2、Jakarta Faces 5.0-M5和CDI 5.0-RC1，部分实现Jakarta Servlet 6.2-M2，并初步支持Jakarta Concurrency 3.2-M3。
- GraalVM Native Build Tools 1.1.9默认输出简洁的仓库测试结果，将单元测试与native-maven-plugin及远程bootstrap任务解耦，并将Native Image层升级为共享模型，优先支持Gradle和Maven。
- Eclipse JNoSQL 1.1.16新增对Valkey键值数据存储的支持，改进Oracle NoSQL集成，并更新了MongoDB、DynamoDB、Couchbase、OrientDB和Elasticsearch的驱动。
- Open Liberty 26.0.0.8修复多个拒绝服务漏洞，包括CVE-2026-50645、CVE-2026-9171和CVE-2026-15057，官方建议开发者升级。
- LangChain4j 1.19.0（第29个beta）新增AnthropicBatchChatModel，实现Anthropic Message Batches API，并在attributes()方法中支持映射MCP服务器的_meta。
- Apache Groovy 6.0.0-beta-2新增对JEP 371隐藏类的支持，DefaultGroovyMethods新增findingResults(Iterator)方法，并新增GeneratedDispatcher接口用于原生镜像中的Packed Closures。
