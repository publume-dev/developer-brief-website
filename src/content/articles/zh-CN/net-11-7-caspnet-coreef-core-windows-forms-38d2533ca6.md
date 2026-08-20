---
decisionKey: "38d2533ca65b6f0b899daead299e85f1a1eab6310e48283211987f2dbf50d498"
language: "zh-CN"
title: ".NET 11 预览版 7 更新 C#、ASP.NET Core、EF Core 和 Windows Forms"
summary: ".NET 11 预览版 7 带来了多项面向开发者的更新，包括 C# 的带标签 break/continue、联合类型的新匹配方式、Blazor 服务器电路暂停以及 Windows Forms 的新渲染管线。"
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

- C# 的 break 和 continue 语句现在可以指定要退出的封闭循环或 switch，从而允许从内部构造直接退出或继续。
- 联合类型预览版更新为使用 try-both 方法：先针对联合本身测试模式，然后针对其包含的值进行测试。
- ASP.NET Core 引入了 CacheView 组件，它缓存服务器端子树的渲染输出，并在缓存命中时重放存储的 HTML，以减少 CPU 和内存使用。
- Blazor Interactive Server 电路可以在浏览器标签页隐藏时自我暂停，释放服务器资源，直到用户返回。
- Windows Forms 通过 VisualStylesMode 引入了选择加入的现代渲染管线。
