---
video_id: z1EaBe9oIME
template_id: concept
template_version: 1
source_summary: ../summaries/2026-10-14-the-3-levels-of-harness-engineering-beginner-to-pro.md
source_transcript: ../transcripts/2026-10-14-the-3-levels-of-harness-engineering-beginner-to-pro.md
source_summary_hash: sha256:05b17874eedba25aa4cfd49254dbb96945e4903f637c0507a0f877f8f0040157
source_transcript_hash: sha256:755bf36c756209b3148aea804c98583b2471d26a7eda9f46dd24afb931dcecf3
fill_id: 9900707b-3ca3-4d2c-89aa-9e5743aa2c37
published_at: '2026-10-15T21:05:12.767036'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

Most developers stop at configuring vendor tools, but true AI engineering requires building custom tools and orchestrating multi-agent systems. This video outlines three levels of harness engineering—configuration, custom tools, and orchestration—that separate beginners from pros. Mastering these levels is key to a career in AI engineering.

## The argument

### Define the Harness and Its Components
- **Anchor Timestamps**: ['00:01:47']
- **Claim**: An agent is a model plus a harness. The harness defines rules, tools, checks, hooks, memory files, and sandboxing. It empowers the agent and shapes its environment.
- **Role**: definition

### Level 1: Configuration of Vendor Harnesses
- **Anchor Timestamps**: ['00:04:10']
- **Claim**: Most developers use vendor harnesses like Claude Code and configure them via memory files (agents.md) and hooks. This level is about adapting existing tools to your needs, not building new ones.
- **Role**: definition

### Level 2: Building Custom Tools for Control and Performance
- **Anchor Timestamps**: ['00:07:47']
- **Claim**: Custom tools allow organizations to enforce policies, control provider access, and optimize for specific models. Evidence shows that changing the toolkit can dramatically improve model performance (e.g., from 6.7% to 70% on SWE-bench).
- **Role**: evidence

### Level 3: Orchestration Harnesses for Multi-Agent Systems
- **Anchor Timestamps**: ['00:13:22']
- **Claim**: Orchestration harnesses manage multiple coding agents, enabling long-running tasks and swarms. Examples like AutoForge and a 3D software factory demonstrate how to scale beyond single-agent workflows.
- **Role**: synthesis

## Evidence and caveats

The speaker cites LangChain's experiment with GPT-5.2, improving results from 53% to 66% by using a custom CLI tool. He also mentions Ken Bullock's post, where changing the toolkit raised Grok Code Fast One's score from 6.7% to nearly 70%. For local models, he built Small Coder, which reduces context usage to 1,400 tokens versus 30,000+ for Claude Code, making open-weight models practical. Caveats: The speaker notes that custom tools require technical expertise, but he offers a course for beginners. He also acknowledges that orchestration harnesses can run for weeks and require careful setup.

## Concepts surfaced

[[harness-engineering]] · [[agentic-ai]] · [[claude-code]] · [[custom-tools]] · [[orchestration]] · [[local-models]]
