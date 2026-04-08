# 🧩 Product Management & Ideation Prompts

> Prompts for hackathon strategy, tech stack selection, AI feature ideation, and process visualization.

[← Back to Main Library](../README.md)

---

### 4.1 Hackathon Problem Statement Evaluator

**When to use:** You have multiple hackathon problem statements and need a structured, multi-criteria analysis to select the best one — especially when presenting to senior PM/tech juries.

```
I have [N] problem statements for a hackathon and need to select the best one to build.

Problem statements: [attach or paste each one with its dataset description]

Jury profile: [e.g., Senior PMs at Microsoft and Google]
My team's strengths: [e.g., vibe coding, n8n, AI agent workflows]
Time constraint: [e.g., 4–5 hours build time]

Evaluate each problem statement across these 7 criteria and score them 1–5:
1. Data richness — how much can the dataset demonstrate live?
2. Agentic reasoning visibility — can the AI's decision-making be shown clearly?
3. Demo-ability — how impressive is the live demo in 5 minutes?
4. Jury relatability — will this jury have personally experienced this problem?
5. Build feasibility — can my team build an MVP in the given time?
6. Domain risk — are there liability/sensitivity issues (e.g., healthcare, finance)?
7. Storytelling narrative — how compelling is the before/after story?

Output:
- Scoring table for all [N] problems
- Recommended choice with rationale
- Key product metrics to pitch to the jury for the winning choice
- Top 3 demo moments to script
```

**Tags:** `PM` `hackathon` `product` `evaluation` `decision-making` `ideation`

---

### 4.2 Vibe-Coding Tech Stack Recommendation

**When to use:** You have a product idea and want a no-code/low-code "vibe coding" tech stack recommendation for rapid prototyping — especially for hackathons or course projects.

```
I want to build [describe product/feature, e.g., an agentic AI interview scheduling tool].

Constraints:
- I prefer vibe-coding tools over traditional engineering stacks
- Build time: [e.g., 4–5 hours / 1 weekend]
- Team size: [e.g., 3 people, mixed technical backgrounds]
- Must be deployable for a live demo

Recommend a complete vibe-coding tech stack including:
1. Frontend UI generation tool (e.g., Lovable.dev, v0.dev)
2. Backend/workflow automation (e.g., n8n, Make)
3. AI/LLM integration (e.g., Claude API, Gemini, OpenAI) — specify which node/method to use
4. Hosting/deployment (e.g., Vercel, n8n Cloud)
5. Any supporting tools (e.g., Cursor, Windsurf for custom logic)

For each tool:
- Why it fits this specific use case
- How it connects to the other tools
- What to build in it vs. what to hand off to the next tool

Also provide: a 5-step build sequence with time estimates.

Reference: I have prior experience with n8n + Gemini for a Resume Analyzer project — align patterns where possible.
```

**Tags:** `PM` `vibe-coding` `hackathon` `n8n` `Lovable` `tech-stack` `rapid-prototyping`

---

### 4.3 AI-Powered Product Feature Ideation

**When to use:** You want to brainstorm AI-powered improvements for an existing product (e.g., Microsoft Teams, Copilot) with concrete, implementable concepts — not vague ideas.

```
Act as a senior product manager and AI product strategist.

Product: [e.g., Microsoft Teams / Microsoft Copilot]
Focus area: [e.g., meeting productivity / notification overload / agent reliability]

Generate 5–7 AI-powered feature improvements for this product. For each feature:
1. Feature name
2. Problem it solves (with a specific user pain point)
3. How AI makes it possible (specific model behavior or capability)
4. 3 concrete mechanisms (e.g., "auto-batches notifications by priority score," "summarizes thread context before alerting")
5. Success metric — how would you measure if it worked?
6. Potential edge case or risk

Prioritize features that:
- Are technically feasible today
- Would noticeably change user behavior
- Could be built as an agent or MCP integration

Format as a structured table, then expand on the top 2 ideas in detail.
```

**Tags:** `PM` `ideation` `AI-product` `Microsoft` `Copilot` `Teams` `features`

---

### 4.4 MIRO AI Process Flow Prompt Generator

**When to use:** You have a use case from a client or stakeholder and need a detailed prompt to feed into MIRO AI to generate a professional process flow diagram for a POC or management presentation.

```
I need to create a detailed process flow diagram for a POC presentation to management.

Use case overview: [e.g., Contract/License Management Predictive Analytics system that predicts software renewal needs]

Data sources: [e.g., SAP, SharePoint, Manual Excel files]
Key stakeholders/users: [e.g., Field Service Managers, Engineers]
Core AI components: [e.g., Predictive ML model, Generative AI for recommendations]
Integration systems: [e.g., API front-end, ERP]

Generate a detailed MIRO AI prompt that instructs it to create a process flow with:
1. Swim lanes for: [Data Sources / AI Engine / Users / Output]
2. Decision points with conditions
3. Automated vs. manual step indicators
4. Data flow direction arrows
5. Color coding: [e.g., Blue = data, Green = AI/ML, Orange = user actions]
6. Technical annotations for API touchpoints and data governance checkpoints
7. Feedback loops for model improvement

The flow should read left-to-right from data collection → processing → AI → output → user action.
Keep the MIRO prompt under 800 words for best results.
```

**Tags:** `PM` `MIRO` `process-flow` `POC` `stakeholder` `diagram` `consulting`

---

*[← Back to Main Library](../README.md)*
