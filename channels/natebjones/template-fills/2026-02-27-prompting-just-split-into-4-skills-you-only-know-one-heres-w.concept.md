---
video_id: BpibZSMGtdY
template_id: concept
template_version: 1
source_summary: ../summaries/2026-02-27-prompting-just-split-into-4-skills-you-only-know-one-heres-w.md
source_transcript: ../transcripts/2026-02-27-prompting-just-split-into-4-skills-you-only-know-one-heres-w.md
source_summary_hash: sha256:e477d9f4acf2b06ee84e57fe1d0be6f9b695666bd1072d1e02d227704c51ce4c
source_transcript_hash: sha256:3d2f6d99c911ecc6aa4150a2b6173002e53cc2929ecc63e5844c58b482d2e9e4
fill_id: ffc03dae-1001-419b-95d7-02276d265946
published_at: '2026-10-20T00:52:13.136552'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

Prompting has split into four distinct skills: prompt craft, context engineering, intent engineering, and specification engineering. As AI agents run autonomously for days, only the first skill is now table stakes; the real leverage lies in curating context, encoding intent, and treating your entire document corpus as agent-readable specifications. Mastering these skills is the new bottleneck for effective AI use in 2026.

## The argument

### Define the Four Disciplines
- **Anchor Timestamps**: ['00:08:58']
- **Claim**: Prompting has diverged into four distinct disciplines: prompt craft (synchronous, session-based), context engineering (curating relevant tokens), intent engineering (encoding goals and guardrails), and specification engineering (writing documents agents can execute against). Each operates at a different altitude and time horizon, and they build on each other.
- **Role**: definition

### Prompt Craft Is Now Table Stakes
- **Anchor Timestamps**: ['00:10:26']
- **Claim**: Prompt craft—the original chat-based skill—is no longer a differentiator. It's become table stakes, like typing with ten fingers. The key shift is that this model broke when agents started running for hours without checking in, because you can no longer act as the intent, context, and quality layer in real time.
- **Role**: evidence

### Context Engineering Is the New Leverage
- **Anchor Timestamps**: ['00:13:05']
- **Claim**: Context engineering—curating the optimal token set—is where the industry's attention is focused. Your prompt might be 200 tokens, but the context window is a million. The 10x effective people aren't writing better prompts; they're building better context infrastructure, like CLAUDE.md files and RAG pipelines.
- **Role**: evidence

### Intent Engineering Aligns Agent Goals
- **Anchor Timestamps**: ['13:05']
- **Claim**: Intent engineering tells agents what to want, not just what to know. It encodes organizational purpose, values, and trade-off hierarchies. The Klarna case shows the cost of misalignment: optimizing for resolution time instead of customer satisfaction led to a rehiring of human agents. Intent sits above context like strategy above tactics.
- **Role**: evidence

### Specification Engineering Is the Highest Leverage
- **Anchor Timestamps**: ['00:16:31']
- **Claim**: Specification engineering is the practice of writing documents that autonomous agents can execute against over extended time horizons. It's about making your entire organizational corpus agent-readable. The Opus 4.5 example shows that a structured spec—with a setup agent, progress log, and incremental coding—enables coherent multi-day output.
- **Role**: synthesis

## Evidence and caveats

The speaker cites concrete examples: Klarna's AI agent resolved 2.3 million conversations but optimized for the wrong metric, causing a rehiring of human agents. Anthropic's Opus 4.5 agent struggled with high-level prompts but succeeded with a structured specification. The speaker also notes that context engineering is often misunderstood as 'everything' (Harrison Chase's quote), but it's only one of four levels. He cautions that models degrade with more information, so retrieval quality matters. The 10x gap example is a hypothetical but replicable experiment. The speaker acknowledges that these skills are cumulative and that failure at higher levels has more serious consequences.

## Concepts surfaced

[[intent-engineering]] · [[context-engineering]] · [[specification-engineering]] · [[prompt-craft]] · [[autonomous-agents]] · [[agent-specifications]]
