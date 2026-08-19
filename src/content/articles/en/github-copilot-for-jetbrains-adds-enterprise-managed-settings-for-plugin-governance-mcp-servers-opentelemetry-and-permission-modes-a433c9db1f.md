---
decisionKey: "a433c9db1f4d45dbde9c845042c14534d7ffa1ee3f3ad2f575b6d420e8d56195"
language: "en"
title: "GitHub Copilot for JetBrains Adds Enterprise Managed Settings for Plugin Governance, MCP Servers, OpenTelemetry, and Permission Modes"
summary: "GitHub Copilot for JetBrains now supports enterprise managed settings, enabling administrators to centrally control plugins, MCP servers, OpenTelemetry, and permission modes. This enhances security and compliance in enterprise environments."
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

- GitHub Copilot for JetBrains now supports enterprise managed settings for plugin governance, MCP server access, OpenTelemetry, and permission modes.
- Administrators can use `enabledPlugins` to require a plugin to be enabled or disabled, `extraKnownMarketplaces` to make approved plugin sources available, and `strictKnownMarketplaces` to limit installation to approved sources.
- Administrators can use `allowedMcpServers` and `deniedMcpServers` to centrally control which MCP servers developers can connect to from GitHub Copilot for JetBrains.
- Administrators can centrally configure OpenTelemetry for Copilot in JetBrains IDEs, including the collector endpoint, protocol, service name, resource attributes, and content-capture policy.
- Administrators can set `permissions.disableBypassPermissionsMode` to `disable` to prevent the Copilot agent in JetBrains from using Bypass Approvals or Autopilot.
