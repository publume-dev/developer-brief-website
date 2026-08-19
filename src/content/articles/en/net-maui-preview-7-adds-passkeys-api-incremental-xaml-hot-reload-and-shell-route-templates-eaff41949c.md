---
decisionKey: "eaff41949c8c72b85eea82eae0ea8d51c99237f6c58b35d15f3c8c3965e309f3"
language: "en"
title: ".NET MAUI Preview 7 Adds Passkeys API, Incremental XAML Hot Reload, and Shell Route Templates"
summary: ".NET MAUI Preview 7 introduces a new Passkeys API, incremental XAML Hot Reload, Shell route templates, and AOT-safe bindings, offering developers a more efficient and secure development experience."
publishedAt: "2026-08-19T03:13:51.491Z"
score: 0.85
topics:
  - ".NET MAUI"
  - "XAML Hot Reload"
  - "Passkeys"
  - "Shell Navigation"
  - "AOT"
  - "Mobile Development"
topicIds:
  - "net-maui-xo9bps"
  - "xaml-hot-reload-1ulyx6t"
  - "passkeys-nhzzh8"
  - "shell-navigation-w5t5qt"
  - "aot-cj7ss7"
  - "mobile-development-hsmae2"
sourceUrls:
  - "https://www.infoq.com/news/2026/08/dotnet-11-preview7-maui/"
---

- MAUI Essentials adds a new Passkeys API supporting Android 14+, iOS and Mac Catalyst 16+, and Windows 10, with methods Passkeys.CreateAsync and Passkeys.AssertAsync.
- XAML Incremental Hot Reload is enabled by default for Debug builds as a preview feature, using a source generator with MetadataUpdateHandler to modify existing pages without full rebuilds.
- Shell navigation now supports route templates with required, optional, default, constrained, catch-all, and mixed segments, but only for absolute navigation.
- The XAML source generator expands AOT support so RelativeSource AncestorType bindings compile to trim-safe TypedBinding instances when the ancestor type is resolvable at compile time.
