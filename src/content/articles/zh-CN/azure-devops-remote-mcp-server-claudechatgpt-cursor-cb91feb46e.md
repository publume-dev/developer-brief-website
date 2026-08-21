---
decisionKey: "cb91feb46e5e1bd3b0f969a84e9bbc4c29bb577637f7ba25cd2fd210791fac98"
language: "zh-CN"
title: "Azure DevOps Remote MCP Server 正式发布，但不支持 Claude、ChatGPT 或 Cursor"
summary: "Azure DevOps Remote MCP Server 现已正式发布，提供托管端点，但由于 Microsoft Entra 的限制，Claude Desktop、Claude Code、ChatGPT 和 Cursor 无法连接。"
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

- Azure DevOps Remote MCP Server 现已正式发布，通过 streamable HTTP 提供托管端点，地址为 https://mcp.dev.azure.com/{organization}。
- 当前支持的客户端包括 Visual Studio Code with GitHub Copilot、Microsoft Foundry、Copilot Studio、Visual Studio、GitHub Copilot CLI 和 GitHub Copilot 应用。
- Claude Desktop、Claude Code、ChatGPT 和 Cursor 无法连接，因为它们需要 Microsoft Entra 支持动态 OAuth 客户端注册或客户端 ID 元数据文档。
- Entra 认证可确保 AI 助手继承开发者的权限，无需在配置文件中使用个人访问令牌。
- MCP 2026-07-28 规范（更早一周发布）优先使用预注册客户端，然后是客户端 ID 元数据文档，动态客户端注册作为已弃用的回退方案，计划在 2027 年夏季后移除。
- 需要 Entra 租户，因此仅使用 Microsoft 账户的独立组织不受支持。
- Microsoft 表示最近整合了本地工具集以与远程服务器保持一致，并承诺在 Entra 工作推进的同时保持一致性。

关注 Entra 团队何时为动态 OAuth 注册或客户端 ID 元数据文档提供支持，这可能决定 Claude、ChatGPT 和 Cursor 客户端能否在未来连接。
