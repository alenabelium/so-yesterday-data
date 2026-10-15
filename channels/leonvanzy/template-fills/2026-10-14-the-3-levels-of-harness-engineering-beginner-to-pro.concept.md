---
video_id: z1EaBe9oIME
template_id: concept
template_version: 1
source_summary: ../summaries/2026-10-14-the-3-levels-of-harness-engineering-beginner-to-pro.md
source_transcript: ../transcripts/2026-10-14-the-3-levels-of-harness-engineering-beginner-to-pro.md
source_summary_hash: sha256:05b17874eedba25aa4cfd49254dbb96945e4903f637c0507a0f877f8f0040157
source_transcript_hash: sha256:755bf36c756209b3148aea804c98583b2471d26a7eda9f46dd24afb931dcecf3
fill_id: c4560a44-64f7-4ff8-8509-a69ab9698b5a
published_at: '2026-10-15T06:14:10.395698'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

Most developers stop at configuring vendor-provided AI coding tools, but that's only the first level of harness engineering. The second level involves building custom tools to control the developer experience and boost model performance. The third level is orchestration, where you manage multiple agents to work on long-running tasks autonomously.

## The argument

### Define the Harness and Its Components
- **Anchor Timestamps**: ['00:01:47']
- **Claim**: A harness is the environment that defines rules, tools, checks, hooks, memory files, and sandboxing for an AI agent. It's what empowers the model to act, and it can be extended with subagents and workflows.
- **Role**: definition

### Level 1: Configuration
- **Anchor Timestamps**: ['00:04:10']
- **Claim**: Configuration is using a vendor harness like Claude Code and tweaking it via memory files (agents.md) and hooks. This is where most developers are, but it's just the starting point.
- **Role**: definition

### Level 2: Custom Tools
- **Anchor Timestamps**: ['00:07:47']
- **Claim**: Building your own tools lets you control the developer experience, enforce policies, and optimize for specific models. Evidence shows that custom tooling can dramatically improve model performance, e.g., from 53% to 66% in a LangChain experiment.
- **Role**: evidence

### Level 3: Orchestration
- **Anchor Timestamps**: ['00:13:22']
- **Claim**: Orchestration harnesses manage multiple coding agents to handle long-running tasks, like AutoForge or a software factory. They distribute tasks among agents and run autonomously until completion.
- **Role**: synthesis

## Evidence and caveats

The speaker cites a LangChain experiment where the same model improved from 53% to 66% with a custom CLI tool. Ken Bullock's post shows Grok Code Fast's score jumping from 6.7% to nearly 70% by changing the toolkit. The speaker's own Small Coder tool reduces context to 1400 tokens for local models, while Claude Code uses over 30,000 tokens before any message. Caveats: the speaker notes that custom tools are in high demand but may require technical skills, and orchestration systems like AutoForge can run for weeks without supervision.

## Concepts surfaced

[[ai-agents]] · [[claude-code]] · [[software-factory]] · [[small-coder]] · [[harness-engineering]]
