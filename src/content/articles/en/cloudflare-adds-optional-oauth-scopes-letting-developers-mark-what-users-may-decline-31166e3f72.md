---
decisionKey: "31166e3f726daa18bd891a5c05fc2a12f4afdacd45da67e4e478f0677396244b"
language: "en"
title: "Cloudflare Adds Optional OAuth Scopes, Letting Developers Mark What Users May Decline"
summary: "Cloudflare has introduced optional OAuth scopes, allowing applications to mark permissions as deniable by users, offering more flexible consent flows."
publishedAt: "2026-09-02T12:05:26.117Z"
score: 0.9
topics:
  - "OAuth"
  - "Cloudflare"
  - "Security"
  - "Identity and Access Management"
  - "MCP Servers"
topicIds:
  - "oauth-1y1upas"
  - "cloudflare-18thlla"
  - "security-1jtharf"
  - "identity-and-access-management-ek3pxf"
  - "mcp-servers-hifxuf"
sourceUrls:
  - "https://www.infoq.com/news/2026/09/cloudflare-optional-oauth-scopes/"
---

- Cloudflare now lets client owners mark scopes as optional via an optional_scopes array alongside the scopes array.
- During an authorization flow, the consent screen shows only the scopes requested in that flow, and required and optional scopes are evaluated against those requested scopes, not the full client configuration.
- Applications must inspect the scope parameter in the token response after code exchange to see which scopes were granted, and should degrade gracefully if optional scopes are declined, rather than failing.
