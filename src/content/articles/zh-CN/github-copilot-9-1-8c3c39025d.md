---
decisionKey: "8c3c39025d02c1362e8c220bf515833acf8389813960c449aec2b80dfc63a890"
language: "zh-CN"
title: "GitHub Copilot 全局模型策略正式发布，9 月 1 日前逐步生效"
summary: "GitHub 宣布 Copilot Business 和 Enterprise 计划的全局模型策略正式可用，并将在 2026 年 9 月 1 日前逐步强制执行。管理员需注意未配置模型的默认行为。"
publishedAt: "2026-08-30T12:02:47.817Z"
score: 0.85
topics:
  - "GitHub Copilot"
  - "Model Policy"
  - "Enterprise Managed Settings"
topicIds:
  - "github-copilot-mbl6jy"
  - "model-policy-1oxkots"
  - "enterprise-managed-settings-wnejic"
sourceUrls:
  - "https://github.blog/changelog/2026-08-26-global-model-policy-generally-available"
  - "https://github.blog/changelog/2026-08-26-enterprise-managed-settings-now-support-autoupdate-for-plugin-marketplaces"
---

- 全局模型策略现已对 Copilot Business 和 Enterprise 计划正式可用，强制执行将在 2026 年 9 月 1 日前逐步推出。\n- 策略生效后，未配置的模型将变为“委派给默认策略”并遵循企业的策略设置；如果策略启用（默认），这些模型将对用户可用。\n- 开放权重模型（如 DeepSeek、Kimi K2）以及未覆盖 GitHub 数据保留协议的模型（如 Fable 5）默认禁用，无论策略设置如何。\n- 企业托管设置现支持插件市场自动更新，通过在 extraKnownMarketplaces 条目上设置 autoUpdate: true 启用；支持的客户端（Copilot 应用、CLI 和 VS Code）会自动检查和更新。

管理员应检查现有模型配置，因为策略的逐步推出可能影响模型可用性。
