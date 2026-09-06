---
decisionKey: "b9c1ffc792bb5985230c47ac195dca7a513a40e5da45bc5638a2c4d164fc468b"
language: "zh-CN"
title: "谷歌开源 Mantis：面向漏洞生命周期的智能代理框架"
summary: "谷歌已开源 Mantis，这是一个智能代理框架，用于自动化软件漏洞的识别、验证、复现和修复，并通过分层文件摘要将令牌使用量减少 85%。"
publishedAt: "2026-09-06T14:38:26.492Z"
score: 0.85
topics:
  - "Open Source"
  - "Security"
  - "AI Development Tools"
topicIds:
  - "open-source-17ixijy"
  - "security-1jtharf"
  - "ai-development-tools-12bmj4p"
sourceUrls:
  - "https://www.infoq.com/news/2026/09/google-mantis-vulnerability-scan/"
---

- 谷歌已开源 Mantis，这是一个旨在自动化软件漏洞生命周期的 AI 代理框架，涵盖漏洞的识别、验证、复现和修复。
- Mantis 通过将分析文件汇总为包含目录和仓库级上下文的分层树，将令牌使用量减少 85%。
- Mantis 采用模块化技能套件组织，包含超过 15 个工具，各阶段通过存储在磁盘上的共享状态进行通信。
- Mantis 支持在不同阶段组合不同 AI 模型，建议在分类阶段使用较轻量模型，在编写崩溃复现程序和生成修复等任务中使用更强大的模型。
- Mantis 通过 mantis-review 阶段利用基于规则的负向过滤器解决误报问题，但应谨慎使用该过滤器，以避免降低真正的漏洞检测率。
