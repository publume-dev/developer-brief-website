---
decisionKey: "b1ab4d78127b1453adf5b28eb0f317fc30d78a14584b595ab7afd79fd91bc765"
language: "en"
title: "Copilot Code Review Reaches Azure Repos, Billed Per Review with Reporting Two Days Behind"
summary: "GitHub Copilot code reviews are now available to all Azure DevOps customers without sign-up, billed per review, with onboarding controls at multiple levels."
publishedAt: "2026-09-04T12:05:05.180Z"
score: 0.85
topics:
  - "Azure DevOps"
  - "GitHub Copilot"
  - "Code Review"
  - "Developer Tooling"
  - "Billing"
topicIds:
  - "azure-devops-pjzhht"
  - "github-copilot-mbl6jy"
  - "code-review-ig4nr4"
  - "developer-tooling-q9uwan"
  - "billing-i5mxng"
sourceUrls:
  - "https://www.infoq.com/news/2026/09/copilot-code-review-azure-repos/"
---

- GitHub Copilot code review is now available to all Azure DevOps customers without sign-up, previously gated since June; it posts review comments on pull requests and bills per review through the linked Azure subscription, with usage reporting delayed by 48 hours.
- The August release adds onboarding controls at organization, project, and repository level, supports Managed DevOps Pools, custom instructions (with path-level targeting), and automatic reviews via branch policies.
- Charges for Copilot code review appear under 'GitHub Copilot for AzDO' in Azure Cost Management, carrying Azure DevOps project tags, appearing 48 hours after review completion; budgets only notify and do not stop reviews.
- Concurrency limits apply: five concurrent reviews per organization, two per user, and one per pull request. The feature runs on Azure Pipelines infrastructure, using the default agent pool or Managed DevOps Pools with Ubuntu Server; self-hosted agents are not supported.
- Copilot always leaves a 'Comment' review and never approves or requests changes; it does not re-review after new commits unless asked, and does not block merges. Known issues include reviews stopping after the plan-tool phase and being canceled after about 60 minutes, with a fix rolling out over a week.
- Feature limitations: repositories up to 10 GB, pull requests with ≤100 changed files and no merge conflicts, TFVC unsupported, gradual regional rollout over two to three weeks.
