---
decisionKey: "909d22012ee9e441ffb80d28b9d4483796366b795abb82ca9dbdc9553b389ed2"
language: "en"
title: "Spotify Introduces Random Access Parquet to Enable Low-Latency Point Queries on Its Data Lake"
summary: "Spotify unveiled Random Access Parquet (RAP), a storage architecture that lets point queries run directly on data lake data without duplication. The design preserves analytics capability while boosting lookup performance."
publishedAt: "2026-08-12T15:30:42.918Z"
score: 0.85
topics:
  - "Data Engineering"
  - "Data Lake"
  - "Apache Iceberg"
topicIds:
  - "data-engineering-cqrk2u"
  - "data-lake-18bx0pw"
  - "apache-iceberg-h1oyqe"
sourceUrls:
  - "https://www.infoq.com/news/2026/08/spotify-data-lake-point-queries/"
---

- Spotify introduced Random Access Parquet (RAP), a storage architecture that enables low-latency point queries directly against data in its data lake without replicating to operational databases.
- RAP adds an external indexing layer over Apache Parquet files, allowing interactive lookups while retaining analytics and AI compatibility.
- The index maps lookup keys directly to Parquet files and row locations, avoiding full scans and enabling targeted ranged reads.
- As new data is written into Iceberg tables, an index builder generates append-only index fragments without modifying immutable Parquet files.
- Storage layout optimizations include sorting by lookup key, grouping related records, interleaving value columns, and covering indexes, enabling some point queries via a single ranged read of a few kilobytes.
- RAP supports secondary indexes for multiple lookup dimensions, such as buyer ID or seller ID, with hash-based indexes for exact lookups and sorted indexes for range queries.
