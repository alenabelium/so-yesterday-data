---
video_id: z1EaBe9oIME
template_id: concept
template_version: 1
source_summary: ../summaries/2026-10-14-the-3-levels-of-harness-engineering-beginner-to-pro.md
source_transcript: ../transcripts/2026-10-14-the-3-levels-of-harness-engineering-beginner-to-pro.md
source_summary_hash: sha256:05b17874eedba25aa4cfd49254dbb96945e4903f637c0507a0f877f8f0040157
source_transcript_hash: sha256:755bf36c756209b3148aea804c98583b2471d26a7eda9f46dd24afb931dcecf3
fill_id: 188b6cb2-37f6-4f65-84c8-3fba7ad90b3b
published_at: '2026-10-16T19:04:08.780164'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

Most developers stop at configuring vendor-provided AI coding tools, but that's only the first level of harness engineering. The second level involves building custom tools to control the developer experience and unlock model performance. The third level is orchestration, where you manage multiple agents to work autonomously on complex projects.

## The argument

### Define the Harness and Its Components
- **Anchor Timestamps**: ['00:01:47', '00:03:07']
- **Claim**: An agent is the model plus the harness, where the harness defines the environment: rules, tools, checks, hooks, memory files, and sandboxing. This framing sets up the three levels of engineering that follow.
- **Role**: definition

### Level 1: Configuration of Vendor Harnesses
- **Anchor Timestamps**: ['00:04:10', '00:05:46']
- **Claim**: The first level is configuration: using tools like Claude Code and adjusting memory files (agents.md) and hooks to enforce behavior. This is where most developers operate, but it's limited by the vendor's design.
- **Role**: definition

### Level 2: Building Custom Tools
- **Anchor Timestamps**: ['00:07:47', '00:08:55']
- **Claim**: The second level is creating custom tools, which can dramatically improve model performance and allow organizational control. Evidence: LangChain improved GPT-5.2 from 53% to 66% with a custom CLI, and Ken Bullock boosted Grok Code Fast One from 6.7% to ~70% by changing the toolkit.
- **Role**: evidence

### Level 3: Orchestration of Multiple Agents
- **Anchor Timestamps**: ['00:13:22', '00:14:33']
- **Claim**: The third level is orchestration: controlling multiple coding agents (e.g., AutoForge, software factories) to handle long-running tasks autonomously. This enables scaling to hundreds of tasks without constant supervision.
- **Role**: synthesis

## Evidence and caveats

Custom tools can be built by anyone; the speaker's community offers a course. Small Coder, a custom tool, reduces context to 1400 tokens for open-weight models, making them practical on consumer hardware. Caveat: vendor tools like Claude Code consume over 30,000 tokens before any message, which is impractical for small models. The speaker notes that orchestration tools like AutoForge and software factories are open source and can run for weeks on autopilot.

## Concepts surfaced

[[ai-agents]] · [[claude-code]] · [[open-source-ai]] · [[software-factory]] · [[agent-orchestration]]
