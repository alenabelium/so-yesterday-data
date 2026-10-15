---
video_id: z1EaBe9oIME
template_id: concept
template_version: 1
source_summary: ../summaries/2026-10-14-the-3-levels-of-harness-engineering-beginner-to-pro.md
source_transcript: ../transcripts/2026-10-14-the-3-levels-of-harness-engineering-beginner-to-pro.md
source_summary_hash: sha256:05b17874eedba25aa4cfd49254dbb96945e4903f637c0507a0f877f8f0040157
source_transcript_hash: sha256:755bf36c756209b3148aea804c98583b2471d26a7eda9f46dd24afb931dcecf3
fill_id: f9362b95-ef1f-450a-825d-1038c109993f
published_at: '2026-10-15T10:14:11.889941'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

Most developers treat AI coding tools as fixed environments, but that's only the first level of harness engineering. The real power comes from building custom tools and orchestration harnesses that manage multiple agents. Mastering these levels is key to a career in AI engineering.

## The argument

### Define the Agent and Its Environment
- **Anchor Timestamps**: ['00:00:55']
- **Claim**: The agent is the model plus its environment. The environment defines rules, tools, checks, and hooks that shape the model's behavior. Most users only configure this environment, which is the first level of harness engineering.
- **Role**: definition

### Level 1: Configuration
- **Anchor Timestamps**: ['00:04:10']
- **Claim**: Configuration involves using vendor-provided harnesses like Claude Code and tweaking memory files (agents.md) and hooks. This is the baseline that most developers use, but it's limited to what the vendor provides.
- **Role**: definition

### Level 2: Custom Tools
- **Anchor Timestamps**: ['00:07:47']
- **Claim**: Building custom tools can dramatically improve model performance. Evidence: LangChain improved GPT-5.2 from 53% to 66% with a custom CLI, and Ken Bullock boosted Grok Code Fast One from 6.7% to ~70% by changing the toolkit. Custom tools also enable organizational control and provider flexibility.
- **Role**: evidence

### Level 3: Orchestration
- **Anchor Timestamps**: ['00:12:14']
- **Claim**: Orchestration harnesses manage multiple agents, like AutoForge or a 3D software factory. These systems coordinate agents on real projects, handle task assignment, and can run hundreds of tasks autonomously. This is the frontier of harness engineering.
- **Role**: synthesis

## Evidence and caveats

The speaker cites LangChain's experiment where a custom CLI improved GPT-5.2 from 53% to 66%, and Ken Bullock's post where changing tools boosted Grok Code Fast One from 6.7% to ~70%. He also shares his own experience with local models, noting that standard tools like OpenCode and DeepSeek Coder aren't optimized for local models, but his custom tool uses only 1400 tokens versus 30,000+ for Claude. He cautions that these results are anecdotal and not universally guaranteed. The speaker emphasizes that custom tools are in high demand for organizational control, but acknowledges that building them requires some technical skill, though he offers a course for beginners.

## Concepts surfaced

[[ai-agents]] · [[claude-code]] · [[environment-engineering]] · [[orchestration]] · [[custom-tools]]
