---
video_id: z1EaBe9oIME
template_id: concept
template_version: 1
source_summary: ../summaries/2026-10-14-the-3-levels-of-harness-engineering-beginner-to-pro.md
source_transcript: ../transcripts/2026-10-14-the-3-levels-of-harness-engineering-beginner-to-pro.md
source_summary_hash: sha256:05b17874eedba25aa4cfd49254dbb96945e4903f637c0507a0f877f8f0040157
source_transcript_hash: sha256:755bf36c756209b3148aea804c98583b2471d26a7eda9f46dd24afb931dcecf3
fill_id: d23366e2-804f-4406-bacc-d6ba66f2f384
published_at: '2026-10-15T19:04:54.716868'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

Most developers only use the first level of harness engineering—configuration—when working with AI coding tools. To excel as an AI engineer, you must progress to creating custom tools and eventually orchestration harnesses that manage multiple agents. Understanding these three levels is crucial for building a career in AI engineering.

## The argument

### Define the Agent and Harness
- **Anchor Timestamps**: ['00:00:55']
- **Claim**: An agent is the model plus the harness. The harness defines the environment: rules, tools, checks, hooks, memory files, and sandboxing. It empowers the agent and controls its operations.
- **Role**: definition

### Level 1: Configuration
- **Anchor Timestamps**: ['00:04:10']
- **Claim**: Configuration uses vendor harnesses like Claude Code. You set rules in agents.md, add hooks for events like stop hooks, and manage memory files. This is the baseline level most developers use.
- **Role**: definition

### Level 2: Custom Tools
- **Anchor Timestamps**: ['00:07:47']
- **Claim**: Creating custom tools is in high demand. It allows organizations to control developer experience, implement policies, and optimize for specific models. Custom tools can significantly improve model performance.
- **Role**: evidence

### Level 3: Orchestration
- **Anchor Timestamps**: ['00:13:22']
- **Claim**: Orchestration harnesses control multiple coding agents. Examples include AutoForge for long-running tasks and software factories with swarms of agents. They enable autonomous, large-scale development.
- **Role**: synthesis

## Evidence and caveats

LangChain improved GPT-5.2 results from 53% to 66% with a custom CLI tool. Ken Bullock increased Grok Code Fast One's score from 6.7% to nearly 70% by changing the toolkit. The speaker built Small Coder to optimize for local models, reducing context to 1400 tokens vs. 30,000 for Claude Code. Caveats: custom tools require technical skill; orchestration may need supervision; results vary by model and task.

## Concepts surfaced

[[ai-agents]] · [[claude-code]] · [[custom-tools]] · [[orchestration]] · [[software-factory]] · [[small-coder]]
