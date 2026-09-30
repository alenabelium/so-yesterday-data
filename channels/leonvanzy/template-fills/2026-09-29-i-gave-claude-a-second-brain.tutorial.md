---
video_id: CwL_XeedKw4
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-09-29-i-gave-claude-a-second-brain.md
source_transcript: ../transcripts/2026-09-29-i-gave-claude-a-second-brain.md
source_summary_hash: sha256:ce493e569a7c85c4e4fae569deedee516c647b57dfc01b3f61bfb5e4f2029930
source_transcript_hash: sha256:994968f8e89e6bcc08381b16bbf99cb73e95ea7db6a33d06ab36f259b10f0e57
fill_id: d9cc41cb-2728-4384-8e92-172854f871d4
published_at: '2026-09-30T06:10:54.900773'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Build a custom AI 'second brain' using Progress Agent Crack and RAG to let Claude search your personal videos and documents.

## Prerequisites

### Progress Account
- **Kind**: account
- **Note**: Create a free account at rag.progress.cloud to host your knowledge base.

### Claude Desktop or Web
- **Kind**: tool
- **Note**: Required to connect the MCP server and query your second brain.

### Code Work Agent
- **Kind**: tool
- **Note**: An agent capable of executing code scripts to automate data ingestion.

## Steps

### Create Knowledge Box
- **Timestamp**: [02:37](https://www.youtube.com/watch?v=CwL_XeedKw4&t=157)
- **Action**: Log in to Progress, create a new 'knowledge box' (your second brain), select region and embedding model.
- **Command Or Clicks**: Click 'create a new account', fill form, go to profile > knowledge boxes > create new.
- **Choice Branch**: Choose default 'General Languages' for embeddings or external partners like OpenAI.

### Generate API Key
- **Timestamp**: [05:28](https://www.youtube.com/watch?v=CwL_XeedKw4&t=328)
- **Action**: Navigate to Advanced > API Keys, create a key with 'manager' role for the agent.
- **Command Or Clicks**: Click three dots > developer/integrate > copy Nucleus DB API endpoint. Go to Advanced > API Keys > add > copy key.
- **Choice Branch**: Paste key into chat for setup, then delete it for security.

### Ingest Data via Agent
- **Timestamp**: [06:35](https://www.youtube.com/watch?v=CwL_XeedKw4&t=395)
- **Action**: Ask the agent to download videos (e.g., from archive.org) and upload them to the knowledge box.
- **Command Or Clicks**: Prompt agent: 'Upload remaining 14 videos... keep title, source links, skip duplicates.'
- **Choice Branch**: Manually upload files/folders via 'load data' or let the agent automate it.

### Connect MCP Server
- **Timestamp**: [08:28](https://www.youtube.com/watch?v=CwL_XeedKw4&t=508)
- **Action**: Copy the MCP server endpoint from Progress and add it as a connector in Claude.
- **Command Or Clicks**: Click three dots > developer/integrate > copy MCP server URL. In Claude: Connectors > Manage > Add > paste URL > OAuth 'register automatically'.
- **Choice Branch**: Allow access via the opened URL to complete authentication.

### Query Second Brain
- **Timestamp**: [09:37](https://www.youtube.com/watch?v=CwL_XeedKw4&t=577)
- **Action**: Ask Claude to search your second brain for specific information from the uploaded sources.
- **Command Or Clicks**: Prompt: 'Search my second brain, compare how magnetic fields move particles... cite both sources.'
- **Choice Branch**: Works in both Desktop and Web apps; syncs automatically.

## Gotchas

### Don't pass your API key directly to the agent if possible; let it set up the environment first, then add the key manually for security.
- **Severity**: serious
- **Timestamp**: [05:28](https://www.youtube.com/watch?v=CwL_XeedKw4&t=328)

### Markdown files don't scale well for second brains; use RAG/vector databases like Progress for fast querying.
- **Severity**: heads_up
- **Timestamp**: [01:18](https://www.youtube.com/watch?v=CwL_XeedKw4&t=78)

## Where to go next

Explore other MCP-compatible agents like Hermes or ChatGPT Work Mode to automate data ingestion further. Check the description for exact prompts and documentation links.

## Concepts surfaced

[[retrieval-augmented-generation]] · [[mcp-server-integration]] · [[ai-agent-automation]] · [[personal-knowledge-base]]
