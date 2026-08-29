---
decisionKey: "a2d831ebe22b982c16642eaa4f4d2ccc9a129e3e059cf21e86980b36da466b26"
language: "en"
title: "Astro Introduces Sätteri: A Rust-powered Markdown and MDX Processor With Up to 60% Faster Builds"
summary: "Astro team has introduced Sätteri, a Rust-powered Markdown and MDX processor now a core dependency of Astro 7.0, delivering up to 60% faster builds."
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

- Sätteri is a Rust-powered Markdown and MDX processor introduced by the Astro team, now a core dependency of Astro 7.0, contributing up to 60% faster builds.
- Switching the Astro and Cloudflare documentation sites to Sätteri reduced build times by over a minute each, with overall Astro 7 builds improving by 15 to 61%.
- Sätteri natively implements features like GitHub Flavored Markdown, smart punctuation, container directives, math, frontmatter, superscript, subscript, and wikilinks, which previously required separate plugins.
- Sätteri does not run remark or rehype plugins; projects with such plugins can port them to Sätteri MDAST or HAST plugins or stay on unified by installing @astrojs/markdown-remark.
