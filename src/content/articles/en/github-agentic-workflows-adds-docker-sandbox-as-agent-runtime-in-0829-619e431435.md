---
decisionKey: "619e431435330eab06e62c9ee8d934bfe39bf2c2fc42ef551c80377711cdf5ce"
language: "en"
title: "GitHub Agentic Workflows Adds Docker Sandbox as Agent Runtime in 0.82.9"
summary: "GitHub Agentic Workflows (gh-aw) 0.82.9 now supports Docker Sandbox as an agent runtime, offering microVM isolation. The feature requires specific runtime configuration and Docker credentials, along with enabling required GitHub permissions."
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

- GitHub Agentic Workflows (gh-aw) added Docker Sandbox as a supported agent runtime in version 0.82.9.
- Docker Sandbox runs as a microVM with its own private Docker daemon, isolating the agent from the host.
- Configuring Docker Sandbox requires setting `sandbox.agent.runtime` to `docker-sbx` in the workflow Markdown frontmatter.
- Using Docker Sandbox requires Docker credentials (`DOCKER_USERNAME` and `DOCKER_PAT`) and enabling 'Allow GitHub Actions to create and approve pull requests' in repository settings.
