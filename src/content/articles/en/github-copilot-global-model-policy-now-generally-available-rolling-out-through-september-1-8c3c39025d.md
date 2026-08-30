---
decisionKey: "8c3c39025d02c1362e8c220bf515833acf8389813960c449aec2b80dfc63a890"
language: "en"
title: "GitHub Copilot global model policy now generally available, rolling out through September 1"
summary: "GitHub's global model policy for Copilot Business and Enterprise is generally available and will be enforced incrementally until September 1, 2026. Admins should watch unconfigured models, which will follow the enterprise policy by default."
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

- The global model policy for generally available GitHub Copilot models on Copilot Business and Enterprise plans is now generally available, with enforcement rolling out incrementally until September 1, 2026.\n- Once the policy takes effect, unconfigured models will change state to 'Delegate to default policy' and will follow the enterprise's policy setting; if policy is enabled (default), those models become available to users.\n- Open-weight models (e.g., DeepSeek, Kimi K2) and models not covered by GitHub's data retention agreement (e.g., Fable 5) are disabled by default regardless of the policy setting.\n- Enterprise managed settings now support autoUpdate for plugin marketplaces by setting autoUpdate: true on extraKnownMarketplaces entries; supported clients automatically check and update plugins from those marketplaces, with GA in Copilot app, CLI, and VS Code.

Admins should review existing model configurations because the gradual rollout may affect model availability.
