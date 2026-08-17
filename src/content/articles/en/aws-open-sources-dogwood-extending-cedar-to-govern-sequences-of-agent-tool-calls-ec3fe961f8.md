---
decisionKey: "ec3fe961f89fd5beff499d8d667bf8dbdfb1c42e41c412b8f9d116667c5742c6"
language: "en"
title: "AWS Open-Sources Dogwood, Extending Cedar to Govern Sequences of Agent Tool Calls"
summary: "AWS open-sourced Dogwood, a policy language extending Cedar to govern agent tool-call sequences, adding temporal conditions on event history."
publishedAt: "2026-08-17T03:15:51.896Z"
score: 0.85
topics:
  - "Agent Policy"
  - "Open Source"
  - "Authorization"
topicIds:
  - "agent-policy-jts638"
  - "open-source-17ixijy"
  - "authorization-14ahghq"
sourceUrls:
  - "https://www.infoq.com/news/2026/08/aws-dogwood-agent-policy/"
---

- AWS open-sourced Dogwood under Apache 2.0, a policy language for agent tool calls that extends Cedar with temporal conditions.
- Dogwood adds a second clause type where conditions can use `when temporal` to read the agent's event history.
- Temporal conditions are translated into a Cedar context field, with four operators: `formerly`, `count_within`, `count_distinct_within`, and `sum_within`.
- AWS warns that rate limits based on response events can be defeated by concurrency, recommending policies based on request events.
- Temporal conditions do not support Cedar's automated reasoning analysis tools, and evaluation time depends on event log length.
- Dogwood is backward compatible: any valid Cedar policy is also a valid Dogwood policy.
- The reference interpreter is for exploring and testing, not for production authorization.

The limitation on temporal conditions means existing Cedar workflows that rely on automated reasoning need adjustment.

Future roadmap items such as absolute-time windows and liveness properties are not yet implemented and lack detail.
