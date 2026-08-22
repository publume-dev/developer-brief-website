---
decisionKey: "1fe7b8ac0108b25b5c4e631744552542691197279983fd56652df3ee3f175669"
language: "en"
title: "AWS Releases aws-bench to Evaluate Agents on Real-World Cloud Tasks"
summary: "AWS has released aws-bench, an open-source benchmark for evaluating AI agents on real AWS tasks such as diagnosing misconfigurations, provisioning infrastructure, and operating live cloud environments. The benchmark uses isolated accounts with automated scoring via LLM or programmatic checks, but no baseline results or leaderboard are available yet."
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

- AWS released aws-bench, an open-source benchmark to evaluate AI agents on real AWS tasks like diagnosing misconfigurations, infrastructure provisioning, and operating live cloud environments.
- The benchmark deploys scenarios in isolated AWS accounts using resources defined in CDK stacks; agents run tasks in sandboxed containers with scoped credentials, and results are scored via an automated verifier, either an LLM judge or a programmatic check against live AWS state.
- Built-in adapters cover Claude Code, Codex, Kiro CLI, and Mini-SWE-Agent, and it supports any agent already included in Harbor, such as Gemini CLI and OpenCode.
- The project is built on Harbor, an open-source framework for evaluating AI agents, and is available on GitHub under the Apache-2.0 license.
- AWS has not published baseline results or a standardized leaderboard yet, placing them on the future roadmap; the setup is pinned to us-east-1 and may incur persistent resource costs.
- No metrics or baseline results are provided, leaving the benchmark's effectiveness or agent performance unverified; most tasks use an LLM judge, and AWS documents that leftover state can produce unwanted passes or random failures.
