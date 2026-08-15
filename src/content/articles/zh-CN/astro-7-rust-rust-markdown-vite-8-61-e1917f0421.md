---
decisionKey: "e1917f0421e4a2f56113a00c766fb690a06fba529b89bb0c878288d8b4c6b439"
language: "zh-CN"
title: "Astro 7 发布：Rust 编译器、Rust Markdown 管道和 Vite 8 使构建速度提升高达 61%"
summary: "Astro 7 已发布，采用基于 Rust 的新编译器并集成 Vite 8，官方基准测试显示构建速度提升 15% 至 61%。该版本还引入了更严格的 HTML 编译、高级路由、稳定缓存以及面向 AI 编码代理的新开发者体验特性。"
publishedAt: "2026-08-15T03:02:50.132Z"
score: 0.88
topics:
  - "Astro 7 Release"
  - "Rust Compiler"
  - "Web Framework Performance"
topicIds:
  - "astro-7-release-1dmoneg"
  - "rust-compiler-1idgrno"
  - "web-framework-performance-1vr362r"
sourceUrls:
  - "https://www.infoq.com/news/2026/08/astro-7-release-speed/"
---

- Astro 7 将 .astro 编译器重写为 Rust 实现，使用 oxc 进行解析，Lightning CSS 处理作用域，替换了原来的 Go 实现。
- 官方基准测试显示构建时间缩短 15% 至 61%：例如 astro.build 从 62.70 秒降至 24.24 秒，Cloudflare 开发者文档（8431 页）从 386.89 秒降至 261.94 秒。
- 引入更严格的 HTML 编译：未闭合标签将报错，无效嵌套按原样传递，空白处理遵从 JSX 规则。
- 新增高级路由，通过 src/fetch.ts 入口支持 Hono；稳定路由缓存，并为 Netlify、Vercel 和 Cloudflare 提供实验性 CDN 供应商；同时新增 `astro dev --background` 命令和 JSON 日志，便于 AI 编码代理使用。
- 迁移可通过 npx @astrojs/upgrade 进行，v7 升级指南提供详细说明。
