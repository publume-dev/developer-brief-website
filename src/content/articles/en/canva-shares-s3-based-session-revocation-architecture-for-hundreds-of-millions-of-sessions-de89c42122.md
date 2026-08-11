---
decisionKey: "de89c42122a9b80d5bbe4a94f95b62de0a79d4f9149789cc1fbc8461f92d266b"
language: "en"
title: "Canva Shares S3-Based Session Revocation Architecture for Hundreds of Millions of Sessions"
summary: "Canva rearchitected session revocation to store compact immutable records in Amazon S3 and distribute them as in-memory indexes to application gateways, supporting hundreds of millions of active sessions while cutting revocation cache memory use by 87.5%."
publishedAt: "2026-08-11T15:30:50.566Z"
score: 0.9
topics:
  - "Session Management"
  - "Amazon S3"
  - "Authentication Infrastructure"
topicIds:
  - "session-management-1pt6b6u"
  - "amazon-s3-14p3lpp"
  - "authentication-infrastructure-35y6a0"
sourceUrls:
  - "https://www.infoq.com/news/2026/08/canva-session-revocation-scale/"
---

- Canva redesigned session revocation to store compact immutable revocation records in Amazon S3 and distribute them as in-memory indexes to application gateways, supporting hundreds of millions of active sessions.
- Revocation data is divided into 30-minute S3 objects representing a 12-hour window; each revocation is a 16-byte binary record containing a principal and timestamp, and sorted arrays enable direct in-memory search, reducing the revocation cache memory footprint by 87.5%.
- Gateways use conditional GETs to download changed chunks and discard data older than 12 hours; asynchronous workers merge new revocations into the latest chunk and upload with conditional PUTs for optimistic concurrency, with ZooKeeper leader election reducing conflicts but not required for correctness.
- After migration, Canva reduced its session revocation database to two read replicas for redundancy, improved deployment speed, and made database load scale with revocation write throughput and site traffic rather than the number of gateway instances loading the cache.
- Canva reports the worker can process more than 2,000 revocations per second, and a chunk containing one million revocations represents about 16 MB of binary data.
