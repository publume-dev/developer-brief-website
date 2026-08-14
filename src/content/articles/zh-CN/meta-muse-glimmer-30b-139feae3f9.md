---
decisionKey: "139feae3f9bb456f6b1ca814aa18f382b7e679219d31db4a7d7222c55bb5884a"
language: "zh-CN"
title: "Meta 开源 Muse Glimmer：面向端侧执行的 30B 参数智能体模型"
summary: "Meta 发布了 Muse Glimmer，一个 30B 参数的开源模型，采用 Apache 2.0 许可，专为端侧智能体工作流设计，内存占用降至约 17-20GB，可在消费级 GPU 上运行。该模型支持多种框架，并通过投机解码实现最高 3.1 倍生成吞吐量提升。"
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

- Meta 发布了 Muse Glimmer，一个 30B 参数的开源模型（Apache 2.0），用于消费级 GPU 上的本地智能体工作流。
- 该模型采用动态 4 位量化（K-Quant），内存占用降至约 17-20GB，可在 24-32GB GPU/NPU 上运行。
- 与 DFlash 草稿模型结合实现投机解码，在 Apple Silicon 和 RTX 5090 上生成吞吐量最高提升 3.1 倍。
- 训练流程包括 logit 蒸馏、长上下文序列的中期训练，以及 SFT、on-policy 蒸馏和 RL 的后训练对齐。
- 模型包含一个 1.8B 感知编码器，用于处理截图和图表等交错多模态输入。
- 支持 OpenClaw 等智能体框架，可调节推理力度，并在工具执行期间具备失败恢复能力。
- 在 SWE-Bench、DeepSearch QA、τ-Bench 和 MCP-Atlas 基准上，与 Gemma 4 31B 和 Qwen 3.6 27B 等模型相比表现出色。
- 权重已上传至 Hugging Face，支持 llama.cpp、ExecuTorch、Apple MLX、Ollama、LM Studio、vLLM 和 TorchTitan 微调。
