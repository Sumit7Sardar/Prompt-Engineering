# ⚙️ Automation & Workflows (n8n) Prompts

> Prompts for designing, debugging, and sanitizing n8n workflows with AI agent integrations.

[← Back to Main Library](../README.md)

---

### 5.1 n8n AI Agent Workflow Design (Beginner-Friendly)

**When to use:** You need step-by-step instructions to build a complete n8n backend workflow with an AI Agent node (Gemini or Claude) for a course project or POC — written for someone with no coding experience.

```
Act as an n8n workflow specialist.

I need to build a backend workflow in n8n for: [describe application, e.g., a Resume Analyzer that takes a job description and resume PDF, scores them, and returns a hiring recommendation].

My experience level: [e.g., no coding experience / beginner]
AI model to use: [e.g., Google Gemini Chat Model / Claude API via HTTP Request node]
Frontend: [e.g., Lovable.dev app that sends a webhook POST request]

Design a complete n8n workflow with:
- Exact node names as they appear in n8n v1.0+ (e.g., "Edit Fields" not "Set", "Code" not "Function")
- All node configurations with parameter values
- JavaScript code for all Code nodes
- The AI Agent system prompt with structured JSON output instructions
- A Respond to Webhook node with the correct response format

Output format: Number each node sequentially. For each node provide:
1. Node name (exact)
2. Node type
3. All parameter configurations
4. Any code or expressions (complete, copy-paste ready)
5. Connection to next node

Include a cURL test command and a sample expected JSON output at the end.
```

**Tags:** `n8n` `automation` `AI-agent` `Gemini` `workflow` `beginner` `webhook`

---

### 5.2 n8n Workflow Sanitizer for GitHub

**When to use:** You have an n8n workflow JSON you want to publish to GitHub, and need all credentials, personal identifiers, and instance-specific data replaced with safe placeholders.

```
I have an n8n workflow JSON that I want to publish to a public GitHub repository. Sanitize it by identifying and replacing all confidential information with clearly labeled placeholders.

Replace the following categories:
- n8n instance URL/hostname → YOUR_N8N_INSTANCE.app.n8n.cloud
- All credential IDs and credential names → YOUR_[SERVICE]_CREDENTIAL_ID / YOUR_[SERVICE]_CREDENTIAL_NAME
- Personal email addresses → placeholder@example.com
- Webhook UUIDs → YOUR_WEBHOOK_ID
- Real IP addresses and CF Ray IDs → 0.0.0.0 / REDACTED
- Instance ID and workflow ID (meta fields) → YOUR_N8N_INSTANCE_ID / YOUR_WORKFLOW_ID
- Version ID → YOUR_VERSION_ID
- Any uploaded file names or binary data paths containing personal info → Sample_File.pdf / REDACTED_BINARY_ID

Rules:
- Preserve 100% of workflow logic, node structure, and connections
- Do not alter any JavaScript code, expressions, or system prompts
- Output the sanitized JSON only (no commentary)
- After the JSON, provide a summary table: Original Value | Replaced With | Category

Workflow JSON: [paste JSON]
```

**Tags:** `n8n` `GitHub` `security` `sanitize` `workflow` `open-source`

---

### 5.3 n8n Workflow Debugging — Identify & Fix Issues

**When to use:** Your n8n workflow has errors or unexpected behavior and you need a structured analysis and corrected code.

```
I have an n8n workflow with issues. Please identify all problems and provide a fully corrected version.

My workflow: [paste node configurations and code]
Error or unexpected behavior: [describe what's going wrong, e.g., "AI Agent returns markdown instead of JSON", "data from upstream node not accessible"]
n8n version: [v1.x]
AI model node in use: [Google Gemini / Claude / OpenAI]

Analyze and fix:
1. Incorrect node names for this n8n version (e.g., "Set" → "Edit Fields", "Function" → "Code")
2. Broken data references (correct n8n expression syntax: $('NodeName').item.json.fieldName)
3. AI Agent response parsing issues — strip markdown fences, validate required fields
4. Missing error handling
5. Any logical flow issues (wrong connections, missing merge nodes, incorrect IF conditions)

For each issue found:
- Location (node name and parameter)
- Root cause
- Corrected code or configuration (complete, copy-paste ready)

Deliver the full corrected workflow node by node.
```

**Tags:** `n8n` `debugging` `workflow` `automation` `AI-agent` `troubleshooting`

---

*[← Back to Main Library](../README.md)*
