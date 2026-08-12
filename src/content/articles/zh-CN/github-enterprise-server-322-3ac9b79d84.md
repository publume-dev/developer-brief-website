---
decisionKey: "3ac9b79d843cb0b973238e7ca66284fffd4c248c9fe904980b923dba6b8db7f7"
language: "zh-CN"
title: "GitHub Enterprise Server 3.22 候选版现已可用"
summary: "GitHub Enterprise Server 3.22 引入离线环境的 Copilot CLI 支持、Enterprise Teams 正式可用，以及更精细的规则集和审查控制，便于管理员在正式版发布前评估。"
publishedAt: "2026-08-12T05:45:50.677Z"
score: 0.9
topics:
  - "GitHub Enterprise Server"
  - "Release Candidate"
  - "Enterprise Administration"
topicIds:
  - "github-enterprise-server-1q9nybg"
  - "release-candidate-11olwb"
  - "enterprise-administration-t1v3e0"
sourceUrls:
  - "https://github.blog/changelog/2026-08-11-github-enterprise-server-3-22-release-candidate"
---

- GitHub 的变更日志宣布，GitHub Enterprise Server 3.22 候选版（RC）现已可用。
- 管理员可将 Copilot CLI 配置为在无法连接 GitHub Cloud 的隔离或离线 GHES 环境中工作；该能力目前为技术预览，后续可能变化。
- Enterprise Teams 在公开预览后现正式可用（GA），企业所有者可通过集中式团队结构跨组织和仓库管理用户与访问权限。
- 安全分析人员现在可在仓库、组织和企业三个层级，将 secret scanning 的推送保护绕过请求和告警解除请求按日期升序或降序排序。
- 仓库规则集现已支持由单个用户绕过，管理员对规则绕过权限拥有更细粒度的控制。
- 组织所有者和仓库管理员可通过“必需审查者”规则要求拉取请求的指定审查者，并使用模式匹配定位分支、文件和文件夹，还可设置每个团队所需的最少审查人数。
- 开发者可在 issue 侧边栏查看发布状态；当关联的拉取请求被包含在某个发布中时，会出现“Latest release”或“Pre-release”徽章。
- 维护者可以在公共仓库的拉取请求列表视图中看到贡献者角色标签，例如“First-time contributor”、“Contributor”和“Member”。
