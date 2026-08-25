---
decisionKey: "3b632aa788a19c04a97f1104fdd81c67c6fc6e3dc8e16b95b46f30139346dc48"
language: "zh-CN"
title: "Nuxt 4.5 发布：实验性 SSR 流式渲染、Vite 8 与基于 Rsbuild 的 Rspack 构建器"
summary: "Nuxt 4.5 引入了实验性的 SSR 流式渲染，并升级到 Vite 8，同时提供了基于 Rsbuild 的 Rspack 构建器，为开发者带来更快的首屏体验和更灵活的构建选项。"
publishedAt: "2026-08-25T14:27:51.056Z"
score: 0.85
topics:
  - "Nuxt 4.5"
  - "SSR Streaming"
  - "Vite 8"
  - "Rspack"
  - "Error Codes"
  - "useLayout"
topicIds:
  - "nuxt-4-5-mgzwap"
  - "ssr-streaming-bloc73"
  - "vite-8-2dskez"
  - "rspack-2oipqz"
  - "error-codes-6s26iz"
  - "uselayout-15ym6ka"
sourceUrls:
  - "https://www.infoq.com/news/2026/08/nuxt-4-5-streaming/"
---

- 实验性 SSR 流式渲染：启用 `experimental: { ssrStreaming: true }` 后，立即发送 HTML 壳，并在 Vue 渲染时流式传输正文。
- 流式渲染自动对爬虫和机器人禁用；使用重定向、缓存、isr 或 swr 规则的路由回退到缓冲渲染。
- 构建工具升级：采用 Vite 8，并引入基于 Rsbuild 重建的 Rspack 2 构建器。
- 稳定的错误代码系统：提供可检索的错误码（如 NUXT_E1001），包含解释和修复建议。
- 新 `useLayout` 组合式函数：返回当前路由布局的只读计算引用；命名视图支持通过 `child@sidebar.vue` 约定实现多个 NuxtPage 出口。
- `useFetch` 和 `useAsyncData` 新增响应式 `enabled` 选项，用于条件性获取。
- 主要依赖升级：unhead v3 和 unctx v3；unhead v3 对 useHead 的类型收窄可能带来破坏性类型变更。
- Nuxt 3 将于 2026 年 7 月 31 日停止维护，建议通过 `nuxt upgrade --dedupe` 升级。
