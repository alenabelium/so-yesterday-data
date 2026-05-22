---
video_id: zP6TnEiueEc
template_id: concept
template_version: 1
source_summary: ../summaries/2026-05-19-google-spent-a-year-stitching-mcp-a2a-ag-ui-together-io-toda.md
source_transcript: ../transcripts/2026-05-19-google-spent-a-year-stitching-mcp-a2a-ag-ui-together-io-toda.md
source_summary_hash: sha256:4c8b34904a207ea4aafd279d729296ea8abba04ddc0d9df8acaac260f7a76347
source_transcript_hash: sha256:e0b46ff1e9fa7ef7eee245a3f5485f6f10b9aa5bec2c5613c28e6ba96f8aac86
fill_id: 9044fe3b-42de-4383-a579-f215a457412b
published_at: '2026-05-21T23:52:07.998689'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

Six emerging protocols define the agentic substrate, but only three form the foundational stack: MCP for tool access, A2A for coordination, and AGUI for human control. The other three—A2UI, AP2, and X42—address narrower, contested domains like structured UI and payments. Builders must look past model selection to understand how these protocol layers shape security, workflow reliability, and customer trust.

## The argument

### Define the Core Substrate
- **Anchor Timestamps**: ['00:01:54']
- **Claim**: Three protocols form the foundation: MCP handles tool/data discovery, A2A handles agent-to-agent coordination, AGUI handles human-in-the-loop state sharing. These map directly to the core questions of agent capability, reach, and control.
- **Role**: definition

### MCP Enables Access, Not Safety
- **Anchor Timestamps**: ['00:03:11']
- **Claim**: MCP standardizes tool discovery, allowing agents to invoke external systems. However, it enables arbitrary code execution and data access, creating a high-trust environment that requires explicit security configurations like scopes and audit trails to prevent tool poisoning attacks.
- **Role**: evidence

### A2A Adds Coordination Complexity
- **Anchor Timestamps**: ['00:06:26']
- **Claim**: A2A allows agents to delegate tasks via 'agent cards' across boundaries. This introduces latency, failure modes, and permission challenges, making it essential only when workflows require distributed expertise beyond a single agent's scope.
- **Role**: evidence

### AGUI Solves Supervision Debt
- **Anchor Timestamps**: ['00:08:57']
- **Claim**: AGUI provides the human control layer for long-running, non-deterministic agents. It enables streaming state, approvals, and interruptions, addressing the 'supervision debt' that arises when traditional web apps fail to handle agent workflows.
- **Role**: synthesis

### Contested Layers Are Domain-Specific
- **Anchor Timestamps**: ['00:10:39']
- **Claim**: A2UI, AP2, and X42 address specific needs like structured UI rendering and payments. These are not universal substrates but specialized solutions for commerce and interface generation, requiring careful customer-experience mapping rather than broad adoption.
- **Role**: counter

## Evidence and caveats

MCP has over 14,000 servers but lacks root security design, requiring teams to implement scopes and approval flows to mitigate tool poisoning risks (Invariant Labs research). A2A relies on 'agent cards' as operating contracts, with Google launching it with partners like Atlassian and PayPal. AGUI docs specify needs like streaming and shared state, supported by frameworks like Langraph and Crew AI. A2UI uses trusted component catalogs to avoid arbitrary HTML execution. AP2 uses cryptographically signed mandates for payment authorization, while X42 handles HTTP-native agent-to-agent payments. The speaker notes that payment protocols are highly opinionated and geographically biased, urging builders to consider customer trust and reauthorization friction rather than just technical specs.

## Concepts surfaced

[[model-selection-trap]] · [[tool-poisoning]] · [[agent-card]] · [[supervision-debt]] · [[agentic-commerce]] · [[protocol-substrate]]
