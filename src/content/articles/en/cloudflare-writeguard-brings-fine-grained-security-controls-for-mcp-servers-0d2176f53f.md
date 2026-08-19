---
decisionKey: "0d2176f53f336e7b9175b9ce4d79628de506ffbac377841477d71af4d88851a9"
language: "en"
title: "Cloudflare WriteGuard Brings Fine-Grained Security Controls for MCP Servers"
summary: "Cloudflare is introducing WriteGuard, now in private beta, to provide fine-grained security controls for MCP servers, acting as a centralized policy, attribution, and auditing layer."
publishedAt: "2026-08-19T03:13:51.491Z"
score: 0.9
topics:
  - "Security"
  - "AI Agents"
  - "MCP"
topicIds:
  - "security-1jtharf"
  - "ai-agents-1bsn16v"
  - "mcp-1kiasf7"
sourceUrls:
  - "https://www.infoq.com/news/2026/08/cloudflare-writeguard-mcp-safety/"
---

- Cloudflare is introducing WriteGuard, now in private beta, to provide fine-grained security controls for MCP servers, acting as a shared policy, attribution, and auditing layer.
- WriteGuard sits behind Cloudflare's MCP server portal, intercepts all incoming MCP requests, and evaluates them against tool-specific policies, blocking or allowing requests without requiring changes to the MCP server itself.
- Each tool is assigned a risk tier ranging from read-only to critical, with examples such as completing a merge request as critical and adding a comment as minimal.
- WriteGuard uses existing OAuth credentials to identify users, avoiding standalone agent accounts, and adds MCP client and session context for auditability.
- WriteGuard classifies each invocation as successful, failed, or blocked, and asynchronously sends a scrubbed audit event to an internal audit Worker, omitting sensitive values.
