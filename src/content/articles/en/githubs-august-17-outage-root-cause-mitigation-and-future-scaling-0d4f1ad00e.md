---
decisionKey: "0d4f1ad00e262db220e1af06239ff7c802627b76980aff7194f216da623ce330"
language: "en"
title: "GitHub's August 17 Outage: Root Cause, Mitigation, and Future Scaling"
summary: "GitHub suffered a 7-hour 47-minute outage impacting core services, caused by a critical infrastructure component failing to scale with a new traffic peak. GitHub has implemented immediate mitigations and plans a linear read scaling architecture. "
publishedAt: "2026-08-21T14:06:07.365Z"
score: 0.9
topics:
  - "Incident Response"
  - "Platform Reliability"
  - "Capacity Planning"
topicIds:
  - "incident-response-ld2rq6"
  - "platform-reliability-jp0p8i"
  - "capacity-planning-brpogi"
sourceUrls:
  - "https://github.blog/news-insights/company-news/the-august-17-outage-and-the-work-ahead/"
---

- On August 17, GitHub experienced a 7-hour 47-minute outage affecting github.com, authentication, Actions, APIs, PRs, issues, and Copilot.
- The root cause was a critical infrastructure component in the Central US data center failing to scale with a new traffic peak, leading to capacity pressure and cascading failures.
- Recovery involved rerouting traffic, isolating affected infrastructure, and mitigating a client-side retry loop in Copilot services that increased traffic during recovery.
- Since reliability commitments earlier this year, GitHub has added over 3 million CPU cores, 120 petabytes of high-speed storage, and significant network capacity.
- Azure now serves approximately 58% of GitHub's platform load and half of all Git operations, up from 12% in May.
- GitHub's next milestone is an architecture that scales read capacity linearly with the number of readers, enabling unlimited read operations, rolled out gradually starting with the largest monorepos.
- Immediate changes include applying consistent retry limits, retry budgets, and variable timeouts across service-to-service interactions, and reviewing lower-priority CPU and memory alerts.
