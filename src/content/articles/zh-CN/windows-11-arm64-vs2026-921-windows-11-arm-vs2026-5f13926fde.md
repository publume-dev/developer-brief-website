---
decisionKey: "5f13926fde456e4be68a8232351830f25af03e6d793b7285e3229f4d8a97c32d"
language: "zh-CN"
title: "Windows 11 arm64 VS2026 镜像正式发布：9月21日起 windows-11-arm 将逐步默认 VS2026"
summary: "GitHub 宣布 Windows 11 arm64 版 Visual Studio 2026 镜像现已正式在标准及更大规格的 GitHub 托管运行器上可用。自 2026 年 9 月 21 日起，windows-11-arm 镜像将逐步切换至 VS2026，可能导致依赖 VS2022 的工作流中断。"
publishedAt: "2026-08-21T14:06:07.365Z"
score: 0.85
topics:
  - "GitHub Actions"
  - "Windows"
  - "Visual Studio"
topicIds:
  - "github-actions-7tcwgt"
  - "windows-1n9htyi"
  - "visual-studio-xicopd"
sourceUrls:
  - "https://github.blog/changelog/2026-08-20-windows-11-arm64-vs2026-image-generally-available"
---

- **变更**：Windows 11 arm64 镜像现已正式支持 Visual Studio 2026，适用于标准及更大规格的 GitHub 托管运行器。
- **使用方式**：将工作流文件中的 `runs-on` 更新为 `windows-11-vs2026-arm` 即可使用新镜像。
- **生效时间**：自 2026 年 9 月 21 日起，`windows-11-arm` 镜像将逐步更新为默认使用 Visual Studio 2026，预计于 2026 年 9 月 30 日完成。
- **未变条件**：`windows-11-arm` 镜像仍保持可用，但默认版本将变更。

依赖 Visual Studio 2022 的工作流可能在迁移后中断，请提前测试并在适当时间手动指定运行器标签以控制切换时机。
