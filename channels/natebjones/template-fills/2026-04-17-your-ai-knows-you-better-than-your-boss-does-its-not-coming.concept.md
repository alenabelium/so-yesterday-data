---
video_id: 4KAF72BTyCE
template_id: concept
template_version: 1
source_summary: ../summaries/2026-04-17-your-ai-knows-you-better-than-your-boss-does-its-not-coming.md
source_transcript: ../transcripts/2026-04-17-your-ai-knows-you-better-than-your-boss-does-its-not-coming.md
source_summary_hash: sha256:956ef277709e23353c9a9c8949e471fed36e9c24379ef2b9932a9f629bb90a21
source_transcript_hash: sha256:f5d013376c6655e62b35f18ce60b99424dead14da3dbca834c90fe53db00f80c
fill_id: a4229a4a-f5e3-42e5-bf7c-ab0ac521cf30
published_at: '2026-10-20T00:21:55.727873'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

Workers are building a new form of professional capital—AI context—inside fragmented, proprietary platforms they don't control. This context, composed of domain knowledge, workflow preferences, and behavioral patterns, is hard to move and often lost when switching tools or jobs. The solution is a BYOC strategy: extract your working identity into a portable, user-controlled database accessible via MCP.

## The argument

### Define the Four Layers of AI Context
- **Anchor Timestamps**: ['00:03:26']
- **Claim**: Professional AI context has four distinct layers: domain encoding (industry vocabulary, products, market dynamics), workflow calibration (how you like research structured, code reviewed, memos formatted), behavioral relationship (emergent understanding of your unstated preferences), and artifact rationale (the thinking behind your work products). Each layer is built incrementally through daily
- **Role**: definition

### The Context Gap Is a Market Failure
- **Anchor Timestamps**: ['00:11:37']
- **Claim**: This problem is universal and imminent: most workers will switch jobs, AIs, or face a new AI regime within two years. Yet there's no reliable way to evaluate or transfer AI capability. Employers resort to flying candidates in for supervised tests, and candidates have no structured way to demonstrate their AI proficiency. This is a genuine market failure, not an individual failing.
- **Role**: evidence

### Platform Incentives Block Portable Context
- **Anchor Timestamps**: ['00:13:16']
- **Claim**: Model makers have no incentive to make context portable—they want to keep you inside their ecosystem. They make it easy to get context in and hard to get it out. Memory-layer startups fail because the pain is diffuse, not acute; it's a 'candy' product, not an 'opium' product. This explains why no one has solved it on the platform side.
- **Role**: counter

### BYOC: Extract, Store, Expose via MCP
- **Anchor Timestamps**: ['00:19:38']
- **Claim**: The solution is a BYOC architecture: extract your working identity from the AI that knows you best using structured prompts, store it in a database you control (e.g., local Postgres, Supabase), and expose it via MCP so any compliant AI can read and write to it. This flips from push-based (pasting documents) to pull-based (AI queries what it needs), making context portable and evolvable.
- **Role**: synthesis

## Evidence and caveats

The speaker cites that over 60% of workers use personal AI at work, and that a well-calibrated AI can save 5–8 turns of conversation. He notes that a markdown file is a 'band-aid' and not sufficient for full behavioral calibration—it's like a 720p video versus 4K. He also acknowledges that some work AIs disable external MCPs for security, but argues most AIs need to be less locked down and that a markdown file can still help in those cases. The speaker is building extraction prompts and an OpenBrain plugin to implement this, but admits the tooling is not perfect today.

## Concepts surfaced

[[model-context-protocol]] · [[ai-memory]] · [[ai-adoption]] · [[career-capital]] · [[ai-productivity]] · [[data-portability]]
