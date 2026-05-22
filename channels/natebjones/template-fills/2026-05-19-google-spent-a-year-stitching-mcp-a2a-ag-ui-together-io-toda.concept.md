---
video_id: zP6TnEiueEc
template_id: concept
template_version: 1
source_summary: ../summaries/2026-05-19-google-spent-a-year-stitching-mcp-a2a-ag-ui-together-io-toda.md
source_transcript: ../transcripts/2026-05-19-google-spent-a-year-stitching-mcp-a2a-ag-ui-together-io-toda.md
source_summary_hash: sha256:4c8b34904a207ea4aafd279d729296ea8abba04ddc0d9df8acaac260f7a76347
source_transcript_hash: sha256:e0b46ff1e9fa7ef7eee245a3f5485f6f10b9aa5bec2c5613c28e6ba96f8aac86
fill_id: 3f93cd5e-b246-46af-b43a-0a7db3b767af
published_at: '2026-05-22T01:01:31.413886'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

Six emerging protocols are reshaping AI agent development, but only three form the foundational substrate for tool access, coordination, and human control. The other three address narrower, contested use cases like structured UI and payments. Builders must look past model selection to understand how these protocol layers directly dictate customer experience and security.

## The argument

### Define the Core Substrate
- **Anchor Timestamps**: ['00:01:54']
- **Claim**: Three protocols form the foundation: MCP handles tool/data discovery, A2A handles agent-to-agent coordination, AGUI handles human-in-the-loop state sharing. These map to the core questions of what an agent can use, who it works with, and how humans stay in control.
- **Role**: definition

### MCP Enables Reach, Not Safety
- **Anchor Timestamps**: ['00:03:11']
- **Claim**: MCP standardizes tool access, solving the immediate pain of custom glue code. However, it enables arbitrary code execution and data access, creating a high-trust security boundary. Developers must implement scopes and audit trails because MCP itself does not decide if an agent should do the work.
- **Role**: evidence

### A2A Adds Coordination Cost
- **Anchor Timestamps**: ['00:06:26']
- **Claim**: A2A allows agents to delegate to specialized peers via 'agent cards,' but this adds latency, failure surfaces, and permission complexity. It is not required for every product; builders should only use it when delegated expertise or authority outside the primary agent is necessary.
- **Role**: counter

### AGUI Solves Supervision Debt
- **Anchor Timestamps**: ['00:08:57']
- **Claim**: AGUI provides the human control layer for long-running, non-deterministic agents. It enables streaming, shared state, and approval points, addressing the 'supervision debt' that arises when traditional call-and-response UIs fail to handle agent work-in-progress.
- **Role**: synthesis

### Contested Layers Are Domain-Specific
- **Anchor Timestamps**: ['00:10:39']
- **Claim**: Protocols like A2UI (structured interfaces), AP2 (commercial trust), and X42 (machine payments) are valuable but narrow. They address specific domains rather than the universal substrate, meaning builders must evaluate them based on specific workflow needs rather than assuming they are core standards.
- **Role**: evidence

## Evidence and caveats

The host notes that MCP has over 14,000 servers but warns of 'tool poisoning' attacks where malicious instructions hide in tool descriptions. A2A requires a critical mass of partners (Google launched with 50+ including Atlassian, Box, PayPal) to work across boundaries. AGUI is still early in adoption, with potential competitors from Langraph, Crew AI, and Amazon Bedrock. Payment protocols are highly fragmented, with Stripe, Mastercard, Visa, and PayPal all building competing layers, making customer trust and geographic bias key differentiators.

## Concepts surfaced

[[model-selection]] · [[security-boundaries]] · [[human-in-the-loop]] · [[agent-coordination]] · [[protocol-standards]] · [[customer-experience]]
