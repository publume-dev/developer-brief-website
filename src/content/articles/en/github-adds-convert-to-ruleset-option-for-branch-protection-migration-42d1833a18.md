---
decisionKey: "42d1833a18985a9f8da716ca486cd17ed82c00e3781e1e23c7e31be44fb3080b"
language: "en"
title: "GitHub adds Convert to ruleset option for branch protection migration"
summary: "GitHub repository admins can now convert classic branch protection rules into repository rulesets, carrying over required reviews, status checks, and push restrictions. This provides a migration path to rulesets' cross-branch patterns, rule layering, and finer-grained bypass controls."
publishedAt: "2026-08-12T05:45:50.677Z"
score: 0.9
topics:
  - "GitHub"
  - "Repository Management"
  - "Developer Tooling"
topicIds:
  - "github-9o7vw2"
  - "repository-management-lf9x50"
  - "developer-tooling-q9uwan"
sourceUrls:
  - "https://github.blog/changelog/2026-08-11-automatically-migrate-branch-protection-rules-to-repository-rulesets"
---

- GitHub added a **Convert to ruleset** option in repository settings for converting an existing branch protection rule into a repository ruleset.
- The conversion maps branch protection configuration, including required reviews, status checks, and push restrictions, into equivalent ruleset rules.
- The option is available for all repositories where rulesets are available.
- To use it: go to **Settings → Branches**, find the classic rule under **Branch protection rules**, and click **Convert to ruleset**.
- Rulesets add capabilities beyond classic branch protection: applying rules across branches with pattern matching, layering multiple rulesets, managing rulesets at organization or enterprise level, and configuring fine-grained bypass permissions.
- The changelog does not state whether conversion removes the original branch protection rule or whether it can be reversed.
