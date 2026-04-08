# 🎨 Visual & Diagram Generation Prompts

> Prompts for creating architecture diagrams, workflow visuals, and stakeholder-ready diagrams using Excalidraw and MIRO.

[← Back to Main Library](../README.md)

---

### 7.1 Excalidraw Architecture Diagram Prompt

**When to use:** You need to explain a technical architecture to stakeholders using a visual diagram — for MCP, API flows, system integrations, or workflow pipelines.

```
Create an Excalidraw architecture diagram for: [describe what you want to visualize, e.g., "the MCP (Model Context Protocol) request/response pipeline"]

The diagram should show:
- [Zone/Layer 1]: [describe components, e.g., "Host/AI Client — User, LLM/Agent, MCP Client"]
- [Zone/Layer 2]: [describe, e.g., "Protocol Layer — JSON-RPC 2.0 over stdio or SSE"]
- [Zone/Layer 3]: [describe, e.g., "MCP Server — Request Router → Tools / Resources / Prompts handlers"]
- [Zone/Layer 4]: [describe, e.g., "External Systems — databases, APIs, file systems"]

Visual requirements:
- Use swim lanes or clearly labeled zones with different background colors
- Show data flow with directional arrows (solid for requests, dashed for responses/returns)
- Label each connection with the protocol or data format where relevant
- Group related components with a rounded rectangle container
- Use clean, minimal labels — no jargon beyond what's necessary for the audience

Audience: [e.g., non-technical practice lead and a technical consultant]

After the diagram, include a written walkthrough explaining each zone and how they connect.
```

**Tags:** `Excalidraw` `diagram` `architecture` `MCP` `visual` `stakeholder` `consulting`

---

### 7.2 Excalidraw Workflow Diagram — Stakeholder Explainer

**When to use:** You need a concise Excalidraw prompt (under 1000 characters) to generate a workflow diagram for stakeholder presentations.

```
Generate a detailed Excalidraw prompt (under 1,000 characters) to create a workflow diagram for: [describe workflow, e.g., employee onboarding, AP invoice processing, data pipeline].

The prompt should specify:
- Layout direction: horizontal, left to right
- Number of main phases/stages: [N]
- Key steps within each phase (2–4 bullet points each)
- Decision points (diamond shapes) with Yes/No conditions
- Color coding: [e.g., Green = start, Blue = process, Yellow = checkpoint, Red = issue/delay]
- Swim lanes if multiple teams/systems are involved: [list them]

Keep the Excalidraw prompt tight and actionable — every sentence should be a direct instruction to the diagram tool.
```

**Tags:** `Excalidraw` `workflow` `diagram` `stakeholder` `visual` `consulting`

---

*[← Back to Main Library](../README.md)*
