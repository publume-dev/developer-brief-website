---
decisionKey: "4f6d9c00497866fcd0278e5f2456b385cd5312a1ef2b9b00eb5e54659609f9d8"
language: "en"
title: "Agent Plugins 1.0 Released as Open Standard, Now Available in VS Code, Copilot CLI, and Copilot App"
summary: "GitHub announced the general availability of Agent Plugins 1.0, an open standard for packaging agent skills and MCP servers into a single installable plugin, now supported in VS Code, Copilot CLI, the Copilot app, and the Copilot SDK."
publishedAt: "2026-08-12T20:10:48.278Z"
score: 0.85
topics:
  - "Agent Plugins"
  - "GitHub Copilot"
  - "Developer Tooling"
topicIds:
  - "agent-plugins-11h2tga"
  - "github-copilot-mbl6jy"
  - "developer-tooling-q9uwan"
sourceUrls:
  - "https://github.blog/changelog/2026-08-12-agent-plugins-1-0-in-vs-code-copilot-cli-and-the-copilot-app"
---

- Agent Plugins 1.0 is an open standard for packaging agent skills and MCP servers into a single plugin, published on August 6 with AWS, Anysphere, Microsoft, OpenAI, and Vercel; Google joined as a core maintainer on the same day.
- Support is generally available in VS Code, Copilot CLI, the GitHub Copilot SDK, and the GitHub Copilot app, on all Copilot plans.
- To adopt the spec, plugin maintainers must add $schema to plugin.json, keep skills under skills/ and MCP configuration in mcp.json, and move Copilot-specific files into the com.github.copilot/ directory.
- Copilot Business and Enterprise customers can govern plugins via managed-settings.json using enabledPlugins, extraKnownMarketplaces, and strictKnownMarketplaces.
- Existing GitHub Copilot plugins that don't target Agent Plugins 1.0 remain supported, with no migration required.
