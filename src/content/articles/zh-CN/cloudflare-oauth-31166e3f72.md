---
decisionKey: "31166e3f726daa18bd891a5c05fc2a12f4afdacd45da67e4e478f0677396244b"
language: "zh-CN"
title: "Cloudflare 推出可选 OAuth 作用域，支持用户拒绝部分权限"
summary: "Cloudflare 新增可选 OAuth 作用域，使应用能将权限标记为可被用户拒绝，为开发者提供更灵活的授权流程。"
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

- Cloudflare 现已允许客户端所有者通过 optional_scopes 数组（与 scopes 数组并列）标记用户可拒绝的作用域。
- 授权流程中，同意页面仅显示该流程请求的作用域；必需和可选作用域的评估均基于这些被请求的作用域，而非完整的客户端配置。
- 应用必须在代码交换后检查令牌响应中的 scope 参数以确定被授予的作用域；若可选作用域被拒绝，应优雅降级而不是中断。
