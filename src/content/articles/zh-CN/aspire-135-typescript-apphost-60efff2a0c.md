---
decisionKey: "60efff2a0c46e2a45c73ddd9733b20f1798d4fc725ed19044d3517e44285c747"
language: "zh-CN"
title: "Aspire 13.5 发布：更新仪表板、TypeScript AppHost 正式可用及多项工作流改进"
summary: "Aspire 13.5 带来了刷新后的仪表板、TypeScript AppHost 正式可用，以及与 Kubernetes 集成相关的工作流改进。"
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

- 仪表板经过刷新，改进了可访问性、不区分大小写的控制台日志搜索、更干净的重新连接以及更友好的健康检查失败消息。
- Interaction Service 支持文件导入（JSON 或 YAML）、带可选取消功能的进度对话框，以及将命名命令参数显示为仪表板中的输入控件和 CLI 选项。
- 仪表板内通过 WithTerminal() 新增终端（实验性功能），支持交互式会话、副本切换和多查看器。
- TypeScript AppHost 现为正式可用，移除了实验性选择加入，并增加了自定义健康检查和容器文件复制。
- 为 Kubernetes 工作负载引入持久卷建模，包括存储类、容量和访问模式配置，并生成持久卷声明。
- Aspire CLI 现可通过 Homebrew、WinGet、npm、Nix、mise 和 NuGet 安装和更新。
- 破坏性变更：ServiceProvider 重命名为 Services，GitHub Models 集成弃用，仪表板 AI 助手聊天移除。
- VS Code 扩展更名为 Aspire，新增仪表板侧面板、Bun 和 MAUI 调试支持，以及树视图中的资源命令。
