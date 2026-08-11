---
decisionKey: "ff6b7dbce102ee2b5f3078889ada62e08f1b13de78404e1ce6c0a63c1a51a10c"
language: "zh-CN"
title: "GitHub Copilot Java SDK 发布 Maven 预览版，支持自带模型密钥"
summary: "GitHub 已以 Maven 预览形式发布 Copilot Java SDK，让 Java 开发者能够构建由 Copilot 驱动的代理工作流，并通过自带模型密钥接入不同模型提供商，无需 Copilot 订阅。"
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

该预览版带有运行环境要求，而不是一个直接可用的依赖：GitHub 称 SDK 需要本机安装 Copilot CLI 1.0.71 或更新版本，并要求 JDK 17 或 25（推荐 25）。SDK 同时支持 BYOK（自带密钥），可以对接 OpenAI、Azure、Anthropic 或 OpenAI 兼容端点，而无需 Copilot 订阅。

该 Maven 构件以 1.0.7-preview.1 版本发布。基于注解的工具调用 API（@CopilotTool）仍处于实验阶段，使用时需要启用实验 API，并在 Maven 构建中注册注解处理器。官方博客称这是“首个真正框架无关的从 Java 驱动 AI 的方式”，但该说法属于宣传性表述，尚未获得独立验证。

对评估该预览版的团队来说，主要权衡在于：BYOK 提供了模型提供商方面的灵活性，但采用时仍要满足 CLI 和 JDK 前提条件，并且工具 API 还是实验特性。将“框架无关”视为官方宣传而非既定事实，是更稳妥的预期。
