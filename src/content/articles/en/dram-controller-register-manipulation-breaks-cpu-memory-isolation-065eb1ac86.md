---
decisionKey: "065eb1ac86251bbc373414417dfebeab32d9a5435a1624e29a9c77aa3d702200"
language: "en"
title: "DRAM Controller Register Manipulation Breaks CPU Memory Isolation"
summary: "The open-source hardware security project skitter-creek-bath-salts breaks CPU memory isolation on AMD Family 14h, 15h, and 16h processors by manipulating DRAM memory controller translation registers. The attack poses risks to bare-metal cloud and confidential computing environments."
publishedAt: "2026-08-23T13:44:57.509Z"
score: 0.8
topics:
  - "Hardware Security"
  - "Memory Isolation"
  - "AMD Processors"
topicIds:
  - "hardware-security-195i7r1"
  - "memory-isolation-1c5algm"
  - "amd-processors-ntkzdi"
sourceUrls:
  - "https://www.infoq.com/news/2026/08/amd-memory-exploit/"
---

- Christopher Domas unveiled skitter-creek-bath-salts, an open-source hardware security project that manipulates DRAM memory controller translation registers to break CPU memory isolation on AMD Family 14h, 15h, and 16h processors.
- The exploit targets memory controller registers such as BankSwizzleMode to alter physical-to-DRAM address mappings, allowing unprivileged (Ring 0) software to access protected memory regions like SMM RAM, PSP firmware tables, CC6 sleep save areas, and microcode patch buffers without triggering architectural memory fences.
- The attack requires Ring 0 privileges and primarily targets older AMD Family 15h and 16h processors, posing risks to bare-metal cloud and confidential computing environments.

The vulnerability may affect bare-metal cloud services and confidential computing environments based on AMD Family 15h and 16h processors, as an attacker with Ring 0 privileges can break memory isolation.

Since primary sources, such as the project repository or Domas's talk details, are missing, further verification is needed. Future attention should be on official project releases or patches.
