---
decisionKey: "eaff41949c8c72b85eea82eae0ea8d51c99237f6c58b35d15f3c8c3965e309f3"
language: "zh-CN"
title: ".NET MAUI Preview 7 新增 Passkeys API、增量 XAML 热重载和 Shell 路由模板"
summary: ".NET MAUI Preview 7 引入了新的 Passkeys API、增量 XAML 热重载、Shell 路由模板及 AOT 安全绑定，为开发人员带来更高效、更安全的移动应用开发体验。"
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

- MAUI Essentials 新增 Passkeys API，支持 Android 14+、iOS 和 Mac Catalyst 16+、Windows 10，提供 Passkeys.CreateAsync 和 Passkeys.AssertAsync 方法。
- XAML 增量热重载作为预览功能默认在 Debug 构建中启用，通过源生成器配合 MetadataUpdateHandler 直接修改现有页面，无需完整重建。
- Shell 导航支持包含必需、可选、默认、约束、捕获所有及混合片段的路由模板，但仅适用于绝对导航。
- XAML 源生成器扩展 AOT 支持，当祖先类型在编译时可解析时，RelativeSource AncestorType 绑定编译为剪裁安全的 TypedBinding 实例。
