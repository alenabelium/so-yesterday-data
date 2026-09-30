---
video_id: CwL_XeedKw4
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-09-29-i-gave-claude-a-second-brain.md
source_transcript: ../transcripts/2026-09-29-i-gave-claude-a-second-brain.md
source_summary_hash: sha256:ce493e569a7c85c4e4fae569deedee516c647b57dfc01b3f61bfb5e4f2029930
source_transcript_hash: sha256:994968f8e89e6bcc08381b16bbf99cb73e95ea7db6a33d06ab36f259b10f0e57
fill_id: c0e5f888-a240-43bb-8e31-9c367983b115
published_at: '2026-09-30T07:10:52.848091'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Build a searchable 'second brain' for Claude using Progress Agent Crack and RAG to ingest videos and documents.

## Prerequisites

### Claude Desktop or ChatGPT
- **Kind**: tool
- **Note**: Desktop app or web interface with connector support.

### Progress Account
- **Kind**: account
- **Note**: Create at rag.progress.cloud to host the knowledge base.

### Code Work / Agent
- **Kind**: tool
- **Note**: Agent capable of executing scripts to upload data.

## Steps

### Create Knowledge Box
- **Timestamp**: [02:37](https://www.youtube.com/watch?v=CwL_XeedKw4&t=157)
- **Action**: Log in to Progress, create a new knowledge box named 'YouTube second brain', select region and embedding model.
- **Command Or Clicks**: Click 'create a new account' at rag.progress.cloud. Go to profile > knowledge boxes > create new.
- **Choice Branch**: Choose default General Languages or external partners like OpenAI for embeddings.

### Generate API Key
- **Timestamp**: [05:28](https://www.youtube.com/watch?v=CwL_XeedKw4&t=328)
- **Action**: Navigate to Advanced > API Keys, create a key with 'manager' role, and copy it.
- **Command Or Clicks**: Click three dots > developer/integrate > copy Nucleus DB API endpoint. Go to Advanced > API Keys > add > manager role.
- **Choice Branch**: Set expiration date if desired.

### Configure Data Loader
- **Timestamp**: [04:03](https://www.youtube.com/watch?v=CwL_XeedKw4&t=243)
- **Action**: Ask your agent to set up a reusable loader using the API endpoint and key.
- **Command Or Clicks**: Forward request to Code Work: 'Set up a reusable loader for my Progress knowledge block...'
- **Choice Branch**: Grant folder access to allow the agent to write scripts.

### Ingest Data
- **Timestamp**: [06:35](https://www.youtube.com/watch?v=CwL_XeedKw4&t=395)
- **Action**: Have the agent download videos (e.g., NASA Science Cast) and upload them to the knowledge base.
- **Command Or Clicks**: Ask agent: 'Find 15 NASA Science Cast videos... Upload only the MP4 file with the dark lightning...'
- **Choice Branch**: Manually click 'load data' for documents/links or let the agent handle it.

### Connect MCP Server
- **Timestamp**: [08:28](https://www.youtube.com/watch?v=CwL_XeedKw4&t=508)
- **Action**: Copy the MCP server endpoint from Progress and add it as a connector in Claude.
- **Command Or Clicks**: Click three dots > developer/integrate > copy MCP server URL. In Claude: Connectors > manage connectors > add > paste URL.
- **Choice Branch**: Select 'register automatically' for OAuth client.

### Authorize and Query
- **Timestamp**: [09:37](https://www.youtube.com/watch?v=CwL_XeedKw4&t=577)
- **Action**: Allow access in the browser, then query the second brain using specific instructions.
- **Command Or Clicks**: Click 'connect' > 'continue connecting' > 'allow'. Ask: 'Search my second brain... cite both sources.'
- **Choice Branch**: Works on both Desktop and Web apps.

## Gotchas

### Markdown files don't scale well; use RAG via Progress for fast querying.
- **Severity**: serious
- **Timestamp**: [01:18](https://www.youtube.com/watch?v=CwL_XeedKw4&t=78)

### Avoid pasting API keys directly into chat if possible; let the agent set it up or delete after recording.
- **Severity**: serious
- **Timestamp**: [05:28](https://www.youtube.com/watch?v=CwL_XeedKw4&t=328)

## Where to go next

Explore other MCP server integrations for different data sources. Check Progress documentation for advanced embedding models.

## Concepts surfaced

[[retrieval-augmented-generation]] · [[mcp-server-integration]] · [[ai-agent-workflows]] · [[knowledge-base-setup]]
