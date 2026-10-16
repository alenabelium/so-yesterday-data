---
video_id: z1EaBe9oIME
template_id: concept
template_version: 1
source_summary: ../summaries/2026-10-14-the-3-levels-of-harness-engineering-beginner-to-pro.md
source_transcript: ../transcripts/2026-10-14-the-3-levels-of-harness-engineering-beginner-to-pro.md
source_summary_hash: sha256:05b17874eedba25aa4cfd49254dbb96945e4903f637c0507a0f877f8f0040157
source_transcript_hash: sha256:755bf36c756209b3148aea804c98583b2471d26a7eda9f46dd24afb931dcecf3
fill_id: 32ea469f-50fc-4c26-a324-15f8f5050b78
published_at: '2026-10-16T15:05:36.770039'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

Most developers treat their AI coding environment as fixed, but it's actually a harness that can be engineered. The speaker argues there are three levels of mastery: configuration, custom tools, and orchestration. Understanding these levels is key to building a career as an AI engineer.

## The argument

### Define the Harness and Its Components
- **Anchor Timestamps**: ['00:01:47']
- **Claim**: An agent is the model plus the harness. The harness defines the environment: rules, tools, checks, hooks, memory files, and sandboxing. It empowers the agent and controls its actions.
- **Role**: definition

### Level 1: Configuration with Vendor Harnesses
- **Anchor Timestamps**: ['00:04:10']
- **Claim**: The first level is configuration, where you use a vendor harness like Claude Code and tweak it via memory files (agents.md), hooks, and other settings. This is the level most developers are at, but it's just the starting point.
- **Role**: definition

### Level 2: Building Custom Tools
- **Anchor Timestamps**: ['00:07:47']
- **Claim**: The second level is creating your own custom tools. This allows you to control the developer experience, implement policies, and optimize for specific models. A custom tool can drastically reduce context overhead, as shown by the Small Coder example.
- **Role**: evidence

### Level 3: Orchestration of Multiple Agents
- **Anchor Timestamps**: ['00:13:22']
- **Claim**: The third level is orchestration, where you control multiple coding tools and agents. Examples include AutoForge for long-running tasks and a software factory with a swarm of agents. This enables autonomous, large-scale development.
- **Role**: synthesis

## Evidence and caveats

The speaker provides concrete examples: LangChain improved results with a custom CLI tool, and his own Small Coder tool uses only 1400 tokens of context versus 30,000 for Claude Code. He also shows AutoForge and a 3D software factory. However, he notes that custom tools are in high demand but not everyone needs them, and orchestration can be complex. He suggests starting with configuration and gradually moving up.

## Concepts surfaced

[[agentic-ai]] · [[ai-coding-assistant]] · [[context-window]] · [[model-context-protocol]] · [[software-factory]]
