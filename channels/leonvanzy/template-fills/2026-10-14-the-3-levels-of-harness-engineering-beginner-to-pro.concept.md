---
video_id: z1EaBe9oIME
template_id: concept
template_version: 1
source_summary: ../summaries/2026-10-14-the-3-levels-of-harness-engineering-beginner-to-pro.md
source_transcript: ../transcripts/2026-10-14-the-3-levels-of-harness-engineering-beginner-to-pro.md
source_summary_hash: sha256:05b17874eedba25aa4cfd49254dbb96945e4903f637c0507a0f877f8f0040157
source_transcript_hash: sha256:755bf36c756209b3148aea804c98583b2471d26a7eda9f46dd24afb931dcecf3
fill_id: d6bdbe2e-5d74-4b2f-9c8d-b20ffd40775b
published_at: '2026-10-15T11:14:12.321464'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

Most developers treat AI coding tools as fixed environments, but that's only the first level of harness engineering. The real skill is progressing from configuration to custom tools and finally to orchestration harnesses that manage multiple agents. Mastering these levels is key to a career in AI engineering.

## The argument

### Define the Agent and Environment
- **Anchor Timestamps**: ['00:01:47']
- **Claim**: The agent is the model itself, and the environment is the setting that defines rules, tools, and checks. Hooks allow intercepting lifecycle events, like checking requests for sensitive information.
- **Role**: definition

### Level 1: Configuration
- **Anchor Timestamps**: ['00:04:10']
- **Claim**: Configuration means using a vendor harness like Claude Code and tailoring it via memory files (agents.md) and hooks. The agents.md file is an open standard, and you can break rules into separate files for better structure.
- **Role**: definition

### Level 2: Custom Tools
- **Anchor Timestamps**: ['00:07:47']
- **Claim**: Building your own tools gives you control over the developer experience, provider choice, and policies. Evidence shows that custom tooling can dramatically improve model performance, e.g., LangChain boosted GPT-5.2 from 53% to 66%.
- **Role**: evidence

### Level 3: Orchestration
- **Anchor Timestamps**: ['00:13:30']
- **Claim**: Orchestration harnesses manage multiple agents, like a swarm of coding agents working on real projects. These systems can handle hundreds of tasks, run in the background, and integrate with tools like GitHub.
- **Role**: synthesis

## Evidence and caveats

The speaker cites a LangChain experiment where a custom CLI tool improved GPT-5.2 results from 53% to 66%. Also, Ken Bullock increased Grok Code Fast One's score from 6.7% to nearly 70% by changing the toolkit. The speaker's own experience with open-weight models shows that standard tools are not optimized for local models, but a custom tool can reduce token usage to 1400 tokens. He notes that custom tools are in high demand for organizational control and consistency across providers. He also mentions that the 3D software factory is open source and available for use.

## Concepts surfaced

[[ai-agents]] · [[claude-code]] · [[environment-engineering]] · [[custom-tools]] · [[orchestration-harness]]
