---
decisionKey: "6aa953196c07a9134484e06a25908fb169f1a9d6ca49f7bef15f2bf3d2a7c03b"
language: "zh-CN"
title: "Kubernetes 将 KYAML 提升为更安全、更一致的清单处理方式"
summary: "Kubernetes 已将在 v1.34 中作为 alpha 引入的 KYAML（严格 YAML 子集）推进到 beta，并在 v1.35 中默认启用，还提供了 kubectl 输出格式 -o kyaml 以转换现有清单。"
publishedAt: "2026-09-04T12:05:05.180Z"
score: 0.86
topics:
  - "Kubernetes"
  - "YAML"
  - "Configuration Management"
topicIds:
  - "kubernetes-wdjqe5"
  - "yaml-or7jby"
  - "configuration-management-1f092uo"
sourceUrls:
  - "https://www.infoq.com/news/2026/09/kubernetes-kyaml-manifests/"
---

- KYAML 是 YAML 的严格子集，在 Kubernetes v1.34 中作为 alpha 引入，并在 v1.35 中默认启用，现已进入 beta。
- Kubernetes 支持 `kubectl -o kyaml` 输出格式，可将现有 YAML 清单转换为 KYAML。
- KYAML 使用流式语法和双引号字符串，同时保持有效的 YAML，并兼容现有 Kubernetes 工具链和较旧版本的 kubectl。
- 具体语法规则的详细信息尚未完全公开；文章描述了其风格，但未提供完整规范或示例。
