---
decisionKey: "1ca58ddaf43cce8d1a11d8731704e896b947341f5e54ea2c825fb6aaf0dfc53b"
language: "en"
title: "Java Ecosystem Roundup: JDK 28 Proposals, Jakarta EE 12 Progress, and Tooling Updates"
summary: "This week's Java ecosystem brings multiple updates: JDK 28's Simple JSON API proposal reaches Target status, Jakarta EE 12 specifications advance, and GlassFish, GraalVM, Open Liberty, and other tools ship new releases with security fixes and new features."
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

- JEP 540 (Simple JSON API, Incubator) has been elevated from Candidate to Proposed to Target for JDK 28, defining a simple standard API for parsing and generating JSON documents per RFC 8259.
- JEP 541 (Deprecate the macOS/x64 Port for Removal) has been elevated from Candidate to Proposed to Target for JDK 28, with review expected to conclude on Friday, August 21, 2026.
- Jakarta EE 12 specifications are progressing: CDI 5.0 is up for release review, JSON Binding 3.1 has M1 with M2 in progress, JSON Processing 2.2 plans M1 shortly, and RESTful Web Services 5.0 awaits required +1s on PR #1340.
- GlassFish 9.0.0-M3 delivers full implementations of Jakarta Security 5.0-M2, Jakarta Faces 5.0-M5, and CDI 5.0-RC1, partial implementation of Jakarta Servlet 6.2-M2, and initial support for Jakarta Concurrency 3.2-M3.
- GraalVM Native Build Tools 1.1.9 ships concise repository test output by default, decouples unit tests from native-maven-plugin and remote bootstrap tasks, and promotes Native Image layers to a shared model with first-class Gradle and Maven support.
- Eclipse JNoSQL 1.1.16 adds support for Valkey key/value datastore, improves Oracle NoSQL integration, and updates drivers for MongoDB, DynamoDB, Couchbase, OrientDB, and Elasticsearch.
- Open Liberty 26.0.0.8 fixes multiple denial-of-service vulnerabilities including CVE-2026-50645, CVE-2026-9171, and CVE-2026-15057, and developers are encouraged to upgrade.
- LangChain4j 1.19.0 (with 29th beta) adds AnthropicBatchChatModel implementing the Anthropic Message Batches API and new functionality to map _meta from MCP server within attributes() method.
- Apache Groovy 6.0.0-beta-2 adds support for JEP 371 Hidden Classes, a new findingResults(Iterator) method to DefaultGroovyMethods, and a new GeneratedDispatcher interface for Packed Closures in native images.
