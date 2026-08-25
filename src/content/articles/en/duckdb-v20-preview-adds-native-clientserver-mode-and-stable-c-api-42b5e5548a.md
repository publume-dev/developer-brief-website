---
decisionKey: "42b5e5548a70b0156dc30e47345ec0680f8aa50d0af0fc3a45e340dc8dfab35a"
language: "en"
title: "DuckDB v2.0 Preview Adds Native Client/Server Mode and Stable C API"
summary: "DuckDB v2.0 preview introduces native client/server mode, a stable C API, and custom extension repositories, reshaping deployment and extension development."
publishedAt: "2026-08-25T14:27:51.056Z"
score: 0.9
topics:
  - "DuckDB v2.0"
  - "Database"
  - "Distribution"
  - "Extension API"
  - "SQL"
topicIds:
  - "duckdb-v2-0-4abr6g"
  - "database-18s5prs"
  - "distribution-elcu97"
  - "extension-api-knf9dm"
  - "sql-1gsjuyn"
sourceUrls:
  - "https://www.infoq.com/news/2026/08/duckdb-v2-distributed/"
---

- DuckDB v2.0 preview introduces a native client/server mode via the quack protocol extension and the new CONNECT SQL statement, allowing DuckDB instances to run as a daemon and accept network connections.
- Introduces a versioned C API with YAML-defined specification and stable ABI guarantees, enabling extensions to be built once and run across minor and patch updates.
- Allows defining, cryptographically pinning, and self-hosting custom extension repositories, with SQL statements such as CREATE EXTENSION REPOSITORY and INSTALL from private repos.
- Brings VARIANT types to full maturity, automatically detecting semi-structured patterns and shredding JSON-like payloads into columnar representations from disk to Parquet without explicit schemas.
- Implements asynchronous I/O across cloud object stores such as Amazon S3, partition-aware query planning, and optimized string compression via default DICT_FSST dictionaries.
- Storage format introduces lazy column metadata loading and incremental checkpoint vacuuming for Adaptive Radix Tree (ART) indexes.
- Replaces the legacy PostgreSQL-derived parser with a custom PEG-based grammar that supports custom SQL syntax registration by extensions and accurate source locations for diagnostics.
- Adds native BEFORE and AFTER triggers with transition tables, APPROX NEAREST similarity joins for vector workloads, and DML expressions inside CTEs.
- Decouples from the external ICU dependency, replacing timezone and collation logic with a compact native IANA-backed subsystem to reduce binary footprint and speed up temporal conversions.
