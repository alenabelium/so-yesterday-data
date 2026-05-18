---
video_id: EpJ0CjTJSag
template_id: concept
template_version: 1
source_summary: ../summaries/2026-05-10-anthropic-and-openai-just-admitted-the-model-isnt-enough.md
source_transcript: ../transcripts/2026-05-10-anthropic-and-openai-just-admitted-the-model-isnt-enough.md
source_summary_hash: sha256:1390bdee489f5142dab638ea71c2b5c7c6c58b644c5beb6c064df529868910e4
source_transcript_hash: sha256:b78a65a2295a90af20793a6f0b1fd041ac7aef00c8d0526d23dc58eb50cab5fb
fill_id: 1f682a2f-c574-412a-a09b-71b25c45b22f
published_at: '2026-05-18T07:18:09.501204'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

The McKinsey 'Lily' breach reveals that traditional SaaS procurement sequences fail for AI agents because they treat autonomous entities as simple human users. Vendors are now shifting to infrastructure for governed agent interactions, forcing organizations to integrate technical teams earlier in the decision-making process to prevent unbounded liability.

## The argument

### The Procurement Sequence Breaks
- **Anchor Timestamps**: ['00:05:36']
- **Claim**: Traditional enterprise software is bought in a sequence where strategic decisions and procurement happen before technical implementation. This works for bounded SaaS but fails for agents because the implementation complexity—authentication, auditing, and permission composition—is effectively the strategic decision itself, not a downstream detail.
- **Role**: definition

### Agents Require Distinct Identity Models
- **Anchor Timestamps**: ['00:07:39']
- **Claim**: Unlike humans who navigate screens, agents query systems in code. If a platform does not distinguish between human users and AI agents, it cannot bound permissions or provide auditable trails. The 'Lily' incident occurred because the API did not ask who was calling, leaving endpoints unauthenticated and writable.
- **Role**: evidence

### Technical Teams Must Lead Early
- **Anchor Timestamps**: ['00:14:55']
- **Claim**: The root cause of the breach was organizational: technical voices were absent from the initial design, allowing defaults to favor speed over security. To avoid unbounded liability, technical teams must be at the table during procurement to define the 'technical default' posture before capital is committed.
- **Role**: synthesis

## Evidence and caveats

The host cites the McKinsey 'Lily' breach where an agent used SQL injection to gain writable access to 22 of 200 endpoints. He notes that while the exploit was basic, the failure was structural. Major vendors like Anthropic, OpenAI, SAP, and Salesforce are now shifting focus to agent infrastructure (e.g., headless APIs, unified data layers) rather than just models. The host hedges that this is not a silver bullet but a signal, and emphasizes that the 'Lily' incident was a procurement failure that surfaced as a security incident, not just a technical hygiene issue. He also notes that the full six-question checklist is available on his Substack.

## Concepts surfaced

[[agentic-workflows]] · [[enterprise-ai-security]] · [[procurement-processes]] · [[ai-governance]] · [[sql-injection]] · [[technical-defaults]]
