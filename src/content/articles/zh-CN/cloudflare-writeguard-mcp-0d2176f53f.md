---
decisionKey: "0d2176f53f336e7b9175b9ce4d79628de506ffbac377841477d71af4d88851a9"
language: "zh-CN"
title: "Cloudflare WriteGuard 为 MCP 服务器引入细粒度安全控制"
summary: "Cloudflare 推出 WriteGuard 私有测试版，为 MCP 服务器提供集中式策略、身份归属和审计层。该工具可拦截请求、评估风险等级并记录审计事件，无需修改服务器。"
publishedAt: "2026-08-19T03:13:51.491Z"
score: 0.9
topics:
  - "Security"
  - "AI Agents"
  - "MCP"
topicIds:
  - "security-1jtharf"
  - "ai-agents-1bsn16v"
  - "mcp-1kiasf7"
sourceUrls:
  - "https://www.infoq.com/news/2026/08/cloudflare-writeguard-mcp-safety/"
---

- Cloudflare 正在推出 WriteGuard，目前处于私有测试阶段，为 MCP 服务器提供细粒度安全控制，充当共享策略、归属和审计层。
- WriteGuard 位于 Cloudflare 的 MCP 服务器门户之后，拦截所有传入的 MCP 请求，并根据工具特定策略评估，阻止或允许请求，而无需更改 MCP 服务器本身。
- 每个工具分配一个风险等级，从只读到关键不等，例如完成合并请求为关键，添加评论为最小。
- WriteGuard 使用现有 OAuth 凭据识别用户，避免独立代理账户，并添加 MCP 客户端和会话上下文以实现可审计性。
- WriteGuard 将每次调用分类为成功、失败或阻止，并异步发送经过清洗的审计事件到内部审计 Worker，省略敏感值。
