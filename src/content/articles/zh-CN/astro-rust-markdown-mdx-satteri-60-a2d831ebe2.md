---
decisionKey: "a2d831ebe22b982c16642eaa4f4d2ccc9a129e3e059cf21e86980b36da466b26"
language: "zh-CN"
title: "Astro 推出基于 Rust 的 Markdown 和 MDX 处理器 Sätteri，构建速度提升最高达 60%"
summary: "Astro 团队发布了 Rust 驱动的 Markdown 和 MDX 处理器 Sätteri，并已将其作为 Astro 7.0 的核心依赖，可显著提升构建速度。"
publishedAt: "2026-08-29T12:02:34.357Z"
score: 0.85
topics:
  - "Rust"
  - "Markdown"
  - "MDX"
  - "Astro"
  - "Build Tools"
topicIds:
  - "rust-845rdz"
  - "markdown-1ades7g"
  - "mdx-1oe8dms"
  - "astro-19njtsc"
  - "build-tools-tnqz7s"
sourceUrls:
  - "https://www.infoq.com/news/2026/08/astro-satteri-rust/"
---

- Sätteri 是 Astro 团队推出的基于 Rust 的 Markdown 和 MDX 处理器，现已成为 Astro 7.0 的核心依赖，据称可使构建速度提升最高达 60%。
- 将 Astro 和 Cloudflare 文档站点切换到 Sätteri 后，各自的构建时间减少了一分钟以上，Astro 7 整体构建时间改善了 15% 至 61%。
- Sätteri 原生支持 GitHub 风格 Markdown、智能标点、容器指令、数学公式、frontmatter、上标、下标和 wikilinks 等功能，这些功能此前需要单独的插件。
- Sätteri 不运行 remark 或 rehype 插件；使用这些插件的项目可以将插件移植为 Sätteri MDAST 或 HAST 插件，或通过安装 @astrojs/markdown-remark 继续使用 unified。
