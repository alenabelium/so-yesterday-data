---
video_id: z1EaBe9oIME
template_id: concept
template_version: 1
source_summary: ../summaries/2026-10-14-the-3-levels-of-harness-engineering-beginner-to-pro.md
source_transcript: ../transcripts/2026-10-14-the-3-levels-of-harness-engineering-beginner-to-pro.md
source_summary_hash: sha256:05b17874eedba25aa4cfd49254dbb96945e4903f637c0507a0f877f8f0040157
source_transcript_hash: sha256:755bf36c756209b3148aea804c98583b2471d26a7eda9f46dd24afb931dcecf3
fill_id: ab9d52b1-4903-4ce6-a9d3-1b0b4e8f0545
published_at: '2026-10-15T14:14:13.625629'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

Most developers stop at configuring vendor-provided coding harnesses, but true AI engineering requires building custom tools and orchestration systems. This video breaks down the three levels—configuration, custom tools, and orchestration—showing how each unlocks more power and control. Understanding these levels is key to advancing your AI engineering career.

## The argument

### Define the Harness and Its Components
- **Anchor Timestamps**: ['00:01:47']
- **Claim**: An agent is the model plus the harness. The harness defines the environment: rules, tools, checks, hooks, memory files, and sandboxing. It's what empowers the agent and controls its actions.
- **Role**: definition

### Level 1: Configuration with Memory Files and Hooks
- **Anchor Timestamps**: ['00:04:10']
- **Claim**: Configuration involves using vendor harnesses like Claude Code, setting rules in agents.md, and adding hooks to enforce behaviors. This is the entry level, but most developers never go beyond it.
- **Role**: definition

### Level 2: Custom Tools for Control and Performance
- **Anchor Timestamps**: ['00:07:47']
- **Claim**: Building custom tools allows organizations to implement policies, control tool access, and optimize for specific models. Evidence shows that custom tooling can dramatically improve model performance, as seen with LangChain's experiment and Ken Bullock's results.
- **Role**: evidence

### Level 3: Orchestration for Long-Running and Multi-Agent Systems
- **Anchor Timestamps**: ['00:13:22']
- **Claim**: Orchestration harnesses manage multiple coding agents, enabling long-running tasks and swarms. Examples like AutoForge and the 3D software factory show how to scale work across many agents autonomously.
- **Role**: synthesis

## Evidence and caveats

The speaker cites LangChain's experiment where a custom CLI tool improved GPT-5.2's results from 53% to 66%, and Ken Bullock's post where changing the toolkit boosted Grok Code Fast One's score from 6.7% to nearly 70%. He also shares his own experience with Small Coder, a custom tool that reduces context usage to 1,400 tokens for local models, compared to 30,000+ tokens with Claude Code. Caveats: The speaker notes that custom tools require technical skill, and orchestration systems can be complex to set up. He also mentions that the 3D software factory is open source, but does not provide detailed setup instructions.

## Concepts surfaced

[[harness-engineering]] · [[agent-environment]] · [[custom-tools]] · [[orchestration]] · [[memory-files]] · [[hooks]]
