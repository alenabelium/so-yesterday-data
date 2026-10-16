---
video_id: z1EaBe9oIME
template_id: concept
template_version: 1
source_summary: ../summaries/2026-10-14-the-3-levels-of-harness-engineering-beginner-to-pro.md
source_transcript: ../transcripts/2026-10-14-the-3-levels-of-harness-engineering-beginner-to-pro.md
source_summary_hash: sha256:05b17874eedba25aa4cfd49254dbb96945e4903f637c0507a0f877f8f0040157
source_transcript_hash: sha256:755bf36c756209b3148aea804c98583b2471d26a7eda9f46dd24afb931dcecf3
fill_id: ddb36c37-67e7-423b-9f60-2fd0c4af30d5
published_at: '2026-10-16T03:14:55.962863'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

Most developers stop at Level 1: configuring vendor harnesses. To excel, you must progress to Level 2: building custom tools, and Level 3: orchestrating multiple agents. Each level unlocks new capabilities and career opportunities.

## The argument

### Define the Harness and Its Components
- **Anchor Timestamps**: ['00:01:47']
- **Claim**: An agent is a model plus a harness. The harness defines the environment: rules, tools, checks, hooks, memory files, and sandboxing. It empowers the agent and controls its operations.
- **Role**: definition

### Level 1: Configuration
- **Anchor Timestamps**: ['00:04:10']
- **Claim**: Most users are at Level 1: configuring vendor harnesses like Claude Code. This involves setting rules in agents.md, using memory files, and adding hooks to enforce behaviors like changelog updates.
- **Role**: definition

### Level 2: Custom Tools
- **Anchor Timestamps**: ['00:07:47']
- **Claim**: Level 2 is creating your own tools. Custom tools can significantly improve model performance, as shown by LangChain's experiment (53% to 66%) and Ken Bullock's post (6.7% to 70%). They also allow organizational control and provider flexibility.
- **Role**: evidence

### Level 3: Orchestration
- **Anchor Timestamps**: ['00:13:22']
- **Claim**: Level 3 is orchestration: controlling multiple coding agents. Examples include AutoForge for long-running tasks and a software factory with a swarm of agents. These systems can run autonomously for days, handling hundreds of tasks.
- **Role**: synthesis

## Evidence and caveats

LangChain improved GPT-5.2 results from 53% to 66% with a custom CLI tool. Ken Bullock boosted Grok Code Fast One from 6.7% to 70% by changing tools. Small Coder, a custom tool for local models, uses only 1400 tokens vs 30,000+ for Claude Code, making open-weight models practical. Caveats: custom tools require technical skill; orchestration systems are complex and may need supervision.

## Concepts surfaced

[[ai-agents]] · [[claude-code]] · [[custom-tools]] · [[orchestration]] · [[open-source-ai]]
