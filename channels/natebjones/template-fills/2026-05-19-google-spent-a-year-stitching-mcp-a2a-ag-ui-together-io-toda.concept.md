---
video_id: zP6TnEiueEc
template_id: concept
template_version: 1
source_summary: ../summaries/2026-05-19-google-spent-a-year-stitching-mcp-a2a-ag-ui-together-io-toda.md
source_transcript: ../transcripts/2026-05-19-google-spent-a-year-stitching-mcp-a2a-ag-ui-together-io-toda.md
source_summary_hash: sha256:4c8b34904a207ea4aafd279d729296ea8abba04ddc0d9df8acaac260f7a76347
source_transcript_hash: sha256:e0b46ff1e9fa7ef7eee245a3f5485f6f10b9aa5bec2c5613c28e6ba96f8aac86
fill_id: 4dd3754a-27c9-441c-b76a-8ff4f13c04f4
published_at: '2026-05-20T09:12:55.413525'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

Six emerging protocols define the agentic stack, but only three form the foundational substrate: MCP for tool access, A2A for agent coordination, and AGUI for human control. The other three—A2UI, AP2, and X42—address narrower, contested layers like structured UI and payments. Builders must stop hedging on model selection and focus on how these protocol choices directly shape customer trust, security, and workflow reliability.

## The argument

### Define the Core Substrate
- **Anchor Timestamps**: ['00:01:54']
- **Claim**: Three protocols form the foundation: MCP handles tool/data discovery, A2A handles agent-to-agent coordination, AGUI handles human-in-the-loop state sharing. These map to the core questions of what an agent can use, who it works with, and how humans stay in control.
- **Role**: definition

### MCP Enables Access, Not Safety
- **Anchor Timestamps**: ['00:03:11']
- **Claim**: MCP standardizes tool discovery, allowing agents to invoke systems like GitHub or Slack. However, it enables arbitrary code execution and data access, meaning it is a security boundary, not a safety feature. Builders must implement scopes and audit trails because MCP was not designed for high-trust security by default.
- **Role**: evidence

### A2A Adds Coordination Cost
- **Anchor Timestamps**: ['00:06:26']
- **Claim**: A2A allows agents to delegate work via 'agent cards' that describe skills and interfaces. While this enables distributed expertise, it introduces latency, failure surfaces, and permission complexities. It is not needed for every product, only those requiring delegated authority outside the primary agent.
- **Role**: evidence

### AGUI Solves Supervision Debt
- **Anchor Timestamps**: ['00:08:57']
- **Claim**: AGUI provides the human control layer for long-running, non-deterministic agents. It enables streaming state, approvals, and interruptions, addressing the 'supervision debt' that arises when traditional chat interfaces fail to handle complex agent workflows. Without it, humans cannot effectively steer or verify agent actions.
- **Role**: synthesis

## Evidence and caveats

The host notes that while MCP, A2A, and AGUI form the core, other protocols like A2UI (structured UI), AP2 (agent payments), and X42 (machine-to-machine payments) are 'contested' or domain-specific. He warns that MCP servers are vulnerable to 'tool poisoning' attacks via malicious metadata. He also cautions that A2A adds 'latency and failure' surfaces and that payment protocols are heavily biased toward specific geographies (e.g., US methods), requiring builders to carefully consider customer trust and authorization flows. The host emphasizes that these protocols are 'opinionated' and shape the customer experience more than the model itself.

## Concepts surfaced

[[mcp-protocol]] · [[agent-to-agent-coordination]] · [[human-in-the-loop-agents]] · [[agentic-security]] · [[protocol-substrate]] · [[customer-trust-in-ai]]
