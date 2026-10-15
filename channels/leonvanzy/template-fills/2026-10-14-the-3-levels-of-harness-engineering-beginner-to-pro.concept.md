---
video_id: z1EaBe9oIME
template_id: concept
template_version: 1
source_summary: ../summaries/2026-10-14-the-3-levels-of-harness-engineering-beginner-to-pro.md
source_transcript: ../transcripts/2026-10-14-the-3-levels-of-harness-engineering-beginner-to-pro.md
source_summary_hash: sha256:05b17874eedba25aa4cfd49254dbb96945e4903f637c0507a0f877f8f0040157
source_transcript_hash: sha256:755bf36c756209b3148aea804c98583b2471d26a7eda9f46dd24afb931dcecf3
fill_id: 57967447-d1e5-4cee-b59e-bd8910af778c
published_at: '2026-10-15T08:14:49.117832'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

Most developers treat AI coding tools as fixed environments, but true AI engineering requires building your own. The speaker outlines three levels: configuration, custom tools, and orchestration. Mastering all three is key to a career in AI engineering.

## The argument

### Define the Agent and Environment
- **Anchor Timestamps**: ['00:01:47']
- **Claim**: The agent is the model itself, and the environment is the setting where it operates. The environment defines rules, assigns tools, and provides checks like tests and hooks, shaping the agent's behavior.
- **Role**: definition

### Level 1: Configuration
- **Anchor Timestamps**: ['00:04:10']
- **Claim**: At the first level, you configure a vendor-provided harness like Claude Code. This involves editing memory files (e.g., agents.md) to set rules, using composite files, and adding hooks to enforce behaviors like changelog updates.
- **Role**: definition

### Level 2: Custom Tools
- **Anchor Timestamps**: ['00:07:47']
- **Claim**: The second level is creating your own tools. This allows organizations to control developer experience, switch providers, and implement policies. Custom tools can dramatically improve model performance, as shown by LangChain's experiment and Ken Bullock's results.
- **Role**: evidence

### Level 3: Orchestration
- **Anchor Timestamps**: ['00:13:25']
- **Claim**: The third level is orchestration: managing multiple agents in a swarm. Examples include AutoForge and a 3D software factory where agents work on real projects, connected to GitHub, and can handle hundreds of tasks in the background.
- **Role**: synthesis

## Evidence and caveats

The speaker cites LangChain's experiment where a custom CLI tool improved GPT-5.2's results from 53% to 66%, and Ken Bullock's post where changing tools boosted Grok Code Fast One's score from 6.7% to nearly 70%. He also shares personal experience with open-weight models, noting that standard tools are not optimized for local models, and his custom tool uses only 1400 tokens compared to Claude's 30,000. He acknowledges that not all details are covered and refers to other videos for deeper dives.

## Concepts surfaced

[[ai-agents]] · [[environment-engineering]] · [[custom-tools]] · [[orchestration]] · [[claude-code]] · [[open-source-ai]]
