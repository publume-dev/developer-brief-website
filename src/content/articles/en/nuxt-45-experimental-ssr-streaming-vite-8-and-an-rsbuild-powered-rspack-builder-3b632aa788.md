---
decisionKey: "3b632aa788a19c04a97f1104fdd81c67c6fc6e3dc8e16b95b46f30139346dc48"
language: "en"
title: "Nuxt 4.5: Experimental SSR Streaming, Vite 8, and an Rsbuild-Powered Rspack Builder"
summary: "Nuxt 4.5 introduces experimental SSR streaming, upgrades to Vite 8, and offers an Rspack builder rebuilt on Rsbuild, giving developers faster first paint and more flexible build options."
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

- Experimental SSR streaming: Enable `experimental: { ssrStreaming: true }` to flush the HTML shell immediately and stream the body as Vue renders.
- Streaming is automatically disabled for bots and crawlers; routes using redirect, cache, isr, or swr rules fall back to buffered rendering.
- Tooling upgrades: Move to Vite 8 and include a Rspack 2 builder rebuilt on top of Rsbuild.
- Stable error code system: Greppable codes such as NUXT_E1001 include explanation and fix suggestions.
- New useLayout composable: Returns a read-only computed ref of the current route's layout; named views support multiple NuxtPage outlets via the `child@sidebar.vue` convention.
- `useFetch` and `useAsyncData` gain a reactive `enabled` option to gate conditional fetches.
- Major dependency bumps: unhead v3 and unctx v3; unhead v3 introduces type-narrowing for useHead that can be a breaking type change.
- Nuxt 3 reaches end-of-life on July 31, 2026; upgrading is recommended via `nuxt upgrade --dedupe`.
