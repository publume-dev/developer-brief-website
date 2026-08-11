---
decisionKey: "d11dfac7db748f69f6c3d605ea2a0b0e1695515c8bc382b6bafb01f21a81a7fc"
language: "en"
title: "JDK 28 Integrates JEP 401: Value Objects Preview Redefines =="
summary: "JEP 401 (Value Objects Preview) is integrated into JDK 28, giving value-class instances no object identity and making `==` compare field values; the preview is off by default and requires `--enable-preview` at compile and run time."
publishedAt: "2026-08-11T15:30:50.566Z"
score: 0.9
topics:
  - "Java"
  - "JDK 28"
  - "Project Valhalla"
  - "Value Objects"
topicIds:
  - "java-295ahx"
  - "jdk-28-zlpqu2"
  - "project-valhalla-14tp945"
  - "value-objects-ssz43u"
sourceUrls:
  - "https://www.infoq.com/news/2026/08/jep401-value-objects-preview/"
---

- JEP 401 (Value Objects Preview) is integrated into JDK 28. The preview is off by default; compilation and run time both require `--enable-preview`.
- A class declared with the `value` modifier becomes a value class: instance fields are implicitly final, and every field must be assigned before the new instance is observed. Records can use the modifier too, e.g., `value record Color(byte red, byte green, byte blue)`.
- For value objects, `==` returns true when both operands are instances of the same value class with equal field values; reference-typed fields are compared recursively with `==`. `String` stays an identity class, and JEP 401 does not replace `equals`.
- With preview enabled, several value-based JDK classes, including primitive wrappers and `LocalDate`, become value classes. Code compiled with preview enabled must run with it enabled, and recompilation is recommended for migrated classes because `LoadableDescriptors` tells the JVM at load time that a class is a value class.
- Some APIs stop working: creating a `Reference` to a value object throws `IdentityException`, and in JDK 28 `javac` extends its identity warnings to value classes.
- The JVM may scalarize or flatten value objects into compact representations, but flattening is constrained by atomicity (often 64 bits including a null flag) and falls back to ordinary allocation during warmup. Security considerations: `==` and `identityHashCode` can expose private field values, and comparing large trees of value objects may take unbounded time.
