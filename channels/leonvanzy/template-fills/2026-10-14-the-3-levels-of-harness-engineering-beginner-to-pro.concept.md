---
video_id: z1EaBe9oIME
template_id: concept
template_version: 1
source_summary: ../summaries/2026-10-14-the-3-levels-of-harness-engineering-beginner-to-pro.md
source_transcript: ../transcripts/2026-10-14-the-3-levels-of-harness-engineering-beginner-to-pro.md
source_summary_hash: sha256:05b17874eedba25aa4cfd49254dbb96945e4903f637c0507a0f877f8f0040157
source_transcript_hash: sha256:755bf36c756209b3148aea804c98583b2471d26a7eda9f46dd24afb931dcecf3
fill_id: 1bad5a6b-2668-447f-aba9-13475d7bb8da
published_at: '2026-10-16T09:04:59.261144'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

Most developers only configure AI coding tools, but that's just the first level of harness engineering. To truly excel, you must progress to creating custom tools and eventually orchestration harnesses that manage multiple agents. Mastering these levels is crucial for building a career in AI engineering.

## The argument

### Define the Harness and Its Components
- **Anchor Timestamps**: ['00:01:47']
- **Claim**: An agent is a model plus a harness. The harness defines the environment: rules, tools, checks, hooks, memory files, and sandboxing. It's what empowers the agent and controls its behavior.
- **Role**: definition

### Level 1: Configuration
- **Anchor Timestamps**: ['00:04:10']
- **Claim**: Configuration is using a vendor harness like Claude Code and tweaking it via memory files (agents.md), hooks, and settings. This is the most common level, but it's limited to what the vendor provides.
- **Role**: definition

### Level 2: Custom Tools
- **Anchor Timestamps**: ['00:07:47']
- **Claim**: Building your own tools gives you control over the model's context and tools. Evidence shows that custom tooling can dramatically improve performance—e.g., LangChain boosted GPT-5.2 from 53% to 66%, and Ken Bullock raised Grok Code Fast One from 6.7% to nearly 70%.
- **Role**: evidence

### Level 3: Orchestration
- **Anchor Timestamps**: ['00:13:22']
- **Claim**: Orchestration harnesses manage multiple agents and long-running tasks. Examples include AutoForge for autonomous feature implementation and a 'software factory' that distributes tasks among a swarm of agents, even visualized in 3D.
- **Role**: synthesis

## Evidence and caveats

The speaker cites LangChain's experiment with GPT-5.2 (53% to 66%) and Ken Bullock's post on Grok Code Fast One (6.7% to ~70%) as proof that custom tools can be a bottleneck. He also shares his own Small Coder tool, which reduces context to 1400 tokens for local models, versus 30,000+ for Claude Code. Caveats: the speaker notes that custom tools require technical skill, but says 'everyone can create their own toolkit' and offers a course. He also mentions that orchestration tools like AutoForge can run for weeks without supervision, but doesn't discuss failure modes or costs.

## Concepts surfaced

[[agentic-ai]] · [[ai-coding-tools]] · [[claude-code]] · [[open-source-ai]] · [[ai-engineering]]
