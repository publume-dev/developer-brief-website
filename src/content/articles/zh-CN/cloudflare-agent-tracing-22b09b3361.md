---
decisionKey: "22b09b33619eb36abc2fb8b523a32e35634426e2c40b24da20bd888da7957332"
language: "zh-CN"
title: "Cloudflare 推出 Agent Tracing，包含截断限制和负载默认值不一致"
summary: "Cloudflare 发布了 agent tracing，为 Workers 跟踪添加 agent 级 span，测试期间免费，并从 2026 年 10 月 1 日起按 Workers Observability 定价。"
publishedAt: "2026-08-16T03:15:57.330Z"
score: 0.85
topics:
  - "Cloudflare Workers"
  - "AI Agent Observability"
  - "Developer Tooling"
topicIds:
  - "cloudflare-workers-1utxsc5"
  - "ai-agent-observability-bsqs1n"
  - "developer-tooling-q9uwan"
sourceUrls:
  - "https://www.infoq.com/news/2026/08/cloudflare-agent-tracing/"
---

- Cloudflare 已推出 agent tracing，为 Workers tracing 添加 agent 级 span。
- Agent tracing 包含 agent 调用、模型调用、工具执行和审批的 span，并将模型和 token 用量作为元数据。
- Cloudflare 警告不要从请求或用户标识符派生 agent 名称，以避免在仪表板中增加不同的 agent。
- 审批 span 记录 Worker 调用中的生命周期事件，而非人工介入延迟。
- 负载记录默认值不同：Think 和 wrapAISDK() 默认不存储消息或工具负载，除非启用；而 Flue 默认存储负载，需设置 content: false 停止。
- 跟踪并非无损；负载数据受 span 大小限制，且会话重放不显示图像。
- 从 2026 年 10 月 1 日起，Workers Free 包含每天 200,000 个可观测事件，保留三天；Workers Paid 包含每月 2000 万个，保留七天；每个 span 计为一个事件。
