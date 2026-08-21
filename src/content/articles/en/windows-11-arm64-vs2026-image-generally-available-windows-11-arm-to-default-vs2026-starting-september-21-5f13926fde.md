---
decisionKey: "5f13926fde456e4be68a8232351830f25af03e6d793b7285e3229f4d8a97c32d"
language: "en"
title: "Windows 11 arm64 VS2026 image generally available: windows-11-arm to default VS2026 starting September 21"
summary: "GitHub announced that the Windows 11 arm64 image with Visual Studio 2026 is now generally available on standard and larger hosted runners. Starting September 21, 2026, the windows-11-arm image will gradually switch to VS2026, which may break workflows depending on VS2022."
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

- **Change**: Windows 11 arm64 image with Visual Studio 2026 is now generally available on standard and larger GitHub-hosted runners.
- **Usage**: Update your workflow file to `runs-on: windows-11-vs2026-arm` to use the new image.
- **Effective time**: Starting September 21, 2026, the `windows-11-arm` image will gradually update to use Visual Studio 2026 by default, completing by September 30, 2026.
- **Unchanged condition**: The `windows-11-arm` image remains available, but its default version will change.

Workflows that depend on Visual Studio 2022 may break after the migration; test in advance and optionally pin the runner label to control the switch timing.
