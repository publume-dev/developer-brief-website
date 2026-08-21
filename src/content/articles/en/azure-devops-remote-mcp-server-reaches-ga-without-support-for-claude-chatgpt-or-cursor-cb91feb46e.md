---
decisionKey: "cb91feb46e5e1bd3b0f969a84e9bbc4c29bb577637f7ba25cd2fd210791fac98"
language: "en"
title: "Azure DevOps Remote MCP Server Reaches GA, Without Support for Claude, ChatGPT, or Cursor"
summary: "The Azure DevOps Remote MCP Server is now generally available with a hosted endpoint, but Claude Desktop, Claude Code, ChatGPT, and Cursor cannot connect due to Microsoft Entra limitations."
publishedAt: "2026-08-21T14:06:07.365Z"
score: 0.9
topics:
  - "Azure DevOps"
  - "MCP"
  - "AI assistants"
  - "Developer tools"
topicIds:
  - "azure-devops-pjzhht"
  - "mcp-1kiasf7"
  - "ai-assistants-1six284"
  - "developer-tools-e6tceu"
sourceUrls:
  - "https://www.infoq.com/news/2026/08/azure-devops-remote-mcp-ga/"
---

- The Azure DevOps Remote MCP Server is now generally available, offering a hosted endpoint at https://mcp.dev.azure.com/{organization} over streamable HTTP.
- Currently supported clients include Visual Studio Code with GitHub Copilot, Microsoft Foundry, Copilot Studio, Visual Studio, GitHub Copilot CLI, and the GitHub Copilot app.
- Claude Desktop, Claude Code, ChatGPT, and Cursor cannot connect because they need support for dynamic OAuth client registration or Client ID Metadata Documents in Microsoft Entra.
- Entra authentication ensures the AI assistant inherits the developer's permissions, eliminating the need for personal access tokens in configuration files.
- The MCP 2026-07-28 specification, released a week before the GA, prefers pre-registered clients, then Client ID Metadata Documents, with Dynamic Client Registration as a deprecated fallback slated for removal after summer 2027.
- An Entra tenant is required, so standalone organizations using only Microsoft accounts are not supported.
- Microsoft says it recently consolidated the local toolset to align with the remote server and commits to maintaining parity while Entra work proceeds.

Watch for when the Entra team provides support for dynamic OAuth registration or Client ID Metadata Documents, which may determine whether Claude, ChatGPT, and Cursor clients can connect in the future.
