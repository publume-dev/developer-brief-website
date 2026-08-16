---
decisionKey: "22b09b33619eb36abc2fb8b523a32e35634426e2c40b24da20bd888da7957332"
language: "en"
title: "Cloudflare Adds Agent Tracing, with Truncation Limits and Uneven Payload Defaults"
summary: "Cloudflare has launched agent tracing, adding agent-level spans to Workers tracing, free during beta and priced under Workers Observability from October 1, 2026."
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

- Cloudflare has launched agent tracing, adding agent-level spans to Workers tracing.
- Agent tracing includes spans for agent invocations, model calls, tool execution, and approvals, with model and token usage as metadata.
- Cloudflare warns against deriving agent names from request or user identifiers to avoid multiplying distinct agents in the dashboard.
- Approval spans record lifecycle events within a Worker invocation, not human-in-the-loop latency.
- Payload recording defaults differ: Think and wrapAISDK() do not store message or tool payloads unless enabled, while Flue stores them by default requiring content: false to stop.
- Traces are not lossless; payload data is subject to span size limits and session replay does not display images.
- From October 1, Workers Free includes 200,000 observability events per day with three-day retention, Workers Paid includes 20 million per month with seven-day retention, and each span counts as one event.
