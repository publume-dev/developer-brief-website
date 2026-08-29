---
decisionKey: "2f65f81f2d1565648f8da4823a5005eef63fcbb944bb4e8b0023508843f7eaec"
language: "en"
title: "FreeToken Open-Source Inference Engine Runs Frontier MoE Models on Consumer Hardware via Dynamic Co-Execution"
summary: "UC Berkeley and MIT have released FreeToken, an open-source inference engine that enables frontier MoE models to run on consumer hardware through dynamic co-execution, with concrete performance figures on various GPUs."
publishedAt: "2026-08-29T12:02:34.357Z"
score: 0.8
topics:
  - "Mixture-of-Experts Inference"
  - "Edge AI"
  - "Open-Source Tooling"
topicIds:
  - "mixture-of-experts-inference-1mfby4c"
  - "edge-ai-107qm9e"
  - "open-source-tooling-1v157t7"
sourceUrls:
  - "https://www.infoq.com/news/2026/08/freetoken-local-inference/"
---

- FreeToken is an open-source inference engine from UC Berkeley and MIT enabling frontier MoE models on consumer hardware via dynamic co-execution.\n- It uses a q* policy to split token computation between CPU and GPU based on real-time interconnect throughput, avoiding GPU stalls during expert offloading.\n- Benchmarks show Qwen3.6-35B at ~39 tokens/sec on an 8GB RTX 4060 laptop, DeepSeek-V4-Flash (284B) on an RTX 5090, and GLM-5.2 (753B) on a single workstation GPU.\n- Supports NVIDIA RTX 30, 40, and 50 series GPUs on Linux and Windows, with CLI and desktop client available.

If benchmarks are reproducible, FreeToken could offer a new high-performance option for local MoE inference, particularly on memory-constrained consumer hardware.
