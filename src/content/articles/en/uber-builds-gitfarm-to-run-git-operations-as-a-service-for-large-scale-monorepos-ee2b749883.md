---
decisionKey: "ee2b749883519114682ac4d5f3f81d3bd3db2780daed4267acdfa78aad82b7c2"
language: "en"
title: "Uber Builds GitFarm to Run Git Operations as a Service for Large-Scale Monorepos"
summary: "Uber has developed GitFarm, a Git-as-a-service platform that centralizes Git operations on backend clusters, eliminating the need for client-side local clones and cutting cold-start times for large monorepos. The service is already in production and shows significant performance improvements."
publishedAt: "2026-08-28T21:50:05.617Z"
score: 0.85
topics:
  - "Git Infrastructure"
  - "Monorepo"
  - "Uber Engineering"
topicIds:
  - "git-infrastructure-1a46aiq"
  - "monorepo-17t0ptq"
  - "uber-engineering-1rropw2"
sourceUrls:
  - "https://www.infoq.com/news/2026/08/uber-gitfarm-git-as-a-service/"
---

- GitFarm is a Git-as-a-service platform that runs Git operations on centralized backend clusters, removing the need for client systems to maintain local repository clones.
- It provides full Git checkouts in under 500 milliseconds, compared with historical 10- to 15-minute host-level cold starts for cloning large monorepos like Uber's Go monorepo.
- It uses pre-warmed checkouts and sandbox pooling to reduce the overhead of providing a ready-to-use checkout to less than a second.
- A code ownership service at Uber eliminated local checkouts across six hosts after adopting GitFarm, reducing CPU from over 70 cores to 16 and memory from 400 GB to 32 GB, and cutting startup time from 15-20 minutes to under one minute.
- A compliance auditing service processing 10,000-20,000 events per hour across 9,000 repositories reduced median latency from 110-160 seconds with Buildkite to 20-30 seconds with GitFarm.
- GitFarm has been in production since early 2025 and its roadmap includes streaming Git output, sparse checkouts, bare workspaces, longer-lived sessions, repository mirroring, and SubmitQueue integration.
