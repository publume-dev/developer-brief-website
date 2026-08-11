---
decisionKey: "8c635bc3d801896d76dc40a182b71fd3350afb3bf48b012d4a91a10cd9d6891b"
language: "en"
title: "Pinterest Centralizes AWS Terraform Pipelines With RPP"
summary: "Pinterest's Resource Provisioner Pipeline centralizes AWS Terraform execution so multi-repository infrastructure changes get least-privilege access and dual-control reviews. It turns plan and apply into separately auditable PR steps instead of relying on per-repo CI setups."
publishedAt: "2026-08-11T18:42:58.614Z"
score: 0.8
topics:
  - "Terraform"
  - "AWS"
  - "CI/CD"
  - "Security"
topicIds:
  - "terraform-16y9a1j"
  - "aws-7brv06"
  - "ci-cd-9jk1ml"
  - "security-1jtharf"
sourceUrls:
  - "https://www.infoq.com/news/2026/08/pinterest-secures-aws-infra/"
---

- Pinterest revealed the Resource Provisioner Pipeline (RPP), a centralized Terraform execution engine for AWS infrastructure that enforces least-privilege access and dual-control reviews.
- RPP runs as a central set of composite GitHub Actions on GitHub pull request events, splitting a PR into separate plan/apply runs for each affected Terraform workspace.
- It uses a chained-role model: the workflow first assumes a central RPPActionsRole validated via OIDC, reads a source-of-truth config mapping workspaces to repositories and IAM roles, and before assuming the workspace-specific team role verifies that the Terraform code path matches the workspace's S3 backend and KMS key.
- Terraform changes require sign-off from an approved reviewer on the owning repository, and applies are triggered only by a clear human comment on the PR, keeping plan and apply as separate auditable actions.
- The centralized pipeline provides a single control point for systemic fixes and runs consistent PR-triggered checks including static analysis with custom Semgrep rules, AI-assisted scanning, and optional LocalStack-based dry runs.
- RPP is a private system and not open-source.
- Reporting caveat: InfoQ's article does not provide the original Pinterest blog post or talk, so these details are not independently verified against the primary source.
