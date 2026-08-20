---
decisionKey: "69450efedab66f0f051d05325fbdcb1e3af166c195adbe04b1fbb42b76c4ea13"
language: "en"
title: "Next.js 16.3: Default Disk Cache and Memory Eviction Cut Dev Memory Up to 90%"
summary: "Next.js 16.3 enables disk caching and memory eviction by default, cutting development memory usage by up to 90% and making repeat builds up to 5.5 times faster. The release also adds faster TypeScript 7 support and optional Instant Navigations with caveats."
publishedAt: "2026-08-20T14:08:59.766Z"
score: 0.86
topics:
  - "Next.js"
  - "React Framework"
  - "Performance"
  - "Developer Tools"
  - "Turbopack"
  - "TypeScript"
topicIds:
  - "next-js-g23au9"
  - "react-framework-zjvpxo"
  - "performance-1ci3hd1"
  - "developer-tools-e6tceu"
  - "turbopack-1feb87a"
  - "typescript-72yc4i"
sourceUrls:
  - "https://www.infoq.com/news/2026/08/vercel-next-js-16-3/"
---

- Next.js 16.3 enables disk caching and a memory eviction feature by default, reducing dev memory usage by up to 90%.
- Vercel reports its dashboard memory usage dropped from 21.5GB to 2GB.
- The disk cache also accelerates `next build`, making repeat builds up to 5.5 times faster on CI.
- `next build` can run TypeScript 7, the native port claimed to be roughly ten times quicker.
- Server-side rendering was rebuilt on native Node.js streams, handling up to 22 percent more requests under load with no code changes.
- Instant Navigations is an opt-in set of tools enabled with `cacheComponents: true` and `partialPrefetching: true` flags.
- Caveats: static exports do not work with Partial Prefetching; global styled-jsx styles can leak between routes; and self-hosting on SST with cacheComponents can break server rendering.
- New projects can install with defaults using `npm install next@latest`; existing projects should follow the migrating to Cache Components guide before enabling the new behavior.
