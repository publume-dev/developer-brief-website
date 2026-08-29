---
decisionKey: "2f65f81f2d1565648f8da4823a5005eef63fcbb944bb4e8b0023508843f7eaec"
language: "zh-CN"
title: "FreeToken 开源推理引擎：通过动态 CPU/GPU 协同执行在消费级硬件上运行前沿 MoE 模型"
summary: "UC Berkeley 和 MIT 发布开源推理引擎 FreeToken，通过动态协同执行让消费级 GPU 运行前沿 MoE 模型，并在多种硬件上展示了具体性能数据。"
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

- FreeToken 由 UC Berkeley 和 MIT 开发，是开源推理引擎，支持在消费级硬件上运行前沿 MoE 模型。\n- 它使用 q* 策略根据实时互连吞吐量在 CPU 和 GPU 之间分割 token 计算，避免专家 offloading 期间 GPU 停顿。\n- 基准测试显示，Qwen3.6-35B 在 8GB RTX 4060 笔记本上约 39 tokens/秒，DeepSeek-V4-Flash（284B）在 RTX 5090 上运行，GLM-5.2（753B）可在单工作站 GPU 上运行。\n- 支持 NVIDIA RTX 30、40、50 系列 GPU，兼容 Linux 和 Windows，提供 CLI 和桌面客户端。

若基准测试可复现，FreeToken 可能为本地 MoE 推理提供一种新的高性能选项，尤其对于显存受限的消费级硬件。
