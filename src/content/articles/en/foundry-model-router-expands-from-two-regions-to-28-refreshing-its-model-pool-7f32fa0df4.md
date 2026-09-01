---
decisionKey: "7f32fa0df4bf1da5ce9fc2a2f0ed7282d1efaf2340dfa24d3960afe99b05e203"
language: "en"
title: "Foundry Model Router Expands from Two Regions to 28, Refreshing Its Model Pool"
summary: "Microsoft expanded Foundry Model Router from two regions to 28 for global standard deployments and 21 for data zone deployments, and updated the model pool with additions like Claude Opus 4.8 and the GPT-5.6 family while removing end-of-life models."
publishedAt: "2026-09-01T12:05:09.734Z"
score: 0.9
topics:
  - "Azure Foundry"
  - "Model Routing"
  - "LLM Deployment"
topicIds:
  - "azure-foundry-epv4bl"
  - "model-routing-1wo1oy8"
  - "llm-deployment-1qs2k9r"
sourceUrls:
  - "https://www.infoq.com/news/2026/08/foundry-model-router-regions/"
---

- Region expansion: from two regions (East US 2, Sweden Central) to 28 for global standard deployments, and 21 for data zone deployments.
- Model pool changes: added Anthropic Claude Opus 4.8 and the GPT-5.6 family; removed gpt-5-chat, gpt-5.2-chat, gpt-5.3-chat, and DeepSeek-V3.1 due to end of life.
- Configuration impact: teams using default configuration receive the model pool change automatically without redeploying; teams with a configured model subset do not, as new models are excluded by default until explicitly added.
- Routing modes: three modes—Balanced (default), Quality (for legal review, medical summaries, complex reasoning), and Cost (for high-volume classification and simple Q&A); changes take up to five minutes.
- Context window: effective window equals the smallest underlying model's window, so adding smaller models lowers the ceiling for all requests.
- Text-only routing: vision inputs are accepted but images do not influence model selection; audio is unsupported.
- Claude models must be deployed separately to the same Foundry account with a matching SKU before the router can select them; referencing them without that deployment fails with InvalidResourceProperties error.
- Azure Policy: router honors the built-in policy, enforced at deploy time; allowed publishers list must include Microsoft plus every publisher in the pool.
- Auditability: every response names the selected model in the model field.
- Recommendation: treat initial deployment as a starting configuration and benchmark before production traffic; Microsoft provides an open-source evaluation pipeline for quality, cost, and latency.
