---
decisionKey: "328c01755bba0092539e70eea7685bb60557eb2cfe494d0e11b0f4dcc34ea841"
language: "zh-CN"
title: "VS Code 中的 GitHub Copilot 八月更新：并排聊天、/btw 侧边对话与可移植代理插件"
summary: "GitHub 在 VS Code 中发布了 2026 年 8 月的 Copilot 更新，引入了并排聊天、/btw 侧边对话、可移植代理插件以及改进的听写和浏览器功能。这些更新提升了代理交互和开发工作流的效率。"
publishedAt: "2026-09-01T12:05:09.734Z"
score: 0.85
topics:
  - "IDE"
  - "AI Assistants"
  - "Developer Tooling"
topicIds:
  - "ide-vutftr"
  - "ai-assistants-1six284"
  - "developer-tooling-q9uwan"
sourceUrls:
  - "https://github.blog/changelog/2026-08-31-github-copilot-in-vs-code-august-2026-releases"
---

- Agents 窗口现在支持并排排列聊天，并会在返回会话时恢复布局。
- /btw 命令打开一个侧边聊天，共享主聊天的上下文和提示缓存。
- 遵循 Agent Plugins 1.0 标准的可移植代理插件现在可以安装到 VS Code 中。
- 在 Claude 会话中，用户可以在 Anthropic 订阅和 Copilot 订阅的模型之间切换。
- VS Code 现在可以从 Sessions 列表继续在其他应用中创建的外部代理会话。
- Agent Host 可以将多个 VS Code 窗口连接到同一个代理会话。
- Agent Host 会话中的实验性 /rubber-duck 命令会请求互补模型揭示遗漏的细节和边缘情况。
- 聊天记录支持文本搜索，包括大小写匹配、全字匹配和正则表达式选项。
- 粘性滚动可在滚动长对话时将当前提示固定。
- 集成浏览器现在可以选择和注释 HTML 元素，以向代理提供 UI 反馈。
- 集成浏览器中的本地 HTML 文件在磁盘上更改时自动重新加载。
- 内置听写支持多种语言、项目特定指令以及终端命令的 shell 感知清理。
