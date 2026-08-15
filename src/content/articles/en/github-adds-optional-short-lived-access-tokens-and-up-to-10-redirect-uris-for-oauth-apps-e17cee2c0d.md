---
decisionKey: "e17cee2c0d5cf7d2bacdc4e950a18a638eeb1048d31a5a30f8795a66046043a6"
language: "en"
title: "GitHub Adds Optional Short-Lived Access Tokens and Up to 10 Redirect URIs for OAuth Apps"
summary: "GitHub now lets OAuth apps opt in to expiring access tokens (8 hours) with refresh tokens (6 months), and register up to 10 redirect URIs. New apps enable short-lived tokens by default, and the improvements are coming to GitHub Enterprise Server 3.23."
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

- OAuth apps can opt in to expiring access tokens: an access token valid for eight hours and a refresh token valid for six months, with the refresh token used to obtain a new token pair after expiry.
- Developers can enable the short-lived token pattern for OAuth apps either by including the offline_access scope in the authentication request or by setting the app registration to always use short-lived tokens; short-lived tokens are enabled by default for all new applications.
- OAuth apps can now register up to 10 redirect URIs (callback URIs) to support multiple environments or domains without creating separate apps.
- OAuth apps and GitHub Apps can enable wildcard matching for each redirect URI, but this can be abused if the redirect target does not have strong control over its routes; apps with only one redirect URI have wildcard matching enabled as a legacy behavior that is now visible and controllable.

These improvements will be included in GitHub Enterprise Server 3.23.
