---
decisionKey: "d2f44921cdd6a88faec3127b3ad9d4294bf4d72e4ba002f6537372df2138db06"
language: "en"
title: "Java Roundup: GraalVM, Quarkus, WildFly, and More"
summary: "This week's Java ecosystem updates include GraalVM performance and security improvements, Quarkus post-quantum cryptography support, WildFly SSRF mitigation, and Open Liberty's MCP support with a breaking change."
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

- GlassFish 8.0.4 Docker images are now available from OmniFish for GlassFish and GlassFish Embedded.
- GraalVM 25.3 introduces a new SubstratePriorityInliningPhase class for improved JIT and Native Image performance, plus security hardening against execution redirection attacks.
- Quarkus 3.39.0 adds post-quantum cryptography support in the TLS Certificate Registry extension and reverses reflection-free Jackson serializers to be non-default.
- WildFly 41.0.1 updates its serialization filter with a new deny list per JEP 290 and upgrades Apache CXF to block decoupled destinations, mitigating SSRF attacks.
- Open Liberty 26.0.0.9-beta adds support for the MCP Java API in the mcpServer-1.0 feature, but updates MCP metrics MBean names to use own JMX ObjectName keys, a breaking change for JMX queries or scripts.
