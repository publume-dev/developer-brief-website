---
decisionKey: "0d3a38f56b3207d5193f827b8f8525bf197e4efb18ebe15c7cab468901c53edf"
language: "en"
title: "Rx.NET 7.0 Reduces Deployment Size by Splitting Windows UI Support"
summary: "Rx.NET 7.0 splits Windows UI support into separate packages, cutting deployment size by about 90 MB for self-contained Windows apps without trimming, and drops support for .NET 6 and .NET 7."
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

- Rx.NET 7.0 splits Windows UI support into separate packages: System.Reactive.Windows.Forms, System.Reactive.Wpf, System.Reactive.WindowsRuntime, and System.Reactive.Uwp, reducing deployment size for self-contained Windows apps.
- The split can reduce deployment size by approximately 90 MB without trimming, 47 MB with trimming, and 11 MB for Native AOT builds, for affected Windows-specific TFM projects.
- Rx.NET 7.0 drops support for .NET 6 and .NET 7, while continuing to support .NET 8, .NET 9, .NET 10, .NET Framework 4.7.2, .NET Standard 2.0, and UWP.
- The UI APIs remain in runtime assemblies but are removed from reference assemblies, preserving binary compatibility for precompiled components built against Rx.NET 6.1, with an analyzer to recommend required packages.
- Projects using packages.config may still see UI APIs without explicit package references, a configuration not supported by maintainers and possibly removed in future.
- Rx.NET 7.0 corrects nullability annotations for OfType, a signature change that technically requires a major version under semantic versioning.
