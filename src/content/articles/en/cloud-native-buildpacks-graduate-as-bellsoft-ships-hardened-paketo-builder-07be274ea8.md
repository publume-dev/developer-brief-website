---
decisionKey: "07be274ea8a7d5c8a9929e5c0b639b06b379f4a36341b4f515a9ba9c02447e96"
language: "en"
title: "Cloud Native Buildpacks Graduate as BellSoft Ships Hardened Paketo Builder"
summary: "Cloud Native Buildpacks graduated in the CNCF on 17 July 2026, and BellSoft made its hardened Paketo builder generally available on 21 July 2026, giving teams a rebase-based patching path that skips full rebuilds."
publishedAt: "2026-08-11T18:42:58.614Z"
score: 0.8
topics:
  - "Container Security"
  - "Cloud Native Buildpacks"
  - "Supply Chain Security"
topicIds:
  - "container-security-1ffi472"
  - "cloud-native-buildpacks-uz45a1"
  - "supply-chain-security-1fqvp23"
sourceUrls:
  - "https://www.infoq.com/news/2026/08/buildpacks-dockerfile-patching/"
---

- Cloud Native Buildpacks graduated within the CNCF on 17 July 2026.
- On 21 July 2026, BellSoft announced general availability of a hardened Paketo builder based on Alpaquita Linux.
- The rebase command updates an application image to a newer runtime base image by rewriting the OCI manifest and configuration, bypassing a rebuild.
- Rebase only replaces compatible run-image layers; vulnerabilities in application dependencies still require a rebuild.
- BellSoft's Standard tier advertises a 7-day remediation SLA for critical vulnerabilities and 14 days for others; the free Community tier lists none.
- In December 2025, Docker made its hardened image catalogue free under Apache 2.0, with a Select tier committing to 7-day critical CVE remediation.
