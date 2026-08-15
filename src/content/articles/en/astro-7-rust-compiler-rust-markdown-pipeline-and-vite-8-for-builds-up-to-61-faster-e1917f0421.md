---
decisionKey: "e1917f0421e4a2f56113a00c766fb690a06fba529b89bb0c878288d8b4c6b439"
language: "en"
title: "Astro 7: Rust Compiler, Rust Markdown Pipeline and Vite 8 for Builds Up to 61% Faster"
summary: "Astro 7 is released with a new Rust-based compiler and Vite 8, showing 15% to 61% faster builds in official benchmarks. The version also introduces stricter HTML compilation, advanced routing, stabilized caching, and new developer experience features for AI coding agents."
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

- Astro 7 rewrites the .astro compiler in Rust using oxc for parsing and Lightning CSS for scoping, replacing the Go implementation.
- Benchmarks show builds 15 to 61 percent faster: astro.build dropped from 62.70s to 24.24s, and the 8,431-page Cloudflare developer docs fell from 386.89s to 261.94s.
- Introduces stricter HTML compilation: errors on unclosed tags, passes through invalid nesting as written, and follows JSX rules for whitespace.
- Adds advanced routing through a src/fetch.ts entrypoint compatible with Hono; stabilizes route caching with experimental CDN providers for Netlify, Vercel, and Cloudflare; and introduces `astro dev --background` plus JSON logging for AI coding agents.
- Migration is handled by npx @astrojs/upgrade, with the v7 upgrade guide covering details.
