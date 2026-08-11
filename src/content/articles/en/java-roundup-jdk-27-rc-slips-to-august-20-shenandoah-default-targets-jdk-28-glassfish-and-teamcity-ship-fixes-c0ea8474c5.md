---
decisionKey: "c0ea8474c59f22c1b5673617336699a3f6c414ee282b4f81e20a49a2ab151221"
language: "en"
title: "Java Roundup: JDK 27 RC Slips to August 20, Shenandoah Default Targets JDK 28, GlassFish and TeamCity Ship Fixes"
summary: "InfoQ's Java roundup covers scheduling and roadmap changes for JDK 27/28, security fixes for GlassFish and TeamCity, and new capabilities in Gradle, Camel, A2A SDK, and Grails; the TeamCity fix follows active exploitation."
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

- InfoQ's roundup reports OpenJDK JEP 535 targets JDK 28 for Shenandoah GC's generational mode by default; non-generational mode is deprecated with intent to remove.
- JDK 27's initial release candidate moves from August 6 to August 20, 2026, aligning with the August 18, 2026 CPU.
- GlassFish 8.0.4 fixes CVE-2026-59889, CVE-2026-54515 (Jackson Databind deserialization), and CVE-2026-12605 (leaked gfresttoken); the report is ambiguous on whether the latter takeover is unauthenticated or requires Admin Console authentication.
- TeamCity CVE-2026-63077 is under active exploitation; fixes ship in 2025.11.7 and 2026.1.3, with a patch plugin for 2017.1+.
- Gradle 9.7.0 moves Isolated Projects from experimental to incubating and improves Configuration Cache.
- Apache Camel 4.22.0 adds camel-ai-tool and camel-mcp-server for AI and MCP integrations.
- A2A Java SDK 1.2.0 adds TaskStreamLifecycleHook and StreamCloseHandle for observing task stream lifecycles.
- Apache Grails 8.0.0 milestone 5 refactors GlobalGrailsClassInjectorTransformation and expands deepSanitize() support.
