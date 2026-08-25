---
decisionKey: "ced408a6711a69cd8198c8f0267424f02f6d61b39050525265359727bc7a3dfb"
language: "en"
title: "GitHub Releases Alt-Text Quality Plugin with Five Deterministic Rules and Optional Model Check"
summary: "GitHub has released an alt-text quality plugin for its Accessibility Scanner, enabling five deterministic rules by default and an opt-in model-based check. The plugin helps developers identify missing or low-quality alt text to improve web accessibility."
publishedAt: "2026-08-25T14:27:51.056Z"
score: 0.85
topics:
  - "Accessibility"
  - "Developer Tooling"
  - "GitHub"
topicIds:
  - "accessibility-tz69kv"
  - "developer-tooling-q9uwan"
  - "github-9o7vw2"
sourceUrls:
  - "https://github.blog/engineering/user-experience/your-alt-text-passes-automated-checks-that-doesnt-mean-its-any-good/"
---

- GitHub released an alt-text quality plugin for its Accessibility Scanner that includes five deterministic rules on by default and an opt-in model-based check.
- The deterministic rules detect missing alt, filenames, placeholders, generic words, and repeated alt text; the repetition rule uses layout proximity rather than DOM order, with a gap threshold to decide when adjacent images form a repetitive run.
- The opt-in model-based rule is off by default, requires a token with access to GitHub Models, sends only the image and redacted context (URLs stripped of queries and fragments), and uses a four-step decision procedure to classify alt text as decorative, redundant, functional, or informative.
