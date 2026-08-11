---
decisionKey: "d11dfac7db748f69f6c3d605ea2a0b0e1695515c8bc382b6bafb01f21a81a7fc"
language: "zh-CN"
title: "JDK 28 集成 JEP 401：值对象预览让 == 按字段值比较"
summary: "JEP 401（值对象预览）已集成到 JDK 28，值类实例不再具备对象标识，`==` 改为按字段值比较；预览默认关闭，编译和运行时都需启用 `--enable-preview`。"
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

- JEP 401（值对象预览）已集成到 JDK 28；预览默认关闭，编译和运行都需传 `--enable-preview`。
- 使用 `value` 修饰符声明的类即为值类：实例字段隐式为 final，且新实例被观察到之前必须完成所有字段赋值；记录也可加该修饰符，例如 `value record Color(byte red, byte green, byte blue)`。
- 值对象的 `==` 在两个操作数是同一个值类的实例且字段值相同时返回 true，引用类型字段用 `==` 递归比较；`String` 仍是标识类，JEP 401 不取代 `equals`。
- 启用预览后，包括基本类型包装类和 `LocalDate` 在内的多个基于值的 JDK 类变为值类；用预览编译的代码必须在启用预览的运行时执行，迁移后的类建议重新编译，因为 `LoadableDescriptors` 类文件属性会在加载时告知 JVM 某个类是值类。
- 部分 API 不再适用于值对象：为值对象创建 `Reference` 会抛出 `IdentityException`；JDK 28 中 `javac` 还会把标识警告扩展到值类。
- JVM 可将值对象标量化或扁平化为紧凑表示，但扁平化受原子性限制（通常小至含 null 标志的 64 位），并在预热期间回退为普通分配。安全方面：`==` 和 `identityHashCode` 可能暴露私有字段值，比较大型值对象树可能消耗无界时间。
