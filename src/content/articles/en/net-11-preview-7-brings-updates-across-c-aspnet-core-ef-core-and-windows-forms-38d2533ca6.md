---
decisionKey: "38d2533ca65b6f0b899daead299e85f1a1eab6310e48283211987f2dbf50d498"
language: "en"
title: ".NET 11 Preview 7 Brings Updates Across C#, ASP.NET Core, EF Core, and Windows Forms"
summary: ".NET 11 Preview 7 delivers several developer-facing changes, including labeled break/continue in C#, a new union type matching approach, Blazor server circuit pausing, and a new Windows Forms rendering pipeline."
publishedAt: "2026-08-20T14:08:59.766Z"
score: 0.86
topics:
  - ".NET"
  - "C#"
  - "ASP.NET Core"
  - "Blazor"
  - "Entity Framework Core"
  - "Windows Forms"
  - "MAUI"
topicIds:
  - "net-9el0mc"
  - "c-15ny19f"
  - "asp-net-core-b9l8lp"
  - "blazor-zligoh"
  - "entity-framework-core-11d7xup"
  - "windows-forms-lp7sbl"
  - "maui-1jwyshl"
sourceUrls:
  - "https://www.infoq.com/news/2026/08/dotnet-11-preview-7/"
---

- In C#, break and continue statements can now name an enclosing loop or switch, allowing direct exit or continuation from inner constructs.
- The union types preview now uses a try-both approach: it tests a pattern against the union itself and then against its contained value.
- ASP.NET Core introduces the CacheView component, which caches rendered output of server-side subtrees and replays stored HTML on cache hits to reduce CPU and memory usage.
- Blazor Interactive Server circuits can pause themselves when a browser tab is hidden, releasing server resources until the user returns.
- Windows Forms introduces an opt-in modern rendering pipeline through VisualStylesMode.
