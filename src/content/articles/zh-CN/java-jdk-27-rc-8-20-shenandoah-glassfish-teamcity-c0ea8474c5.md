---
decisionKey: "c0ea8474c59f22c1b5673617336699a3f6c414ee282b4f81e20a49a2ab151221"
language: "zh-CN"
title: "Java 要闻：JDK 27 RC 推迟至 8 月 20 日、Shenandoah 默认计划、GlassFish 与 TeamCity 修复"
summary: "InfoQ 的 Java 要闻汇总了 JDK 27/28 的时间与路线图调整、GlassFish 与 TeamCity 的安全修复，以及 Gradle、Camel、A2A SDK 和 Grails 的新能力；TeamCity 修复针对的是已被积极利用的漏洞。"
publishedAt: "2026-08-11T18:42:58.614Z"
score: 0.85
topics:
  - "Java"
  - "Security"
  - "Build Tools"
topicIds:
  - "java-295ahx"
  - "security-1jtharf"
  - "build-tools-tnqz7s"
sourceUrls:
  - "https://www.infoq.com/news/2026/08/java-news-roundup-aug03-2026/"
---

- InfoQ 的汇总显示，OpenJDK JEP 535 计划让 Shenandoah GC 的分代模式在 JDK 28 中默认启用；非分代模式已弃用并计划移除。
- JDK 27 的初始 RC 日期从 2026 年 8 月 6 日推迟到 8 月 20 日，与 8 月 18 日的 CPU 保持一致。
- GlassFish 8.0.4 修复了 CVE-2026-59889、CVE-2026-54515（Jackson Databind 反序列化）和 CVE-2026-12605（泄露的 gfresttoken）；该汇总对后者是“未认证”还是需要在 Admin Console 中认证存在歧义。
- TeamCity CVE-2026-63077 正被积极利用；修复版本为 2025.11.7 和 2026.1.3，并提供面向 2017.1+ 的补丁插件。
- Gradle 9.7.0 将 Isolated Projects 从 experimental 提升为 incubating，并改进了 Configuration Cache。
- Apache Camel 4.22.0 新增 camel-ai-tool 和 camel-mcp-server，用于 AI 和 MCP 集成。
- A2A Java SDK 1.2.0 新增 TaskStreamLifecycleHook 和 StreamCloseHandle，用于观察任务流生命周期。
- Apache Grails 8.0.0 milestone 5 重构了 GlobalGrailsClassInjectorTransformation，并扩展了 deepSanitize() 支持。
