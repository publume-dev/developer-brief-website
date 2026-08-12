---
decisionKey: "6dd48e1a9a9c326e05a00e5dc4d10bc00876d992a17e7c31a4362c3c3a753d97"
language: "zh-CN"
title: "JetBrains 版 GitHub Copilot 新增 Copilot 记忆、Ollama BYOK 与企业级管理设置"
summary: "JetBrains 版 GitHub Copilot 的最新版本新增跨会话 Copilot 记忆、Ollama 自带密钥（BYOK）提供商，以及由服务端控制的企业级管理设置。这使 JetBrains IDE 团队能够集中管理插件可用性、MCP 访问和遥测设置，并获得更新的 Codex 工作流。"
publishedAt: "2026-08-12T05:45:50.677Z"
score: 0.9
topics:
  - "GitHub Copilot"
  - "JetBrains IDEs"
  - "Developer Tooling"
topicIds:
  - "github-copilot-mbl6jy"
  - "jetbrains-ides-1frks8e"
  - "developer-tooling-q9uwan"
sourceUrls:
  - "https://github.blog/changelog/2026-08-11-copilot-memory-and-ollama-in-github-copilot-for-jetbrains"
---

- 企业托管设置：管理员现可在服务端控制 Copilot 插件可用性、MCP 服务器访问、权限绕过行为，以及 OpenTelemetry 设置。
- Copilot 记忆：Copilot 记忆可在 JetBrains 的代理聊天会话间保留并调取项目详情和偏好，开关位于 Copilot 设置门户的 Copilot Memory 选项中。
- Ollama BYOK：Ollama 已成为 JetBrains 版 GitHub Copilot 的 BYOK 提供商，支持在整个 JetBrains 体验中配置提供商和选择模型。
- CLI 自动安装：Copilot CLI 现在可以从集成终端自动安装，支持 macOS、Linux 和 Windows。
- Codex 工作流：Codex 会话现会出现在代理调试日志中，Codex 工作流支持更新后的权限模式，并可自定义指令和技能。
- 引用与调试入口：Copilot、Claude 和 Codex 聊天输入中恢复了文件和文件夹的 # 引用，代理调试日志按钮已移至 Options 下拉菜单。
- 可靠性改进：涉及 MCP 执行和审批、终端输出和自动批准、自定义项、云代理、基于 diff 的编辑，并修复了 ANSI 转义渲染和终端滚动条可预测性问题。
