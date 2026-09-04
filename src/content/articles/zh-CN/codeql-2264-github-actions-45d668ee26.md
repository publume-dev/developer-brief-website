---
decisionKey: "45d668ee262b4904e579b295a0258c6c91c0f32beddd200912043d7a7b72821f"
language: "zh-CN"
title: "CodeQL 2.26.4 改进 GitHub Actions 安全检测"
summary: "CodeQL 2.26.4 增加了对 Go 1.27 的支持，并增强了多个语言的安全检测和查询精度。此次更新还包括对 GitHub Actions 工作流的更准确检查，可能产生更多警报。"
publishedAt: "2026-09-04T12:05:05.180Z"
score: 0.85
topics:
  - "CodeQL"
  - "Static Analysis"
  - "GitHub Actions"
  - "Security"
  - "Go"
  - "Rust"
  - "C#"
  - "Java"
  - "Kotlin"
topicIds:
  - "codeql-crqmh5"
  - "static-analysis-14v4mof"
  - "github-actions-7tcwgt"
  - "security-1jtharf"
  - "go-iciszv"
  - "rust-845rdz"
  - "c-15ny19f"
  - "java-295ahx"
  - "kotlin-17pq86k"
sourceUrls:
  - "https://github.blog/changelog/2026-09-03-codeql-2-26-4-improves-github-actions-security-detections"
---

- 新增对 Go 1.27 的支持。
- Rust 数据流查询现在根据实际源和汇节点报告更精确的警报位置，部分警报会显示为新警报，同时关闭旧警报。
- Java/Kotlin：为 Spring R2DBC DatabaseClient 和 R2DBC SPI 添加了 SQL 注入汇模型。
- 当参数为 CharSequence 时，污点现在通过 String.valueOf(Object) 调用传播。
- JavaScript/TypeScript：添加了对使用 d 标志的正则表达式和 React Native Worklets 'worklet' 指令的支持。
- Python：通过 list.extend 和 list.insert 添加了污点流，与现有的 list.append 污点流一致。
- C#：cs/web/missing-token-validation 查询现在能识别启用的 ASP.NET Core RequireAntiforgeryToken 属性，当使用防伪中间件时。
- 在 build-mode: none 数据库中，cs/useless-cast-to-self 和 cs/simplifiable-boolean-expression 查询产生更少的误报。
- GitHub Actions：从事件负载读取的执行者字段的检查现在仅对实际填充该字段的事件视为保护，可能导致使用 ControlCheck 类的查询产生更多警报。
- actions/unpinned-tag 查询现在能检测对可复用工作流的可变引用。
- 现在可以通过 models-as-data 模型指定 EnvironmentCheck。
- 当环境不再是足够的消毒剂时，使用 ControlCheck 的查询可能发现更多结果。

由于 Rust 警报位置的变化，现有警报可能会被重新分类或关闭，用户应重新运行扫描以查看更新后的警报。

需要关注 GitHub Actions 中事件字段填充的详细行为，以了解 actor 检查的具体影响。
