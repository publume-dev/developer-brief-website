---
decisionKey: "ff6b7dbce102ee2b5f3078889ada62e08f1b13de78404e1ce6c0a63c1a51a10c"
language: "en"
title: "GitHub Copilot SDK for Java Reaches Maven Preview with BYOK Support"
summary: "GitHub has published the Copilot SDK for Java as a Maven preview, giving Java developers a way to build Copilot-powered agent workflows and connect their own model providers without a Copilot subscription."
publishedAt: "2026-08-11T04:51:02.825Z"
score: 0.85
topics:
  - "Java Development"
  - "GitHub Copilot"
  - "SDK"
  - "AI Agents"
topicIds:
  - "java-development-18epgfg"
  - "github-copilot-mbl6jy"
  - "sdk-1osyxdn"
  - "ai-agents-1bsn16v"
sourceUrls:
  - "https://github.blog/engineering/using-the-github-copilot-sdk-for-java/"
---

The preview carries environment requirements rather than being a drop-in dependency: GitHub says the SDK needs the Copilot CLI at version 1.0.71 or later and JDK 17 or 25, with 25 recommended. It also supports bring-your-own-key (BYOK), so developers can point it at direct model providers such as OpenAI, Azure, Anthropic, or OpenAI-compatible endpoints without a Copilot subscription.

The Maven artifact is published as version 1.0.7-preview.1. The annotation-based tool API (@CopilotTool) is experimental and requires enabling experimental APIs and registering the annotation processor in the Maven build. GitHub describes this as "the first truly framework agnostic way to drive AI from Java," though that characterization is promotional and was not independently verified.

The main tradeoff is that BYOK provides provider flexibility, but adoption still depends on the CLI/JDK prerequisites and on an experimental tool API. The framework-agnostic framing should be treated as a vendor description rather than a verified guarantee.
