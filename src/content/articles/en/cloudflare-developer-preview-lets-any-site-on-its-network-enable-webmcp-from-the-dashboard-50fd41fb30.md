---
decisionKey: "50fd41fb30e82a02730fe287f3d869bb3b7b3d1b23ef999222d522ba26dfb6a9"
language: "en"
title: "Cloudflare Developer Preview Lets Any Site on Its Network Enable WebMCP From the Dashboard"
summary: "Cloudflare launched a developer preview that gives any website on its network a WebMCP interface from the dashboard, enabling browser-based AI agents to use structured tools instead of scraping pages or automating UIs."
publishedAt: "2026-08-11T15:30:50.566Z"
score: 0.9
topics:
  - "WebMCP"
  - "Cloudflare"
  - "AI Agents"
topicIds:
  - "webmcp-xhdqsf"
  - "cloudflare-18thlla"
  - "ai-agents-1bsn16v"
sourceUrls:
  - "https://www.infoq.com/news/2026/08/cloudflare-webmcp/"
---

- Cloudflare announced the developer preview for exposing a WebMCP interface from any site on its network with a single dashboard switch; enabling it requires going to Agent Readiness > Labs in the Cloudflare Dashboard, toggling WebMCP on for a domain, and selecting desired tool packs.
- WebMCP targets browser-based AI agents, giving them structured tools for interacting with unmodified web pages instead of scraping or UI automation.
- The preview initially includes two tool packs: Content Credentials, which reads C2PA provenance metadata, and Site MCP server, which proxies a site's MCP server tools.
- Cloudflare's implementation injects a bridge.js module via HTMLRewriter at the edge, referencing the selected tool packs in a data-packs attribute.
- WebMCP is currently a preview standard and is supported only in Chrome 145 or later.
- Sites must expose their functionality as tools before they can adopt WebMCP, using either the document.modelContext API or a declarative JavaScript API for annotating HTML forms.
