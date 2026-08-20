---
decisionKey: "69450efedab66f0f051d05325fbdcb1e3af166c195adbe04b1fbb42b76c4ea13"
language: "zh-CN"
title: "Next.js 16.3 发布：默认启用磁盘缓存与内存淘汰，开发内存占用最多可降 90%"
summary: "Next.js 16.3 通过默认启用磁盘缓存和内存淘汰，将开发内存占用最高降低 90%，并让重复构建提速最多 5.5 倍。该版本还支持更快的 TypeScript 7，并引入可选的 Instant Navigations 功能，但有一些注意事项。"
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

- Next.js 16.3 默认启用磁盘缓存和内存淘汰功能，开发内存占用最高可减少 90%。
- Vercel 报告其仪表盘内存使用从 21.5GB 降至 2GB。
- 磁盘缓存也加速了 `next build`，在 CI 上重复构建最快可提升 5.5 倍。
- `next build` 可运行 TypeScript 7，原生移植版据称速度提升约十倍。
- 服务端渲染改用原生 Node.js 流重建，无需修改代码即可处理最多 22% 的额外请求。
- Instant Navigations 是一组可选工具，通过 `cacheComponents: true` 和 `partialPrefetching: true` 启用。
- 注意事项：静态导出不支持 Partial Prefetching；全局 styled-jsx 样式可能跨路由泄漏；在 SST 上自托管并启用 cacheComponents 可能破坏服务端渲染。
- 新项目可通过 `npm install next@latest` 使用默认设置；现有项目应先查阅迁移到缓存组件的指南，再启用新行为。
