---
decisionKey: "619e431435330eab06e62c9ee8d934bfe39bf2c2fc42ef551c80377711cdf5ce"
language: "zh-CN"
title: "GitHub Agentic Workflows 在 0.82.9 中增加 Docker Sandbox 作为代理运行时"
summary: "GitHub Agentic Workflows（gh-aw）0.82.9 支持将 Docker Sandbox 作为代理运行时，提供微虚拟机隔离环境。该功能要求配置特定的运行时设置和 Docker 凭据，并启用相关 GitHub 权限。"
publishedAt: "2026-08-21T14:06:07.365Z"
score: 0.85
topics:
  - "AI Agent Sandboxing"
  - "GitHub Actions"
  - "Docker"
topicIds:
  - "ai-agent-sandboxing-cmeqor"
  - "github-actions-7tcwgt"
  - "docker-3aqwnh"
sourceUrls:
  - "https://www.docker.com/blog/running-ai-agents-in-github-actions-with-docker-sandboxes/"
---

- GitHub Agentic Workflows (gh-aw) 在版本 0.82.9 中新增支持 Docker Sandbox 作为代理运行时。
- Docker Sandbox 在 GitHub Actions 中作为微虚拟机运行，拥有自己的私有 Docker 守护进程，从而将代理与宿主机隔离。
- 配置 Docker Sandbox 需要在工作流 Markdown frontmatter 中设置 `sandbox.agent.runtime` 为 `docker-sbx`。
- 使用 Docker Sandbox 需要 Docker 凭据（`DOCKER_USERNAME` 和 `DOCKER_PAT`），并启用“允许 GitHub Actions 创建和批准拉取请求”的仓库设置。
