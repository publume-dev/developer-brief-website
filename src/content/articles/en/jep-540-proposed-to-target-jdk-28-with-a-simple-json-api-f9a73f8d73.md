---
decisionKey: "f9a73f8d73765ca9dccebf10e057ec1118bc7f7ad2ca1bfe80f35b8c27ed4737"
language: "en"
title: "JEP 540 Proposed to Target JDK 28 with a Simple JSON API"
summary: "JEP 540 has reached Proposed to Target, aiming to add a simple JSON API to JDK 28. The incubator module will enforce strict JSON syntax, rejecting duplicates and other extensions."
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

- JEP 540 for a Simple JSON API has moved from Candidate to Proposed to Target for JDK 28, and would ship in the incubating jdk.incubator.json module.
- The API centers on the Json class and the sealed JsonValue interface, with immutable and thread-safe instances.
- The API rejects duplicate object-member names and other syntax extensions like comments and trailing commas by design.
- Class-path applications will need to resolve the incubator module with --add-modules jdk.incubator.json.
