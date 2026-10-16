---
video_id: z1EaBe9oIME
template_id: concept
template_version: 1
source_summary: ../summaries/2026-10-14-the-3-levels-of-harness-engineering-beginner-to-pro.md
source_transcript: ../transcripts/2026-10-14-the-3-levels-of-harness-engineering-beginner-to-pro.md
source_summary_hash: sha256:05b17874eedba25aa4cfd49254dbb96945e4903f637c0507a0f877f8f0040157
source_transcript_hash: sha256:755bf36c756209b3148aea804c98583b2471d26a7eda9f46dd24afb931dcecf3
fill_id: 0585bf43-d5b9-45a2-97a6-add462eb2016
published_at: '2026-10-16T02:14:57.464281'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

Most developers stay at level one of harness engineering—configuration—but true AI engineering requires building custom tools and orchestration harnesses. Custom tools can dramatically boost model performance, and orchestration systems manage multiple agents for long-running tasks.

## The argument

### Define the Harness and Its Role
- **Anchor Timestamps**: ['00:01:47']
- **Claim**: An agent is the model plus the harness. The harness defines rules, tools, checks, hooks, memory files, and sandboxing. It empowers the agent and shapes its environment.
- **Role**: definition

### Level One: Configuration
- **Anchor Timestamps**: ['00:04:10']
- **Claim**: Configuration uses vendor harnesses like Claude Code. You set rules via agents.md, add hooks for events like stop, and manage memory files. This is the baseline most developers use.
- **Role**: definition

### Level Two: Custom Tools
- **Anchor Timestamps**: ['00:07:47']
- **Claim**: Custom tools let you control the developer experience, enforce policies, and optimize for specific models. Evidence shows simple tool changes can boost scores from 53% to 66% or 6.7% to 70%.
- **Role**: evidence

### Level Three: Orchestration
- **Anchor Timestamps**: ['00:13:22']
- **Claim**: Orchestration harnesses manage multiple agents and long-running tasks. Examples include AutoForge for autonomous feature implementation and software factories that distribute tasks among swarms of agents.
- **Role**: synthesis

## Evidence and caveats

LangChain's experiment with GPT-5.2 improved results from 53% to 66% using a custom CLI tool. Ken Bullock boosted Grok Code Fast One from 6.7% to 70% by changing tooling. The speaker's Small Coder tool reduces context to 1400 tokens for local models, while Claude Code uses over 30,000 tokens before any message. Caveats: custom tools require technical skill, and orchestration systems may need supervision for complex tasks.

## Concepts surfaced

[[ai-agents]] · [[claude-code]] · [[custom-tools]] · [[orchestration]] · [[software-factory]]
