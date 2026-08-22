---
decisionKey: "1fe7b8ac0108b25b5c4e631744552542691197279983fd56652df3ee3f175669"
language: "zh-CN"
title: "AWS 发布 aws-bench：面向真实云任务的 AI 智能体评估基准"
summary: "AWS 发布了 aws-bench，一个用于评估 AI 智能体在真实 AWS 任务（如诊断配置错误、基础设施预置和运维）中表现的开源基准。该基准使用隔离账户并通过 LLM 或程序化检查自动评分，但目前尚未公布基线结果或排行榜。"
publishedAt: "2026-08-22T13:43:12.485Z"
score: 0.85
topics:
  - "AI Agents"
  - "Benchmarking"
  - "AWS"
  - "Open Source"
  - "Cloud Development"
topicIds:
  - "ai-agents-1bsn16v"
  - "benchmarking-h22znw"
  - "aws-7brv06"
  - "open-source-17ixijy"
  - "cloud-development-1tbwjnf"
sourceUrls:
  - "https://www.infoq.com/news/2026/08/aws-bench-agent-evaluation/"
---

- AWS 发布了 aws-bench，一个开源基准，用于评估 AI 智能体在真实 AWS 任务（如诊断配置错误、基础设施预置和运维实时云环境）上的表现。
- 该基准在隔离的 AWS 账户中部署场景，场景资源由 CDK 堆栈定义；智能体在具有受限凭证的沙箱容器中运行任务，结果由自动化验证器评分，验证器可以是 LLM 裁判或针对实时 AWS 状态的程序化检查。
- 内置适配器支持 Claude Code、Codex、Kiro CLI 和 Mini-SWE-Agent，并支持 Harbor 中已有的任何智能体，如 Gemini CLI 和 OpenCode。
- 该项目基于 Harbor（一个用于评估 AI 智能体的开源框架），并在 GitHub 上以 Apache-2.0 许可证提供。
- AWS 尚未公布基线结果或标准化排行榜，这些已列入未来路线图；该设置固定使用 us-east-1 区域，并可能产生持续的持久资源成本。
- 由于缺少指标，基准的有效性或智能体性能尚未得到验证；大多数任务使用 LLM 裁判评估，AWS 文档指出残留状态可能导致不应有的通过或随机失败。
