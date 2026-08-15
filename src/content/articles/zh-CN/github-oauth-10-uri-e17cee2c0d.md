---
decisionKey: "e17cee2c0d5cf7d2bacdc4e950a18a638eeb1048d31a5a30f8795a66046043a6"
language: "zh-CN"
title: "GitHub 为 OAuth 应用推出可选短时访问令牌与最多 10 个重定向 URI"
summary: "GitHub 为 OAuth 应用引入可选的短时访问令牌（8 小时）和刷新令牌（6 个月），并支持最多 10 个重定向 URI。新应用默认启用短时令牌，且这些改进将包含在 GitHub Enterprise Server 3.23 中。"
publishedAt: "2026-08-15T03:02:50.132Z"
score: 0.9
topics:
  - "OAuth"
  - "GitHub Apps"
  - "Token Refresh"
  - "Redirect URIs"
  - "Platform Security"
topicIds:
  - "oauth-1y1upas"
  - "github-apps-gwfp2i"
  - "token-refresh-8jyxq5"
  - "redirect-uris-cyrpaw"
  - "platform-security-npelqg"
sourceUrls:
  - "https://github.blog/changelog/2026-08-14-multiple-redirect-uris-and-token-refresh-for-oauth-apps"
---

- OAuth 应用可选择启用短时访问令牌：访问令牌有效期为 8 小时，刷新令牌有效期为 6 个月，刷新令牌用于在过期后获取新的令牌对。
- 开发者可通过在认证请求中包含 offline_access 范围或设置应用注册始终使用短时令牌来启用该模式；所有新应用默认启用短时令牌。
- OAuth 应用现在可以注册最多 10 个重定向 URI（回调 URI），以支持多个环境或域名而无需创建单独的应用。
- OAuth 应用和 GitHub 应用可以为每个重定向 URI 启用通配符匹配，但这可能被滥用，如果重定向目标对其路由没有强控制；只有一个重定向 URI 的应用默认启用通配符匹配，这是旧行为，现在可见且可控。

这些改进将包含在 GitHub Enterprise Server 3.23 中。
