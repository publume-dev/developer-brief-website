---
decisionKey: "d2f44921cdd6a88faec3127b3ad9d4294bf4d72e4ba002f6537372df2138db06"
language: "zh-CN"
title: "Java 生态周报：GraalVM、Quarkus、WildFly 等发布多项更新"
summary: "本周 Java 生态多个项目发布更新，涵盖 GraalVM 性能与安全改进、Quarkus 后量子密码支持、WildFly SSRF 缓解以及 Open Liberty 的 MCP 支持与破坏性变更。"
publishedAt: "2026-08-31T12:02:47.871Z"
score: 0.8
topics:
  - "Java"
  - "GraalVM"
  - "Quarkus"
  - "WildFly"
  - "Open Liberty"
  - "GlassFish"
topicIds:
  - "java-295ahx"
  - "graalvm-1971dfv"
  - "quarkus-1qmyg6p"
  - "wildfly-7vxm4y"
  - "open-liberty-1ll92cu"
  - "glassfish-29ugah"
sourceUrls:
  - "https://www.infoq.com/news/2026/08/java-news-roundup-aug24-2026/"
---

- GlassFish 8.0.4 Docker 镜像已由 OmniFish 发布，适用于 GlassFish 和 GlassFish Embedded。
- GraalVM 25.3 引入新的 SubstratePriorityInliningPhase 类以提升 JIT 和 Native Image 性能，并加强安全防护以防执行重定向攻击。
- Quarkus 3.39.0 在 TLS 证书注册扩展中支持后量子密码学，并默认反转反射式 Jackson 序列化器（即不再默认使用）。
- WildFly 41.0.1 更新序列化过滤器，按 JEP 290 新增拒绝列表，并升级 Apache CXF 以阻止解耦目标，缓解 SSRF 攻击。
- Open Liberty 26.0.0.9-beta 在 mcpServer-1.0 功能中支持 MCP Java API，但更新了 MCP 指标 MBean 名称以使用自己的 JMX ObjectName 键，这是对 JMX 查询或脚本的破坏性变更。
