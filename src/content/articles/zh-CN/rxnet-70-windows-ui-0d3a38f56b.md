---
decisionKey: "0d3a38f56b3207d5193f827b8f8525bf197e4efb18ebe15c7cab468901c53edf"
language: "zh-CN"
title: "Rx.NET 7.0 分割 Windows UI 支持包，显著减小部署体积"
summary: "Rx.NET 7.0 将 Windows UI 支持拆分为独立包，可使自包含 Windows 应用的部署体积减少约 90 MB（未裁剪时），并移除对 .NET 6 和 .NET 7 的支持。"
publishedAt: "2026-08-15T03:02:50.132Z"
score: 0.88
topics:
  - "Rx.NET"
  - "Package Split"
  - "Deployment Size"
  - "Breaking Changes"
  - ".NET"
topicIds:
  - "rx-net-1mlszfi"
  - "package-split-15eaug7"
  - "deployment-size-mv8ew3"
  - "breaking-changes-1e9r88x"
  - "net-9el0mc"
sourceUrls:
  - "https://www.infoq.com/news/2026/08/rx-net-7/"
---

- Rx.NET 7.0 将 Windows UI 支持细分为多个独立包：System.Reactive.Windows.Forms、System.Reactive.Wpf、System.Reactive.WindowsRuntime 和 System.Reactive.Uwp，从而减小自包含 Windows 应用的部署体积。
- 对于受影响的 Windows 特定 TFM 项目，此拆分可减少约 90 MB（未裁剪）、47 MB（裁剪）和 11 MB（Native AOT）的部署体积。
- Rx.NET 7.0 放弃对 .NET 6 和 .NET 7 的支持，同时继续支持 .NET 8、.NET 9、.NET 10、.NET Framework 4.7.2、.NET Standard 2.0 和 UWP。
- UI API 仍保留在运行时程序集中，但已从引用程序集中移除，从而保持针对 Rx.NET 6.1 预编译组件的二进制兼容性；新增分析器会推荐所需包。
- 使用 packages.config 的项目可能仍会看到 UI API 而无需显式包引用，但此配置不受维护者支持，并可能在将来移除。
- Rx.NET 7.0 修正了 OfType 的可空性注解，这是一个签名变更，根据语义化版本控制需要主版本号。
