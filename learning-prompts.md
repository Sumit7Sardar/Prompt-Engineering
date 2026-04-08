# 📚 Learning & Exploration Prompts

> Prompts for understanding new concepts, building POCs, and technical troubleshooting.

[← Back to Main Library](../README.md)

---

### 3.1 Concept Explained at Three Levels

**When to use:** You want to deeply understand a new concept (technical, business, or domain-specific) and need explanations calibrated for different audiences.

```
Explain [concept/topic] at three levels:

1. Simple analogy — explain it as if to someone with no background, using an everyday analogy
2. Student level — explain it as to a university student studying [relevant field], with foundational terminology
3. Professional level — explain it as to an industry practitioner, using precise frameworks, tools, and real-world application context

After all three explanations, tell me:
- Which explanation is most useful for someone learning this professionally, and why
- What the 3 most important frameworks or references someone should know in this domain
```

**Tags:** `learning` `concepts` `business-analysis` `explainer` `onboarding`

---

### 3.2 MCP POC Idea Generator

**When to use:** You need to generate practical, cost-free Model Context Protocol (MCP) proof-of-concept ideas to propose to your practice lead or technical team.

```
Act as an MCP (Model Context Protocol) expert specialist.

I have recently completed Anthropic's MCP course and need to propose POC ideas to my practice lead. Generate 5 strong POC ideas that:
- Demonstrate clear MCP concepts: Resources, Tools, Prompts, multi-server orchestration
- Have tangible business value for a [describe industry/domain, e.g., IT consulting firm]
- Are buildable with free-tier tools only (no paid API credits required for the POC)
- Range from low to medium complexity

For each idea, provide:
| # | POC Name | Core MCP Concepts Used | Business Value | Free-Tier Stack | Complexity |

After the table, provide a detailed implementation breakdown for the top 2 ideas including:
- Architecture diagram description
- Step-by-step build sequence
- Key files and components
- How to demo it to non-technical stakeholders
```

**Tags:** `MCP` `learning` `POC` `Anthropic` `AI-tools` `consulting` `free-tier`

---

### 3.3 Windows Technical Troubleshooting Guide

**When to use:** You're facing a recurring Windows system error and need a structured, step-by-step troubleshooting guide from basic to advanced fixes.

```
I am facing the following Windows issue: [describe error clearly, e.g., "explorer.exe application error — memory read failure at address 0x000..."]

System info: Windows [version], [RAM], [recent changes if any]

Please provide a structured troubleshooting guide that:
1. Diagnoses the root cause category (driver issue / corrupted system file / shell extension / RAM fault / registry issue)
2. Provides steps from least to most invasive:
   - Step 1: Built-in Windows tools (SFC, DISM)
   - Step 2: Third-party diagnostic tools (NirSoft ShellExView, etc.)
   - Step 3: Driver/update rollback
   - Step 4: Hardware diagnostics
   - Step 5: Registry fixes
3. Includes exact commands to run in elevated Command Prompt or PowerShell
4. Provides a reference table for edge cases: error triggered by specific Windows Update / right-click crash / login-time error / SFC cannot self-repair
5. Tells me what to do if each step fails

Goal: Permanent fix, not a workaround.
```

**Tags:** `Windows` `troubleshooting` `technical` `learning` `sysadmin`

---

*[← Back to Main Library](../README.md)*
