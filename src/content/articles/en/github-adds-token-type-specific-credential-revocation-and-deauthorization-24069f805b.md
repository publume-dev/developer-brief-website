---
decisionKey: "24069f805b2264f5d16cd88d9c46862443bcfec417990dcb13b5672b1a81d2f4"
language: "en"
title: "GitHub adds token-type-specific credential revocation and deauthorization"
summary: "GitHub now supports token-type- and user-specific revocation and deauthorization of user credentials, providing finer-grained control than the previous all-at-once kill switch to contain the blast radius of a compromise."
publishedAt: "2026-08-19T03:13:51.491Z"
score: 0.9
topics:
  - "GitHub"
  - "Security"
  - "Credential Management"
  - "Incident Response"
  - "REST API"
topicIds:
  - "github-9o7vw2"
  - "security-1jtharf"
  - "credential-management-ncfjr7"
  - "incident-response-ld2rq6"
  - "rest-api-15i9t07"
sourceUrls:
  - "https://github.blog/changelog/2026-08-18-credential-revocation-and-deauthorization-by-token-type"
---

- Supports token-type-specific and user-specific deauthorization and revocation of user credentials during security incidents, providing finer-grained control than the previous all-at-once kill switch.
- Enterprise owners, organization admins, and members with the Manage enterprise credentials permission can revoke all tokens of a specific credential type (e.g., Personal access tokens, SSH keys, OAuth app tokens, or GitHub App user access tokens) to contain the blast radius of a compromise.
- New token-type-specific bulk deauthorization allows revoking all SSO authorizations for a specific credential type across the enterprise or for a specific user from the UI or enterprise REST APIs.
- Token-type specific bulk revocation can delete or revoke all user-level credentials of a specific type, e.g., deleting all personal access tokens for an individual EMU user without touching SSH keys.
- All bulk credential-revocation actions previously available at the enterprise level are now available at the organization level through both the web UI and organization REST APIs.
- All deauthorization and revocation actions are captured in the audit log, with email notifications to affected users.

Security teams can now quickly revoke credentials by token type or user during incident response, reducing the risk of unintended disruption and containing the blast radius.

The changelog does not specify whether this feature is available on GitHub Enterprise Server or only on GitHub.com; affected version users should check official documentation.
