---
decisionKey: "6dd48e1a9a9c326e05a00e5dc4d10bc00876d992a17e7c31a4362c3c3a753d97"
language: "en"
title: "GitHub Copilot for JetBrains adds Copilot memory, Ollama BYOK, and enterprise settings"
summary: "The latest GitHub Copilot for JetBrains release adds persistent Copilot memory, Ollama as a bring-your-own-key provider, and server-managed enterprise settings. The update also adds automatic CLI installation, Codex workflow changes, and reliability fixes for MCP and terminal behavior."
publishedAt: "2026-08-12T05:45:50.677Z"
score: 0.9
topics:
  - "GitHub Copilot"
  - "JetBrains IDEs"
  - "Developer Tooling"
topicIds:
  - "github-copilot-mbl6jy"
  - "jetbrains-ides-1frks8e"
  - "developer-tooling-q9uwan"
sourceUrls:
  - "https://github.blog/changelog/2026-08-11-copilot-memory-and-ollama-in-github-copilot-for-jetbrains"
---

- Enterprise managed settings: administrators can now control plugin availability, MCP server access, permission bypass behavior, and OpenTelemetry settings from the server.
- Copilot memory: Copilot memory can retain and recall project details and preferences across agent chat sessions in JetBrains, toggled from the Copilot Memory setting in the Copilot settings portal.
- Ollama BYOK: Ollama is now available as a BYOK provider in GitHub Copilot for JetBrains, with provider configuration and model selection supported throughout the JetBrains experience.
- CLI auto-install: Copilot CLI can now be installed automatically from integrated terminals on macOS, Linux, and Windows.
- Codex workflows: Codex sessions now appear in agent debug logs, and Codex workflows support updated permission modes plus customizations through instructions and skills.
- References and debug entry: File and folder # references are restored in Copilot, Claude, and Codex chat inputs, and the agent debug logs button moved to the Options dropdown.
- Reliability improvements: Updated reliability for MCP execution and approvals, terminal output and auto-approval, customizations, cloud agents, and diff-based editing, plus fixes for ANSI escape rendering and terminal scrollbar predictability.
