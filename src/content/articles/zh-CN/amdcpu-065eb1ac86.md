---
decisionKey: "065eb1ac86251bbc373414417dfebeab32d9a5435a1624e29a9c77aa3d702200"
language: "zh-CN"
title: "AMD内存控制器寄存器操纵打破CPU内存隔离"
summary: "公开的硬件安全项目skitter-creek-bath-salts通过操纵DRAM内存控制器翻译寄存器，打破了AMD Family 14h、15h和16h处理器的CPU内存隔离。这一攻击对裸机云和机密计算环境构成风险。"
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

- Christopher Domas发布了skitter-creek-bath-salts，一个开源硬件安全项目，操纵DRAM内存控制器翻译寄存器以打破AMD Family 14h、15h、16h处理器的CPU内存隔离。
- 该漏洞针对如BankSwizzleMode等内存控制器寄存器，改变物理地址到DRAM地址的映射，从而允许无特权（Ring 0）软件访问受保护内存区域，如SMM RAM、PSP固件表、CC6休眠保存区域和微码补丁缓冲区，而无需触发架构内存屏障。
- 该攻击需要Ring 0特权，主要针对较旧的AMD Family 15h和16h处理器，对裸机云和机密计算环境构成风险。

该漏洞可能影响基于AMD Family 15h和16h处理器的裸机云服务以及机密计算环境，因为攻击者获得Ring 0权限后即可破坏内存隔离。

由于缺乏主要来源，如项目仓库或演讲详情，需进一步验证。后续应关注官方项目发布或补丁。
