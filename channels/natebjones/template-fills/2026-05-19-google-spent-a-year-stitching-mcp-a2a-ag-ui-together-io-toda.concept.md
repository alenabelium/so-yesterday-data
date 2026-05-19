---
video_id: zP6TnEiueEc
template_id: concept
template_version: 1
source_summary: ../summaries/2026-05-19-google-spent-a-year-stitching-mcp-a2a-ag-ui-together-io-toda.md
source_transcript: ../transcripts/2026-05-19-google-spent-a-year-stitching-mcp-a2a-ag-ui-together-io-toda.md
source_summary_hash: sha256:4c8b34904a207ea4aafd279d729296ea8abba04ddc0d9df8acaac260f7a76347
source_transcript_hash: sha256:e0b46ff1e9fa7ef7eee245a3f5485f6f10b9aa5bec2c5613c28e6ba96f8aac86
fill_id: 0be20956-6b89-425f-b54e-6cee137d735f
published_at: '2026-05-19T16:04:21.507847'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

Six emerging protocols form the substrate for agentic systems, but only three—MCP, A2A, and AGUI—constitute the core standard stack for tool access, coordination, and human control. The remaining protocols (A2UI, AP2, X42) address narrower, contested domains like structured UI and payments. Developers must prioritize understanding these operating surfaces over model selection to shape customer experience and security.

## The argument

### Define the Core Substrate
- **Anchor Timestamps**: ['00:01:54']
- **Claim**: Three protocols form the foundational stack: MCP for tool/data discovery, A2A for agent-to-agent coordination, and AGUI for human control and state sharing. These map directly to the fundamental questions of what an agent can use, who it works with, and how humans stay in control.
- **Role**: definition

### MCP Enables Access, Not Safety
- **Anchor Timestamps**: ['00:03:11']
- **Claim**: MCP standardizes tool access, solving the 'glue' problem for integrations. However, it enables arbitrary code execution and data access, meaning it is not a security boundary by default. Builders must implement their own scopes, approval flows, and audit trails to mitigate risks like tool poisoning.
- **Role**: evidence

### A2A Adds Coordination Complexity
- **Anchor Timestamps**: ['00:06:26']
- **Claim**: A2A allows agents to delegate work via 'agent cards,' but this introduces latency, failure modes, and permission challenges. It is only necessary when an agent lacks the expertise or authority to complete a task alone, requiring careful design of what information is shared or withheld.
- **Role**: evidence

### AGUI Solves Supervision Debt
- **Anchor Timestamps**: ['00:08:57']
- **Claim**: Traditional apps handle call-and-response, but long-running agents need streaming state, shared context, and approval points. AGUI provides the control layer to prevent 'supervision debt' by allowing humans to observe, approve, and steer non-deterministic workflows in real-time.
- **Role**: synthesis

### Contested Layers Are Domain-Specific
- **Anchor Timestamps**: ['00:10:39']
- **Claim**: Protocols like A2UI (structured UI), AP2 (commercial trust), and X42 (machine payments) are valuable but narrow. They do not form a universal substrate because they solve specific, often contested, problems like rendering safety or cross-border payment authorization rather than general agentic operation.
- **Role**: counter

## Evidence and caveats

MCP has over 14,000 servers but lacks native security, requiring external scopes and audit trails to prevent tool poisoning attacks (Invariant Labs research). A2A requires a critical mass of partners (50+ including Atlassian, Box) to work across boundaries. AGUI is still early in adoption but essential for non-deterministic workflows. Payment protocols (AP2, X42, Stripe) are highly fragmented by geography and user trust, making them 'customer experience choices' rather than just technical ones. The speaker notes that many teams are overfocused on model selection while underspecifying the operating surface.

## Concepts surfaced

[[model-selection-bias]] · [[security-by-design]] · [[human-in-the-loop]] · [[agent-coordination]] · [[tool-poisoning]] · [[agentic-commerce]]
