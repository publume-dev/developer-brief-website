---
decisionKey: "a433c9db1f4d45dbde9c845042c14534d7ffa1ee3f3ad2f575b6d420e8d56195"
language: "zh-CN"
title: "GitHub Copilot for JetBrains 新增企业管理设置：插件治理、MCP 服务器、OpenTelemetry 与权限模式"
summary: "GitHub Copilot for JetBrains 现已支持企业管理设置，使管理员能够集中控制插件、MCP 服务器、OpenTelemetry 和权限模式。此举增强了企业环境中的安全性和合规性。"
publishedAt: "2026-08-19T03:13:51.491Z"
score: 0.85
topics:
  - "GitHub Copilot"
  - "JetBrains"
  - "Enterprise Managed Settings"
topicIds:
  - "github-copilot-mbl6jy"
  - "jetbrains-1j3dqft"
  - "enterprise-managed-settings-wnejic"
sourceUrls:
  - "https://github.blog/changelog/2026-08-18-enterprise-managed-settings-in-github-copilot-for-jetbrains"
---

- GitHub Copilot for JetBrains 现已支持企业管理设置，涵盖插件治理、MCP 服务器访问、OpenTelemetry 和权限模式。
- 管理员可使用 `enabledPlugins` 强制启用或禁用插件，使用 `extraKnownMarketplaces` 添加受批准的插件来源，并使用 `strictKnownMarketplaces` 限制仅可从受批准来源安装插件。
- 管理员可通过 `allowedMcpServers` 和 `deniedMcpServers` 集中控制开发者可以从 GitHub Copilot for JetBrains 连接的 MCP 服务器。
- 管理员可以集中配置 JetBrains IDE 中 Copilot 的 OpenTelemetry，包括收集器端点、协议、服务名称、资源属性和内容捕获策略。
- 管理员可设置 `permissions.disableBypassPermissionsMode` 为 `disable`，以防止 JetBrains 中的 Copilot 代理使用“绕过批准”或“自动驾驶”功能。
