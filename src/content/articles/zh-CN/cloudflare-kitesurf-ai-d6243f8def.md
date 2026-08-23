---
decisionKey: "d6243f8def14d7ba3c93944aaabea7800f792dff94f92cf3913403fdce389ea4"
language: "zh-CN"
title: "Cloudflare 推出 Kitesurf：面向 AI 代理的浏览器引擎"
summary: "Cloudflare 发布了 Kitesurf，一个基于 WebAssembly/Rust 的轻量级浏览器引擎，可在 Workers 上运行自动化工作负载，并支持 CDP 以兼容 Playwright 和 Puppeteer，标志着从 Chromium 的重大架构转变。"
publishedAt: "2026-08-23T13:44:57.509Z"
score: 0.85
topics:
  - "Browser Engine"
  - "AI Agents"
  - "Cloudflare Workers"
  - "WebAssembly"
topicIds:
  - "browser-engine-g9zsv7"
  - "ai-agents-1bsn16v"
  - "cloudflare-workers-1utxsc5"
  - "webassembly-vyzybd"
sourceUrls:
  - "https://www.infoq.com/news/2026/08/cloudflare-kitesurf-browser/"
---

- Cloudflare 推出了 Kitesurf，一个面向自动化工作负载的轻量级浏览器，在 Cloudflare Workers 上以隔离的 WebAssembly/Rust 环境运行浏览器组件。
- Kitesurf 支持 Chrome DevTools Protocol (CDP)，允许 Playwright 和 Puppeteer 等工具驱动它，资源开销低于完整的 Chromium，但该低开销声明目前是定性的，没有量化基准。
- Kitesurf 将每个页面或 OOPIF 隔离在长期运行的 Dynamic Worker 中，拥有独立的 JavaScript 环境和 DOM，并使用基于 Rust 的 Blitz 渲染引擎和 Firefox 的 Stylo CSS 解析器构建 DOM。
- Kitesurf 尚不能替代 Chromium，缺少视频、WebGL、真实的基于 TLS 的机器人挑战以及长期认证会话的支持。
- Cloudflare 计划很快开源 Kitesurf，但目前尚无代码，且项目仍处于实验阶段，兼容性和 CDP/WPT 支持有待完善。
