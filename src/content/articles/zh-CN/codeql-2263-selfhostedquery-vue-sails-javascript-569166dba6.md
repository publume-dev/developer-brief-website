---
decisionKey: "569166dba6c9e6490757898d4b5f73f864a465bedc44a80820cef6b442b207d0"
language: "zh-CN"
title: "CodeQL 2.26.3 移除 SelfHostedQuery 模块并新增 Vue 与 Sails 的 JavaScript 流模型"
summary: "CodeQL 2.26.3 移除了 GitHub Actions 的 SelfHostedQuery 模块，并增强了 JavaScript/TypeScript 的流模型。"
publishedAt: "2026-08-21T14:06:07.365Z"
score: 0.9
topics:
  - "CodeQL"
  - "Static Analysis"
  - "GitHub Actions"
  - "JavaScript"
topicIds:
  - "codeql-crqmh5"
  - "static-analysis-14v4mof"
  - "github-actions-7tcwgt"
  - "javascript-zxjsqy"
sourceUrls:
  - "https://github.blog/changelog/2026-08-19-codeql-2-26-3-improves-github-actions-queries-and-javascript-modeling"
---

- 移除 `codeql.actions.security.SelfHostedQuery` 模块：由于 runner 标签无法可靠区分自托管 runner 与托管 runner，引用该模块的自定义查询需要更新。
- 新增 JavaScript/TypeScript 流模型：支持 Vue 的 `ref`、`shallowRef`、`toRef`、`reactive` 和 `computed` Composition API 辅助函数，并将 Vue Router 的 `useRoute()` 识别为客户端远程流源。
- 改进 `actions/output-clobbering/high` 查询：不再报告简单的 jq 路径过滤器，并修复了未转义正则表达式输入导致的性能问题。

未来 GHES 版本将包含此功能，但具体版本号未在更新日志中提供。
