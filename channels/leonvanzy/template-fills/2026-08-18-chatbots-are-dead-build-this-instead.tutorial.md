---
video_id: epGDGyTZs5Y
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-08-18-chatbots-are-dead-build-this-instead.md
source_transcript: ../transcripts/2026-08-18-chatbots-are-dead-build-this-instead.md
source_summary_hash: sha256:7800324b311da65b60fe83271c4bcc441bbf56cbb4fb9c5524acad00fc5c634f
source_transcript_hash: sha256:99e333ba75d540ef2863b9585fea133801b0671b4585c4a8dba1183f75a5f8c9
fill_id: 417e925b-43ca-4ba3-92d7-85489ab6143d
published_at: '2026-09-29T11:22:50.706583'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Build an autonomous NDA agent that creates, sends, and tracks agreements using Claude Code and DocuSign's MCP server.

## Prerequisites

### DocuSign Developer Account
- **Kind**: account
- **Note**: Free account required to generate integration keys and secrets for authentication.

### Claude Code
- **Kind**: tool
- **Note**: CLI coding agent used to scaffold the app and manage MCP server connections.

### VS Code
- **Kind**: os
- **Note**: Recommended environment to view generated files while using Claude Code.

## Steps

### Install Playwright MCP and Start App Skill
- **Timestamp**: [06:43](https://www.youtube.com/watch?v=epGDGyTZs5Y&t=403)
- **Action**: Install the Playwright MCP server for browser control and the 'start an app' skill to define tech stack guardrails.
- **Command Or Clicks**: npx skills add Leon Fran Sales / skills
- **Choice Branch**: Skip if using Claude Desktop which has integrated browser access.

### Scaffold App Shell with Clarifying Questions
- **Timestamp**: [08:34](https://www.youtube.com/watch?v=epGDGyTZs5Y&t=514)
- **Action**: Prompt the agent to build a three-screen shell (login, chat, table) using Postgres in Docker and ask clarifying questions.
- **Command Or Clicks**: Pass prompt: 'Build an app called Agreement Agent...'
- **Choice Branch**: Answer questions like 'Postgres in Docker' for data storage.

### Create DocuSign Integration Key
- **Timestamp**: [13:42](https://www.youtube.com/watch?v=epGDGyTZs5Y&t=822)
- **Action**: Generate a private custom integration key and secret in the DocuSign developer portal.
- **Command Or Clicks**: Profile > My apps and keys > Add app and integration key
- **Choice Branch**: Set redirect URI to /api/docusign/callback on localhost:3000.

### Connect App to DocuSign via MCP
- **Timestamp**: [12:42](https://www.youtube.com/watch?v=epGDGyTZs5Y&t=762)
- **Action**: Prompt the agent to add DocuSign auth using the integration key, secret, and redirect URI.
- **Command Or Clicks**: Paste prompt file 'add DocuSign auth' into Claude Code
- **Choice Branch**: Allow access in the browser popup when prompted.

### Create NDA Template in DocuSign
- **Timestamp**: [18:25](https://www.youtube.com/watch?v=epGDGyTZs5Y&t=1105)
- **Action**: Upload a PDF and define recipients (counterparty, internal approver) with signature fields.
- **Command Or Clicks**: Agreements > Templates > Create envelope template
- **Choice Branch**: Set signing order to ensure counterparty signs before internal approval.

### Integrate Agent Brain with Claude SDK
- **Timestamp**: [16:05](https://www.youtube.com/watch?v=epGDGyTZs5Y&t=965)
- **Action**: Prompt the agent to use the Claude Agent SDK and Opus 5 model to connect to the DocuSign remote MCP.
- **Command Or Clicks**: Paste prompt file 'add the agent.md' into Claude Code
- **Choice Branch**: Clear context window before pasting the agent integration prompt.

### Test Agent Workflow via Chat Interface
- **Timestamp**: [21:26](https://www.youtube.com/watch?v=epGDGyTZs5Y&t=1286)
- **Action**: Use voice or text to instruct the agent to send an NDA, confirming details before execution.
- **Command Or Clicks**: Prompt: 'Please, can you send an NDA to Jane? ...'
- **Choice Branch**: Verify the agent asks for approval before sending.

## Gotchas

### Do not specify a tech stack manually; let the 'start an app' skill define guardrails to avoid future issues.
- **Severity**: serious
- **Timestamp**: [07:30](https://www.youtube.com/watch?v=epGDGyTZs5Y&t=450)

### The agent only has permissions of the signed-in user; ensure you are logged in with appropriate access.
- **Severity**: blocking
- **Timestamp**: [15:03](https://www.youtube.com/watch?v=epGDGyTZs5Y&t=903)

### DocuSign MCP server is in beta at the time of recording; stability may vary.
- **Severity**: heads_up
- **Timestamp**: [05:43](https://www.youtube.com/watch?v=epGDGyTZs5Y&t=343)

## Where to go next

Source code and prompts are available on GitHub. Explore DocuSign's pre-created workflow templates for complex multi-step agreements beyond simple NDAs.

## Concepts surfaced

[[autonomous-ai-agents]] · [[docusign-mcp-server]] · [[claude-code-tutorial]] · [[enterprise-workflow-automation]]
