---
decisionKey: "139feae3f9bb456f6b1ca814aa18f382b7e679219d31db4a7d7222c55bb5884a"
language: "en"
title: "Meta Open-Sources Muse Glimmer: A 30B Local Agentic Model Optimized for On-Device Execution"
summary: "Meta released Muse Glimmer, a 30-billion-parameter open-source model under Apache 2.0, designed for local agentic workflows on consumer GPUs, with memory footprint reduced to roughly 17-20 GB. The model supports various frameworks and achieves up to 3.1x generation throughput via speculative decoding."
publishedAt: "2026-08-14T05:45:30.156Z"
score: 0.86
topics:
  - "Open-Source Models"
  - "Local AI"
  - "Agentic Workflows"
  - "Model Optimization"
  - "Developer Tooling"
topicIds:
  - "open-source-models-144e1ap"
  - "local-ai-sw65y"
  - "agentic-workflows-u2ior8"
  - "model-optimization-bcqrrv"
  - "developer-tooling-q9uwan"
sourceUrls:
  - "https://www.infoq.com/news/2026/08/meta-muse-glimmer/"
---

- Meta released Muse Glimmer, a 30-billion-parameter open-weight model under Apache 2.0, for local agentic workflows on consumer GPUs.
- Dynamic 4-bit quantization (K-Quant) reduces memory to roughly 17-20 GB, enabling execution on 24-32 GB GPUs/NPUs.
- Pairs with a DFlash drafter model for speculative decoding, achieving up to 3.1x generation throughput on Apple Silicon and RTX 5090.
- Training pipeline includes logit distillation, mid-training on long-context sequences, and post-training alignment with SFT, on-policy distillation, and RL.
- Includes a 1.8B perception encoder for interleaved multimodal inputs such as screenshots and diagrams.
- Supports agent frameworks like OpenClaw, adjustable reasoning effort, and handles failure recovery during tool execution.
- Benchmarks on SWE-Bench, DeepSearch QA, τ-Bench, and MCP-Atlas show strong performance versus models like Gemma 4 31B and Qwen 3.6 27B.
- Weights are on Hugging Face, with support for llama.cpp, ExecuTorch, Apple MLX, Ollama, LM Studio, vLLM, and TorchTitan for fine-tuning.
