---
video_id: 8jKAT8GNDE0
template_id: concept
template_version: 1
source_summary: ../summaries/2026-02-23-googles-new-ai-is-smarter-than-everyones-but-it-costs-half-a.md
source_transcript: ../transcripts/2026-02-23-googles-new-ai-is-smarter-than-everyones-but-it-costs-half-a.md
source_summary_hash: sha256:46274dadeea3342c2fddcd28156c4b17098390df0de23668c87cef8560e775a9
source_transcript_hash: sha256:c182021568403382ab3572f0d21066e4e24e77fcd7f4a86a443458f163b65d3c
fill_id: 6af1a6ff-913f-4d2a-be08-fbc01bcb690a
published_at: '2026-10-20T01:02:06.195396'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

Google's Gemini 3.1 Pro leads on pure reasoning benchmarks at a fraction of the cost, but the company doesn't need you to use it. This reveals a strategic split: Google optimizes for intelligence, while Anthropic and OpenAI optimize for tool use and sustained work. Understanding this distinction is key to choosing the right model for each task.

## The argument

### Define the Core Substrate
- **Anchor Timestamps**: ['00:00:00']
- **Claim**: Gemini 3.1 Pro is the strongest 'naked reasoner'—optimized for pure, novel reasoning on unseen problems, not for tool orchestration or sustained agentic work. This design choice reflects Google's mission to 'solve intelligence' first, then use it to solve everything else.
- **Role**: definition

### Evidence: The ARC-AGI2 Jump
- **Anchor Timestamps**: ['00:02:05']
- **Claim**: Gemini 3.1 Pro scored 77.1% on ARC-AGI2, a 46-point jump from 3 Pro's 31.1% in 90 days—the largest single-generation reasoning gain ever. This benchmark tests novel logic problems, not pattern matching, proving the model's pure reasoning capability.
- **Role**: evidence

### Counter: Equipped Reasoners Catch Up
- **Anchor Timestamps**: ['00:10:31']
- **Claim**: When given tools (search, code execution, file access), Opus 4.6 catches up and often leads—e.g., 53.1% vs 51.4% on Humanity's Last Exam with tools, and a 289 ELO lead on GDPval. This shows that for real-world tasks, tool use and sustained work matter as much as raw reasoning.
- **Role**: counter

### Synthesis: Hard Is Not One Thing
- **Anchor Timestamps**: ['00:16:11']
- **Claim**: The model landscape forces us to decompose 'hard' into distinct axes: reasoning, effort, coordination, emotional intelligence, judgment, domain expertise, and ambiguity. Each axis is automated on a different timeline by different tools, so the right question is not 'which model is smartest' but 'which model for which problem type.'
- **Role**: synthesis

## Evidence and caveats

Gemini 3.1 Pro leads on 13 of 16 benchmarks, including GPQA Diamond and Live Codebench Pro, and costs ~1/7th of Opus 4.6 ($2 vs $15 per million input tokens). It also offers configurable thinking levels (low/medium/high/max) for cost tuning. However, the host notes that benchmarks can be saturated (e.g., GPQA Diamond) and that real-world performance depends on tool integration. He also admits he doesn't have a precise number for the 'reasoning slice' of knowledge work and is skeptical of anyone who claims one. The host's examples of business reasoning problems (tax optimization, derivative pricing) are specialized and quantitative, not typical daily work.

## Concepts surfaced

[[agentic-ai]] · [[benchmark-saturation]] · [[model-routing]] · [[vertical-integration]] · [[reasoning-vs-effort]]
