---
decisionKey: "50fd41fb30e82a02730fe287f3d869bb3b7b3d1b23ef999222d522ba26dfb6a9"
language: "zh-CN"
title: "Cloudflare 开发者预览：任何站点可从仪表板启用 WebMCP"
summary: "Cloudflare 推出开发者预览，让任何在其网络上的网站都能通过仪表板启用 WebMCP 接口，使基于浏览器的 AI 代理可以用结构化工具取代页面抓取和 UI 自动化。"
publishedAt: "2026-08-11T15:30:50.566Z"
score: 0.9
topics:
  - "WebMCP"
  - "Cloudflare"
  - "AI Agents"
topicIds:
  - "webmcp-xhdqsf"
  - "cloudflare-18thlla"
  - "ai-agents-1bsn16v"
sourceUrls:
  - "https://www.infoq.com/news/2026/08/cloudflare-webmcp/"
---

- Cloudflare 宣布该开发者预览：任何在其网络上的网站都可以通过单个仪表板开关暴露 WebMCP 接口；启用时需在 Cloudflare 控制台的 Agent Readiness > Labs 中为域名打开 WebMCP 开关，并选择所需工具包。
- WebMCP 面向基于浏览器的 AI 代理，让它们通过结构化工具与未修改的网页交互，而不是抓取页面或进行 UI 自动化。
- 预览版最初包含两个工具包：用于读取 C2PA 来源元数据的 Content Credentials，以及用于代理站点 MCP 服务器工具的 Site MCP server。
- Cloudflare 的实现方式是在边缘通过 HTMLRewriter 注入 bridge.js 模块，并在 data-packs 属性中引用所选工具包。
- WebMCP 目前是预览标准，仅支持 Chrome 145 或更高版本。
- 要采用 WebMCP，网站必须先将功能暴露为工具，可通过 document.modelContext API 或用于标注 HTML 表单的声明式 JavaScript API 实现。
