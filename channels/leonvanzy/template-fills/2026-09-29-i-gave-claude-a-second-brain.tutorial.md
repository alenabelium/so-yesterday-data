---
video_id: CwL_XeedKw4
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-09-29-i-gave-claude-a-second-brain.md
source_transcript: ../transcripts/2026-09-29-i-gave-claude-a-second-brain.md
source_summary_hash: sha256:ce493e569a7c85c4e4fae569deedee516c647b57dfc01b3f61bfb5e4f2029930
source_transcript_hash: sha256:994968f8e89e6bcc08381b16bbf99cb73e95ea7db6a33d06ab36f259b10f0e57
fill_id: d075037f-a851-4704-ac95-839122a94e2b
published_at: '2026-09-30T09:10:58.495242'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Build a searchable 'second brain' for Claude using Progress Agent Crack and RAG to ingest videos and documents.

## Prerequisites

### Progress Account
- **Kind**: account
- **Note**: Create a new account at rag.progress.cloud to access the knowledge box database.

### Claude Desktop or Web
- **Kind**: tool
- **Note**: Required to connect the MCP server and query the second brain.

### Code Work Agent
- **Kind**: tool
- **Note**: Needed to execute scripts for uploading data to the knowledge base.

## Steps

### Create Knowledge Box
- **Timestamp**: [02:37](https://www.youtube.com/watch?v=CwL_XeedKw4&t=157)
- **Action**: Log in to Progress, navigate to profile > knowledge boxes, create a new box named 'YouTube second brain', select US region and default embedding settings.
- **Command Or Clicks**: Click 'create a new account' at rag.progress.cloud. Go to Profile > Knowledge Boxes > Create New.

### Configure API Access
- **Timestamp**: [05:28](https://www.youtube.com/watch?v=CwL_XeedKw4&t=328)
- **Action**: Generate an API key via Advanced > API Keys with 'manager' role. Copy the Nucleus DB API endpoint from Developer/Integration.
- **Command Or Clicks**: Advanced > API Keys > Add (Role: manager). Copy Nucleus DB API endpoint from Developer > Integration.

### Ingest Data via Agent
- **Timestamp**: [06:35](https://www.youtube.com/watch?v=CwL_XeedKw4&t=395)
- **Action**: Use Code Work to run a script that downloads videos (e.g., from archive.org) and uploads them to the knowledge box, preserving metadata.
- **Command Or Clicks**: Ask Code Work: 'Upload remaining 14 videos... keep title, source links, skip duplicates.'

### Connect MCP Server
- **Timestamp**: [08:28](https://www.youtube.com/watch?v=CwL_XeedKw4&t=508)
- **Action**: Copy the MCP server endpoint from Progress Developer/Integration. Add it in Claude Connectors > Manage Connectors > Add, selecting 'register automatically' for OAuth.
- **Command Or Clicks**: Connectors > Manage Connectors > Add > Paste MCP URL > Continue > Register Automatically > Allow.

### Query Second Brain
- **Timestamp**: [09:37](https://www.youtube.com/watch?v=CwL_XeedKw4&t=577)
- **Action**: Ask Claude to search the second brain for specific information, ensuring the connector is active to retrieve cited sources.
- **Command Or Clicks**: Chat: 'Search my second brain... cite both sources.'

## Gotchas

### Do not pass API keys directly into the agent chat if possible; let the agent set up the environment first, then add the key manually for security.
- **Severity**: serious
- **Timestamp**: [05:28](https://www.youtube.com/watch?v=CwL_XeedKw4&t=328)

### Ensure you select 'register automatically' in the OAuth client section when adding the MCP connector to avoid authentication errors.
- **Severity**: blocking
- **Timestamp**: [08:28](https://www.youtube.com/watch?v=CwL_XeedKw4&t=508)

## Where to go next

Explore other embedding models like OpenAI or Google Gemini for specialized language support. Check Progress documentation for advanced anonymization settings.

## Concepts surfaced

[[retrieval-augmented-generation]] · [[rag-database]] · [[mcp-server-integration]] · [[ai-agent-workflow]] · [[knowledge-base-setup]]
