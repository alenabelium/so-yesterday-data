---
video_id: z1EaBe9oIME
template_id: concept
template_version: 1
source_summary: ../summaries/2026-10-14-the-3-levels-of-harness-engineering-beginner-to-pro.md
source_transcript: ../transcripts/2026-10-14-the-3-levels-of-harness-engineering-beginner-to-pro.md
source_summary_hash: sha256:05b17874eedba25aa4cfd49254dbb96945e4903f637c0507a0f877f8f0040157
source_transcript_hash: sha256:755bf36c756209b3148aea804c98583b2471d26a7eda9f46dd24afb931dcecf3
fill_id: 8302f423-533b-41de-994c-5f8f75f3cf1a
published_at: '2026-10-16T05:14:59.757210'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

Harness engineering has three levels: configuration, custom tools, and orchestration. Most developers stop at the first, but mastering all three is key to a career in AI engineering.

## The argument

### Define the Harness and Its Components
- **Anchor Timestamps**: ['00:01:47']
- **Claim**: An agent is a model plus a harness. The harness defines rules, tools, checks, hooks, memory files, and sandboxing. It empowers the agent and sets the environment in which it operates.
- **Role**: definition

### Level 1: Configuration with Vendor Harnesses
- **Anchor Timestamps**: ['00:04:10']
- **Claim**: Most users are at the configuration level, using vendor harnesses like Claude Code. They customize via memory files (agents.md) and hooks to enforce rules and behaviors, but they don't build their own tools.
- **Role**: definition

### Level 2: Building Custom Tools
- **Anchor Timestamps**: ['00:07:47']
- **Claim**: Creating custom tools is in high demand. Custom tools allow organizations to control developer experience, switch providers, and implement policies. Even a simple tool can drastically improve model performance, as shown by Small Coder's 1,400-token context vs. Claude's 30,000.
- **Role**: evidence

### Level 3: Orchestration Harnesses
- **Anchor Timestamps**: ['00:13:22']
- **Claim**: Orchestration harnesses manage multiple coding agents. Examples include AutoForge for long-running tasks and a software factory with a swarm of agents. These systems can run autonomously for days, handling hundreds of tasks.
- **Role**: synthesis

## Evidence and caveats

LangChain's experiment showed that a custom CLI tool improved results with the same model and prompt. Small Coder, a custom tool, uses only 1,400 tokens for the system prompt and tool definitions, making open-weight models practical on consumer hardware. However, the speaker notes that most developers never go beyond configuration, and building custom tools requires some technical skill, though a free community course teaches it. Orchestration tools like AutoForge and the 3D software factory are open source and can run for weeks, but they require significant setup and management.

## Concepts surfaced

[[ai-agents]] · [[claude-code]] · [[environment-engineering]]
