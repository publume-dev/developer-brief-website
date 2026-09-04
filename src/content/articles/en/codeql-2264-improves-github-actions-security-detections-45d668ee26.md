---
decisionKey: "45d668ee262b4904e579b295a0258c6c91c0f32beddd200912043d7a7b72821f"
language: "en"
title: "CodeQL 2.26.4 improves GitHub Actions security detections"
summary: "CodeQL 2.26.4 adds support for Go 1.27 and enhances security detections and query precision across multiple languages. The update also improves GitHub Actions workflow checks, potentially resulting in more alerts."
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

- Added support for Go 1.27.
- Rust data flow queries now report more precise alert locations based on actual source and sink nodes, causing some alerts to appear as new alerts while previous ones close.
- Java/Kotlin: Added SQL injection sink models for Spring R2DBC DatabaseClient and the R2DBC SPI.
- Taint now propagates through calls to String.valueOf(Object) when the argument is a CharSequence.
- JavaScript/TypeScript: Added support for regular expressions using the d flag and for the React Native Worklets 'worklet' directive.
- Python: Added taint flow through list.extend and list.insert, matching existing taint flow through list.append.
- C#: The cs/web/missing-token-validation query now recognizes enabled ASP.NET Core RequireAntiforgeryToken attributes when antiforgery middleware is used.
- The cs/useless-cast-to-self and cs/simplifiable-boolean-expression queries produce fewer false positives in build-mode: none databases.
- GitHub Actions: Checks on actor fields read from the event payload now only count as protection for events that actually populate that field, possibly producing more alerts for queries using the ControlCheck class.
- The actions/unpinned-tag query now detects mutable references to reusable workflows.
- You can now specify EnvironmentCheck through a models-as-data model.
- Queries using ControlCheck may find more results when an environment is no longer a sufficient sanitizer.

Due to changes in Rust alert locations, existing alerts may be reclassified or closed; users should re-run scans to see updated alerts.

Watch for detailed behavior of event field population in GitHub Actions to understand the specific impact on actor checks.
