---
decisionKey: "60efff2a0c46e2a45c73ddd9733b20f1798d4fc725ed19044d3517e44285c747"
language: "en"
title: "Aspire 13.5 Release Brings Refreshed Dashboard, TypeScript AppHost GA, and Workflow Improvements"
summary: "Aspire 13.5 introduces a refreshed dashboard, TypeScript AppHost as generally available, and workflow improvements around Kubernetes integration."
publishedAt: "2026-08-22T13:43:12.485Z"
score: 0.85
topics:
  - ".NET Aspire"
  - "Developer Tooling"
  - "Cloud Development"
  - "TypeScript"
  - "Kubernetes"
topicIds:
  - "net-aspire-ms4w5a"
  - "developer-tooling-q9uwan"
  - "cloud-development-1tbwjnf"
  - "typescript-72yc4i"
  - "kubernetes-wdjqe5"
sourceUrls:
  - "https://www.infoq.com/news/2026/08/dotnet-aspire-13-5-release/"
---

- The dashboard gets a refreshed look, with improved accessibility, case-insensitive console log search, cleaner reconnection, and friendlier health-check failure messages.
- The Interaction Service now supports file imports (JSON or YAML), progress dialogs with optional cancellation, and named command arguments surfaced as input controls in the dashboard and CLI options.
- A terminal is added inside the dashboard via WithTerminal(), enabling interactive sessions, replica switching, and multiple viewers, though the feature is experimental.
- TypeScript AppHosts are now generally available, with the experimental opt-in removed and additional custom health checks and container file copying.
- Persistent volume modeling for Kubernetes workloads is introduced, including storage class, capacity, and access mode configuration, emitting persistent volume claims.
- The Aspire CLI can now be installed and updated via Homebrew, WinGet, npm, Nix, mise, and NuGet.
- Breaking changes include the renaming of ServiceProvider to Services, the deprecation of the GitHub Models integration, and removal of the dashboard's AI Assistant chat.
- The VS Code extension is rebranded to Aspire, adding a dashboard side panel, Bun and MAUI debugging support, and resource commands in the tree view.
