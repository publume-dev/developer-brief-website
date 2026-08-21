---
decisionKey: "a7a6c274d17612670732a1fec48d948a833db3ab7393b0ae1c58c79a7136b4d6"
language: "en"
title: "S3 Compatibility Doesn't Guarantee S3-Level Security"
summary: "A Wiz security review found significant differences in public access controls, key formats, and IAM semantics between S3-compatible object storage services and AWS S3. These discrepancies can lead to security gaps that developers should consider when choosing a service."
publishedAt: "2026-08-21T14:06:07.365Z"
score: 0.8
topics:
  - "Object Storage Security"
  - "S3 Compatibility"
  - "Cloud Security"
topicIds:
  - "object-storage-security-9zfrfz"
  - "s3-compatibility-qsk0wf"
  - "cloud-security-1s5iwhw"
sourceUrls:
  - "https://www.infoq.com/news/2026/08/s3-clone-security/"
---

- Many S3-compatible services lack AWS S3's Block Public Access and other security controls: Nebius and Cloudflare R2 allow public buckets but not anonymous listing; DigitalOcean supports publicly listable buckets; Vultr supports both ACLs and bucket policies.
- Crusoe and Lambda Labs lack public-access capabilities entirely, and some services provide fewer protections than AWS S3's Block Public Access.
- Access keys for S3-compatible services often lack the structured formats and secret-scanning patterns that AWS keys have, making them harder for tools like GitHub to detect.
- IAM capabilities and semantics differ among S3-compatible implementations, with past vulnerabilities in MinIO (privilege escalation) and RustFS (tenant isolation) illustrating the risks.
- Wiz's review did not cover Backblaze B2, Wasabi, or Google Cloud Storage.

Developers evaluating S3-compatible services should review their security features, especially public access controls and key management, and consider differences in IAM semantics.
