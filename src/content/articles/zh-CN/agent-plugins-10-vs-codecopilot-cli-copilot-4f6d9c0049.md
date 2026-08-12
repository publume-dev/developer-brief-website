---
decisionKey: "4f6d9c00497866fcd0278e5f2456b385cd5312a1ef2b9b00eb5e54659609f9d8"
language: "zh-CN"
title: "Agent Plugins 1.0 开放标准发布，VS Code、Copilot CLI 和 Copilot 应用全面支持"
summary: "GitHub 宣布 Agent Plugins 1.0 开放标准正式可用，该标准将 agent 技能和 MCP 服务器打包为单一可安装插件，现已在 VS Code、Copilot CLI、Copilot 应用及 Copilot SDK 中全面支持。"
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

- Agent Plugins 1.0 是打包 agent 技能和 MCP 服务器的开放标准，于 8 月 6 日发布，AWS、Anysphere、Microsoft、OpenAI、Vercel 参与，Google 同日加入成为核心维护者。
- 该标准在 VS Code、Copilot CLI、GitHub Copilot SDK 和 GitHub Copilot 应用中全面可用，适用于所有 Copilot 计划。
- 插件维护者需在 plugin.json 中添加 $schema，将技能放在 skills/ 下，MCP 配置放在 mcp.json 中，并将 Copilot 特定文件移至 com.github.copilot/ 目录。
- Copilot Business 和 Enterprise 客户可通过 managed-settings.json 中的 enabledPlugins、extraKnownMarketplaces 和 strictKnownMarketplaces 进行治理。
- 不支持 Agent Plugins 1.0 的现有 GitHub Copilot 插件仍受支持，无需迁移。
