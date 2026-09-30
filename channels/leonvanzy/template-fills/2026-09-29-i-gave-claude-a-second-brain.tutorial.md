---
video_id: CwL_XeedKw4
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-09-29-i-gave-claude-a-second-brain.md
source_transcript: ../transcripts/2026-09-29-i-gave-claude-a-second-brain.md
source_summary_hash: sha256:ce493e569a7c85c4e4fae569deedee516c647b57dfc01b3f61bfb5e4f2029930
source_transcript_hash: sha256:994968f8e89e6bcc08381b16bbf99cb73e95ea7db6a33d06ab36f259b10f0e57
fill_id: 87f13200-fad4-44c2-a709-54b7f81a5f1f
published_at: '2026-09-30T09:22:17.545588'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Build a personal AI second brain using Progress Agent and Claude to search custom data sources via RAG.

## Prerequisites

### Progress Account
- **Kind**: account
- **Note**: Sign up at rag.progress.cloud to create a knowledge box for your second brain.

### Claude Desktop or Web
- **Kind**: tool
- **Note**: Required to act as the agent interface and connect via MCP server.

### Code Interpreter Access
- **Kind**: tool
- **Note**: Use Claude Code Work or ChatGPT work mode to execute data ingestion scripts.

## Steps

### Create Knowledge Box
- **Timestamp**: [02:37](https://www.youtube.com/watch?v=CwL_XeedKw4&t=157)
- **Action**: Log in to Progress and create a new knowledge box named 'YouTube second brain' with default embedding settings.
- **Command Or Clicks**: Click 'create a new account', fill form, go to profile > knowledge boxes > create new.
- **Choice Branch**: Choose region (US) and embedding model (default or external).

### Generate API Key
- **Timestamp**: [05:28](https://www.youtube.com/watch?v=CwL_XeedKw4&t=328)
- **Action**: Navigate to Advanced > API Keys, create a key with 'manager' role for the knowledge box.
- **Command Or Clicks**: Go to 'Advanced', 'API Keys', select role 'manager', click 'add', copy key.
- **Choice Branch**: Set expiration date if desired.

### Ingest Data via Agent
- **Timestamp**: [06:35](https://www.youtube.com/watch?v=CwL_XeedKw4&t=395)
- **Action**: Ask the agent to download videos from archive.org and upload them to the knowledge box using the API.
- **Command Or Clicks**: Prompt agent: 'Upload remaining 14 videos... skip duplicates'. Use Nucleus DB API endpoint.
- **Choice Branch**: Manually upload files via 'load data' or let agent script it.

### Connect MCP Server
- **Timestamp**: [08:28](https://www.youtube.com/watch?v=CwL_XeedKw4&t=508)
- **Action**: Copy the MCP server endpoint from Progress and add it as a connector in Claude.
- **Command Or Clicks**: Go to 'developer/integrate', copy URL. In Claude: connectors > manage > add > paste URL > allow.
- **Choice Branch**: Use OAuth 'register automatically' for authentication.

### Query Second Brain
- **Timestamp**: [09:37](https://www.youtube.com/watch?v=CwL_XeedKw4&t=577)
- **Action**: Ask Claude to search the second brain for specific information and cite sources.
- **Command Or Clicks**: Prompt: 'Search my second brain... cite both sources.' Ensure connector is active.
- **Choice Branch**: Works on both desktop app and claude.ai web interface.

## Gotchas

### Avoid passing API keys directly to the agent if possible; let it set up scripts first, then add key later for security.
- **Severity**: serious
- **Timestamp**: [05:28](https://www.youtube.com/watch?v=CwL_XeedKw4&t=328)

### Markdown files do not scale well for second brains; use RAG/vector databases like Progress for speed and efficiency.
- **Severity**: heads_up
- **Timestamp**: [01:18](https://www.youtube.com/watch?v=CwL_XeedKw4&t=78)

## Where to go next

Explore other MCP-compatible tools to expand your agent's capabilities. Check the description for exact prompts and documentation links.

## Concepts surfaced

[[retrieval-augmented-generation]] · [[mcp-server-integration]] · [[ai-agent-workflows]] · [[knowledge-base-setup]]
