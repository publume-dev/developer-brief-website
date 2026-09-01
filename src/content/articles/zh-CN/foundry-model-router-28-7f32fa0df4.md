---
decisionKey: "7f32fa0df4bf1da5ce9fc2a2f0ed7282d1efaf2340dfa24d3960afe99b05e203"
language: "zh-CN"
title: "Foundry Model Router 从两个区域扩展至 28 个，模型池更新"
summary: "微软将 Foundry Model Router 从两个区域扩展到 28 个（全球标准部署）和 21 个（数据区部署），并更新了模型池，新增 Claude Opus 4.8 和 GPT-5.6 系列，移除了生命周期结束的模型。"
publishedAt: "2026-09-01T12:05:09.734Z"
score: 0.9
topics:
  - "Azure Foundry"
  - "Model Routing"
  - "LLM Deployment"
topicIds:
  - "azure-foundry-epv4bl"
  - "model-routing-1wo1oy8"
  - "llm-deployment-1qs2k9r"
sourceUrls:
  - "https://www.infoq.com/news/2026/08/foundry-model-router-regions/"
---

- 扩展区域：全球标准部署从 2 个区域（East US 2、Sweden Central）增至 28 个，数据区部署为 21 个。
- 模型池变化：新增 Anthropic Claude Opus 4.8 和 GPT-5.6 系列；移除 gpt-5-chat、gpt-5.2-chat、gpt-5.3-chat 和 DeepSeek-V3.1（生命周期结束）。
- 配置影响：使用默认配置的团队自动获得模型池变化，无需重新部署；配置了模型子集的团队不会自动获得，新模型默认排除，需显式添加。
- 路由模式：三种模式——Balanced（默认）、Quality（适合法律审查、医学摘要、复杂推理）、Cost（适合高量分类和简单问答）；更改模式或子集最长需五分钟生效。
- 上下文窗口：有效上下文窗口为池中最小模型的窗口，添加更小模型会降低所有请求的上限。
- 路由决策仅基于文本：支持视觉输入，但图像不影响模型选择；不支持音频。
- Claude 模型需先在同一个 Foundry 账户中单独部署匹配的 SKU，否则在子集中引用会报 InvalidResourceProperties 错误。
- Azure Policy：路由器在部署时强制执行内置政策，允许的发布者列表必须包含 Microsoft 及池中所有模型的发布者。
- 可审计性：每个响应在 model 字段中标识所选模型。
- 建议：将初始部署视为起点，在生产流量前进行基准测试；微软提供开源评估管道用于质量、成本和延迟评估。
