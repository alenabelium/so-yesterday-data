---
video_id: CwL_XeedKw4
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-09-29-i-gave-claude-a-second-brain.md
source_transcript: ../transcripts/2026-09-29-i-gave-claude-a-second-brain.md
source_summary_hash: sha256:ce493e569a7c85c4e4fae569deedee516c647b57dfc01b3f61bfb5e4f2029930
source_transcript_hash: sha256:994968f8e89e6bcc08381b16bbf99cb73e95ea7db6a33d06ab36f259b10f0e57
fill_id: e4cf9a10-18a9-42ba-87d2-4cf4ef947de8
published_at: '2026-09-30T08:10:50.454571'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Build a personal AI second brain using Progress Agent and RAG to let Claude search your custom video library.

## Prerequisites

### Progress Account
- **Kind**: account
- **Note**: Create one at rag.progress.cloud to host the knowledge box.

### Claude Desktop or Web
- **Kind**: tool
- **Note**: Required to connect the MCP server and query the database.

### Code Interpreter Access
- **Kind**: tool
- **Note**: Use Claude Code Work or ChatGPT work mode to run upload scripts.

## Steps

### Create Knowledge Box
- **Timestamp**: [02:37](https://www.youtube.com/watch?v=CwL_XeedKw4&t=157)
- **Action**: Log in to Progress, create a new knowledge box named 'YouTube second brain', select US region and default embeddings.
- **Command Or Clicks**: Click 'create a new account' at rag.progress.cloud, then 'knowledge boxes' > 'new'.
- **Choice Branch**: Choose General Languages for embeddings unless specific language support is needed.

### Generate API Key
- **Timestamp**: [05:28](https://www.youtube.com/watch?v=CwL_XeedKw4&t=328)
- **Action**: Navigate to Advanced > API Keys, create a key with 'manager' role, and copy it for the agent.
- **Command Or Clicks**: Click 'Advanced', 'API Keys', add role 'manager', click 'add', then copy the generated key.
- **Choice Branch**: You can paste the key into the chat for setup or let the agent handle it securely later.

### Deploy Upload Script
- **Timestamp**: [06:35](https://www.youtube.com/watch?v=CwL_XeedKw4&t=395)
- **Action**: Ask Claude Code Work to find NASA videos on archive.org and upload them using the API endpoint.
- **Command Or Clicks**: Prompt: 'Upload 15 NASA Science Cast videos... keep title, source links, skip duplicates.'
- **Choice Branch**: You can also manually upload files via the 'load data' button if not using an agent.

### Connect MCP Server
- **Timestamp**: [08:28](https://www.youtube.com/watch?v=CwL_XeedKw4&t=508)
- **Action**: Copy the MCP server endpoint from Progress developer/integrate and add it as a connector in Claude.
- **Command Or Clicks**: In Claude: Connectors > Manage > Add > Paste URL > OAuth 'register automatically' > Allow.
- **Choice Branch**: Works on both Desktop and Web apps; syncs automatically between them.

## Gotchas

### Markdown files don't scale well for agents; use RAG/vector databases like Progress for speed.
- **Severity**: serious
- **Timestamp**: [01:18](https://www.youtube.com/watch?v=CwL_XeedKw4&t=78)

### Ensure your agent has code execution capabilities (like Code Work) to run the upload scripts.
- **Severity**: blocking
- **Timestamp**: [04:03](https://www.youtube.com/watch?v=CwL_XeedKw4&t=243)

## Where to go next

Explore other MCP connectors for Claude or try uploading document libraries instead of video sources.

## Concepts surfaced

[[retrieval-augmented-generation]] · [[mcp-server-setup]] · [[ai-agent-workflows]] · [[personal-knowledge-base]]
