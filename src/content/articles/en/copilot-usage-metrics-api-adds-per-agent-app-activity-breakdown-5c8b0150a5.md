---
decisionKey: "5c8b0150a550506685a64c58aff398b6ae6f6ae777c30e01cb3dfcbdc1226458"
language: "en"
title: "Copilot usage metrics API adds per-agent app activity breakdown"
summary: "GitHub's Copilot usage metrics API now includes a backward-compatible `totals_by_3rd_party_agent` array that breaks out agent app activity per agent. Admins can use it to see agent-level interaction counts and session counts without altering existing report fields."
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

- The Copilot usage metrics API now reports agent app activity broken out by individual agent via a new optional `totals_by_3rd_party_agent` array.
- Each entry includes `agent_name`, `agent_id`, `user_initiated_interaction_count`, and `session_count`; `session_count` appears only in aggregated enterprise and organization reports.
- The nested `user_initiated_interaction_count` counts agent app job starts and is distinct from the top-level field of the same name, so the two should not be summed.
- The change is backward compatible: existing fields keep their shape, and the array is omitted when there is no recognized agent app activity.
- Access requires enterprise owner/billing manager, organization owner, or custom role with View Copilot Metrics permission, and the Copilot usage metrics policy must be enabled.
