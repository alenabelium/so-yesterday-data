---
video_id: QWzLPn164w0
template_id: concept
template_version: 1
source_summary: ../summaries/2026-02-24-prompt-engineering-is-dead-context-engineering-is-dying-what.md
source_transcript: ../transcripts/2026-02-24-prompt-engineering-is-dead-context-engineering-is-dying-what.md
source_summary_hash: sha256:c3164093cd02f7c2c48bd1463d02cf8d4e9f4e7a7177044fa6ded5f48eda1c30
source_transcript_hash: sha256:f0d8401869050359dbb41b81afe6e66b19a742b149953f72b3ffa7aa7f0bb5d3
fill_id: fea5b186-0e1c-46e5-9806-534979f206e3
published_at: '2026-10-20T01:02:04.646640'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

Intent engineering is the discipline of encoding organizational purpose—goals, values, tradeoffs, decision boundaries—as machine-readable, machine-actionable parameters. It tells autonomous agents what to want, not just what to know. As agents run for weeks and months, this layer determines whether they optimize for what the company actually needs or just what it can measure.

## The argument

### The Intent Gap: When AI Succeeds at the Wrong Thing
- **Anchor Timestamps**: ['00:00:00']
- **Claim**: Klarna's AI agent resolved tickets 5x faster and saved $60M, but the CEO admitted the cost of the rollout exceeded the savings because the agent optimized for resolution speed rather than customer relationships. This illustrates the gap between context (what AI knows) and intent (what AI wants).
- **Role**: definition

### From Prompt to Context to Intent: The Evolution
- **Anchor Timestamps**: ['00:05:14']
- **Claim**: Prompt engineering was individual, synchronous, session-based. Context engineering shifted to crafting the entire information state an AI operates within. Intent engineering is the third discipline: encoding organizational purpose as structured, actionable parameters that shape autonomous decision-making.
- **Role**: definition

### The Three Layers of the Intent Gap
- **Anchor Timestamps**: ['00:11:16']
- **Claim**: The intent gap operates across three distinct layers: unified context infrastructure (the data and access layer), coherent AI worker toolkit (shared workflows and tools), and intent engineering proper (machine-readable expressions of organizational intent). Getting all three right is the difference between having AI tools and being an AI-native organization.
- **Role**: synthesis

### Why Intent Engineering Hasn't Been Built Yet
- **Anchor Timestamps**: ['00:20:41']
- **Claim**: It's genuinely new—before long-running autonomous agents, the human was the intent layer. It's a two-cultures problem: executives understand strategy, engineers build agents, and neither speaks the other's language. And it's hard: most organizations have never had to make their tacit knowledge explicit and structured.
- **Role**: counter

### The Solution: Goal Translation Infrastructure
- **Anchor Timestamps**: ['00:24:09']
- **Claim**: The solution is a composable, vendor-agnostic architecture with an organizational capability map and goal translation infrastructure that converts human-readable objectives into agent-actionable parameters. Early sketches exist (Google's ADK, DeepMind's five autonomy levels), but the integrated system is white space.
- **Role**: synthesis

## Evidence and caveats

Klarna's agent handled 2.3M conversations in the first month across 23 markets and 35 languages, dropping resolution times from 11 minutes to 2. The CEO told Bloomberg that cost was a predominant factor but the result was lower quality. The company rehired human agents. Microsoft Copilot: 85% of Fortune 500 adopted, but only 5% scaled beyond pilots and only 3% of M365 users became paid users. Gartner predicts 15% of day-to-day work decisions will be autonomous by 2028. Deloitte's 2026 report: 84% of companies haven't redesigned jobs around AI, only 21% have mature agent governance, and 74% report no tangible value from AI. Caveats: The speaker notes the AI agent may have inadvertently reflected Klarna's real values (saving money first). He also cautions that agents are 'rather undependable actors' and need human oversight. The numbers are from surveys and may not capture the full picture.

## Concepts surfaced

[[context-engineering]] · [[prompt-engineering]] · [[agent-governance]] · [[model-context-protocol]] · [[okrs]] · [[ai-agents]]
