# 🏢 Project Work & Consulting Prompts

> Prompts for client-facing work, technical analysis, enterprise tools, and consulting deliverables.

[← Back to Main Library](../README.md)

---

### 1.1 SAP Technical Payload Analysis

**When to use:** You have an SAP API endpoint/payload and need to explain what it does in SAP — for proposals, workshops, or technical documentation with clients or architects.

```
Context — [Describe the project context briefly, e.g., "Working on a proposal with the SAP technical head for a client."]

I have encountered the following API payload:
  Endpoint: [paste endpoint]
  Method: [GET/PUT/POST]
  Payload: [paste JSON]

Role — Act as an SAP ECC / S/4HANA expert.

Action —
1. Based on this payload, what is being called in SAP? Break down every field and map it to SAP objects/tables/transactions.
2. How can we verify this in SAP? Provide transaction codes, table queries (SE16N/SE16), and workflow traces.
3. What are the edge cases and failure scenarios to document in the proposal?

Target audience — [e.g., SAP technical head, Sr. BSA]
```

**Tags:** `SAP` `ECC` `S4HANA` `API` `consulting` `proposal` `project-work`

---

### 1.2 Technical Workshop Meeting Summary

**When to use:** You have a transcript or notes from a technical workshop session and need a structured meeting summary Word document that matches a prior session's format.

```
I have a meeting transcript from a technical workshop session. Please generate a detailed meeting summary document from it.

Requirements:
- Apply humanized, natural writing style (avoid AI-sounding language)
- Match the formatting and structure of the attached reference document [attach prior session summary]
- Transcript file: [attach .docx transcript]

The summary must cover:
- Attendees table (Name, Role, Company)
- Key topics discussed (with sub-sections per topic)
- Architecture decisions and trade-offs
- Open questions and action items (with owners)
- Any interface flows, data flows, or comparison tables discussed

Project context: [e.g., Medline AP Invoice 2-Way Match platform migration assessment, Session 4]
```

**Tags:** `meeting-summary` `consulting` `project-work` `Word-doc` `humanizer` `SAP` `Appian`

---

### 1.3 Power BI MCP Server Security Framework

**When to use:** You need a comprehensive, implementation-ready security guide for a Power BI MCP server deployment in an enterprise Microsoft environment.

```
Give me a detailed, implementation-focused security guide for a Power BI MCP (Model Context Protocol) server used for [describe report/use case].

Cover these layers in order:
1. Authentication & Identity — Microsoft Entra ID, OAuth 2.0, Service Principals
2. Authorization — RBAC, least-privilege principles
3. Data-level security — RLS (Row-Level Security) with DAX syntax, OLS (Object-Level Security)
4. Network isolation — VNets, Private Link, NSG rules
5. LLM data handling risks specific to MCP integrations
6. Audit logging — Microsoft Fabric, Azure Monitor
7. Operational safeguards — version control, tool poisoning prevention
8. Compliance & governance — Microsoft Purview, regulatory requirements

For each layer, include:
- Specific configuration steps
- Relevant Microsoft tools and portal paths
- Code snippets or DAX where applicable
- A priority/risk rating

Target audience: Enterprise security architect, Power Platform admin
```

**Tags:** `Power-BI` `MCP` `security` `Microsoft` `enterprise` `Entra-ID` `consulting`

---

### 1.4 Copilot Agent Red-Teaming / Adversarial Prompt Testing

**When to use:** You have built a Microsoft Copilot agent and need to test its robustness against adversarial inputs, prompt injections, and jailbreak attempts.

```
I have built a Microsoft Copilot agent. I need a comprehensive adversarial prompt testing guide to evaluate its security and robustness.

Cover the following attack categories with specific test prompts for each:
1. Direct prompt injection
2. Indirect prompt injection
3. Jailbreaking — roleplay/persona hijacking, hypothetical framing
4. Goal hijacking
5. Data exfiltration probes
6. Context window manipulation
7. Encoding & obfuscation attacks — include Morse code, Base64, ROT13 variants
8. Logic & reasoning manipulation
9. Tool/function call abuse
10. Social engineering patterns

For each category, provide:
- 2–3 example adversarial prompts to test
- What the agent should do (safe behavior)
- What a failure looks like (unsafe behavior)
- Recommended mitigation

Also provide an iterative red-teaming methodology: baseline → isolate → log → escalate.
```

**Tags:** `Copilot` `red-teaming` `security` `adversarial` `Microsoft` `AI-agent` `project-work`

---

### 1.5 JIRA Excel Dashboard with Power Query

**When to use:** You have a JIRA data dump and need to design an auto-refreshing Excel dashboard with pivot tables and charts — without a direct JIRA-Excel connection.

```
I have a JIRA data dump in Excel/CSV format. I need to design an automated Excel dashboard that:
- Uses Power Query as the data bridge (no direct JIRA connection available)
- Auto-refreshes when I replace the JIRA dump file (same filename, same path)
- Includes dynamic pivot tables for: priority status month-wise, overall status, and [add your metrics]
- Has charts that automatically reflect updated data

Constraints: Microsoft Excel only, no external plugins, no direct JIRA API access.

Please provide:
1. Power Query setup steps (connection type, file path configuration, transform steps)
2. How to add a Month-Year calculated column for time-series pivots
3. Pivot table configuration for each chart type
4. Slicer setup for interactive filtering
5. VBA macro (optional) for one-click refresh
6. Troubleshooting guide for common refresh failures

Format as a step-by-step implementation guide I can hand off to a team member.
```

**Tags:** `Excel` `Power-Query` `JIRA` `dashboard` `automation` `reporting` `project-work`

---

*[← Back to Main Library](../README.md)*
