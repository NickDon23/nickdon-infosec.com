---
title: "SquirrelWaffle Debug Analysis"
date: 2025-03-31
categories:
  - Reverse_Engineering
tags:
  - Malware Analysis
  - SquirrelWaffle
---

## Introduction
SquirrelWaffle is a malware loader known for being distributed via malicious Office documents in spam campaigns. It serves as an initial foothold for attackers, enabling them to execute additional malicious payloads. 

When macros are enabled, the document executes a Visual Basic script that downloads further malware, often disguising its execution methods.

## Debugging Process
The full report outlines:
- How to acquire and analyze a SquirrelWaffle sample.
- Loading the sample into **IDA Pro** for function export analysis.
- Debugging with **x32dbg** to track decryption routines.
- Extracting configuration details and blocklisted IP addresses.

### **Read the Full Report**
📄 **[Download PDF Report](https://yourgithubusername.github.io/assets/SquirrelWaffle_Debug.pdf)**

## Resources & Further Reading
- [Malpedia - SquirrelWaffle](https://malpedia.caad.fkie.fraunhofer.de/details/win.squirrelwaffle)
- [Cisco Talos: SquirrelWaffle Analysis](https://blog.talosintelligence.com/squirrelwaffle-emerges/)
- [Trend Micro Research](https://www.trendmicro.com/en_us/research/21/k/Squirrelwaffle-Exploits-ProxyShell-and-ProxyLogon-to-Hijack-Email-Chains.html)
- [VirusTotal Sample](https://www.virustotal.com/gui/file/6095f96dd5eca96a3fb9338eec4ab574921c0febb36f6a6db60aae1aeb9ffcab)
- [Mandiant FLARE VM](https://github.com/mandiant/flare-vm)
