---
decisionKey: "42b5e5548a70b0156dc30e47345ec0680f8aa50d0af0fc3a45e340dc8dfab35a"
language: "zh-CN"
title: "DuckDB v2.0 预览引入原生客户端/服务器模式及稳定 C API"
summary: "DuckDB v2.0 预览版带来了原生客户端/服务器模式、稳定 C API 和自定义扩展仓库等重大架构变化，为部署和扩展开发提供了新的可能性。"
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

- DuckDB v2.0 预览版通过 quack 协议扩展和新的 CONNECT SQL 语句引入原生客户端/服务器模式，使 DuckDB 实例可作为守护进程运行并接受网络连接。
- 引入版本化 C API，具有 YAML 定义的规范和稳定的 ABI 保证，使扩展可一次构建并跨次要和补丁更新运行。
- 支持定义、加密固定和自托管自定义扩展仓库，可通过 CREATE EXTENSION REPOSITORY 和 INSTALL 等 SQL 语句从私有仓库安装扩展。
- VARIANT 类型达到完全成熟，可自动检测半结构化模式并将类似 JSON 的数据从磁盘到 Parquet 分片为列式表示，无需显式模式。
- 实现跨云对象存储（如 Amazon S3）的异步 I/O、分区感知查询计划以及通过默认 DICT_FSST 字典优化字符串压缩。
- 存储格式引入延迟列元数据加载和针对自适应基数树（ART）索引的增量检查点清理。
- 用自定义 PEG 语法替换传统的 PostgreSQL 派生解析器，支持扩展注册自定义 SQL 语法，并提供准确的诊断源位置。
- 添加原生 BEFORE 和 AFTER 触发器及转换表、用于向量工作负载的 APPROX NEAREST 相似性连接以及 CTE 内的 DML 表达式。
- 解耦外部 ICU 依赖，用紧凑的原生 IANA 支持子系统替换时区和排序规则逻辑，以减少二进制占用并加快时间转换。
