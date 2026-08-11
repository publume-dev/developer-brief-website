---
decisionKey: "5c8b0150a550506685a64c58aff398b6ae6f6ae777c30e01cb3dfcbdc1226458"
language: "zh-CN"
title: "Copilot 使用情况指标 API 新增按 agent 拆分应用活动"
summary: "GitHub 的 Copilot 使用情况指标 API 现新增一个向后兼容的可选字段 `totals_by_3rd_party_agent`，按单个 agent 拆分应用活动。管理员可据此查看各 agent 的交互次数和会话次数，而无需改动现有报告字段。"
publishedAt: "2026-08-11T15:30:50.566Z"
score: 0.9
topics:
  - "Copilot Usage Metrics"
  - "Agent App Telemetry"
  - "GitHub API"
topicIds:
  - "copilot-usage-metrics-4nqc5l"
  - "agent-app-telemetry-p8zeue"
  - "github-api-1ov684i"
sourceUrls:
  - "https://github.blog/changelog/2026-08-07-copilot-usage-metrics-api-adds-agent-app-activity"
---

- 该 API 现通过新的可选 `totals_by_3rd_party_agent` 数组，按单个 agent 报告应用活动。
- 每个条目包含 `agent_name`、`agent_id`、`user_initiated_interaction_count` 和 `session_count`；`session_count` 仅出现在企业级和组织级汇总报告中。
- 嵌套数组中的 `user_initiated_interaction_count` 统计的是 agent 应用作业启动次数，与同名顶层字段含义不同，不应相加。
- 该变更向后兼容：现有字段结构保持不变；没有可识别的 agent 应用活动时，该数组会被省略。
- 访问权限要求为：企业所有者/账单管理员、组织所有者，或具有 View Copilot Metrics 权限的自定义角色，且必须启用 Copilot 使用情况指标策略。
