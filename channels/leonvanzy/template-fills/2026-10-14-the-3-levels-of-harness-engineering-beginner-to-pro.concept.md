---
video_id: z1EaBe9oIME
template_id: concept
template_version: 1
source_summary: ../summaries/2026-10-14-the-3-levels-of-harness-engineering-beginner-to-pro.md
source_transcript: ../transcripts/2026-10-14-the-3-levels-of-harness-engineering-beginner-to-pro.md
source_summary_hash: sha256:05b17874eedba25aa4cfd49254dbb96945e4903f637c0507a0f877f8f0040157
source_transcript_hash: sha256:755bf36c756209b3148aea804c98583b2471d26a7eda9f46dd24afb931dcecf3
fill_id: fb336def-ac2d-4def-a034-af1b8dd7d5d6
published_at: '2026-10-15T09:14:06.383613'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

Most developers treat AI coding tools as fixed environments, but that's only the first level of harness engineering. The second level involves building custom tools that can dramatically boost model performance. The third level is orchestration—managing fleets of agents. Mastering these levels is key to a career in AI engineering.

## The argument

### Define the Agent and Its Environment
- **Anchor Timestamps**: ['00:00:55']
- **Claim**: An agent is the model plus its environment. The environment defines rules, tools, checks, and hooks. Most users stop at configuring a vendor-provided harness, but that's just the first level.
- **Role**: definition

### Level 1: Configuration
- **Anchor Timestamps**: ['00:04:10']
- **Claim**: Configuration means tweaking memory files like agents.md and adding hooks. This is the baseline, but it's limited because you're working within someone else's harness.
- **Role**: definition

### Level 2: Custom Tools
- **Anchor Timestamps**: ['00:07:47']
- **Claim**: Building your own tools lets you control the developer experience, enforce policies, and switch providers. Evidence shows simple tooling changes can boost model scores from 53% to 66% or even 6.7% to 70%.
- **Role**: evidence

### Level 3: Orchestration
- **Anchor Timestamps**: ['00:14:33']
- **Claim**: Orchestration harnesses manage multiple agents, like a 3D software factory with a Kanban board and GitHub integration. This is the pro level, enabling massive parallel work.
- **Role**: synthesis

## Evidence and caveats

The speaker cites LangChain's experiment with GPT-5.2, improving results from 53% to 66% with a custom CLI tool. Ken Bullock's post shows Grok Code Fast One's score jumping from 6.7% to 70% by changing underlying tools. The speaker also notes that local models need optimized tools—his own harness uses only 1400 tokens versus 30,000 for Claude. Caveats: the speaker admits he may have mispronounced Ken Bullock's name, and he doesn't provide exact details on the experiments. He also mentions that orchestration tools like AutoForge and the 3D factory are open source.

## Concepts surfaced

[[ai-agents]] · [[environment-engineering]] · [[custom-tools]] · [[orchestration]] · [[claude-code]] · [[local-models]]
