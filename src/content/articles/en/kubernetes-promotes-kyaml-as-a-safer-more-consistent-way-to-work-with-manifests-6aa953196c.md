---
decisionKey: "6aa953196c07a9134484e06a25908fb169f1a9d6ca49f7bef15f2bf3d2a7c03b"
language: "en"
title: "Kubernetes Promotes KYAML as a Safer, More Consistent Way to Work with Manifests"
summary: "Kubernetes has moved KYAML, a strict YAML subset introduced as alpha in v1.34, to beta and enabled it by default in v1.35, with kubectl output format -o kyaml for converting existing manifests."
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

- KYAML is a strict subset of YAML, introduced as alpha in Kubernetes v1.34 and moved to beta, enabled by default, in v1.35.
- Kubernetes supports `kubectl -o kyaml` as an output format for converting existing YAML manifests to KYAML.
- KYAML uses flow-style syntax with double-quoted strings while remaining valid YAML and consumable by existing Kubernetes tooling and older kubectl versions.
- Exact details of KYAML's syntactic rules are not fully specified; the article describes the style but lacks a full specification or examples.
