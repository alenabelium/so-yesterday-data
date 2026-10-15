---
video_id: z1EaBe9oIME
template_id: concept
template_version: 1
source_summary: ../summaries/2026-10-14-the-3-levels-of-harness-engineering-beginner-to-pro.md
source_transcript: ../transcripts/2026-10-14-the-3-levels-of-harness-engineering-beginner-to-pro.md
source_summary_hash: sha256:05b17874eedba25aa4cfd49254dbb96945e4903f637c0507a0f877f8f0040157
source_transcript_hash: sha256:755bf36c756209b3148aea804c98583b2471d26a7eda9f46dd24afb931dcecf3
fill_id: e7763970-0003-4c9e-8693-9e03d1eeeff6
published_at: '2026-10-15T12:14:06.554414'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

Most developers treat AI coding tools as fixed environments, but that's only the first level of harness engineering. The real skill is progressing from configuring vendor tools to building custom tools and orchestration harnesses. Mastering these levels is key to a career as an AI engineer.

## The argument

### Define the Agent and Environment
- **Anchor Timestamps**: ['00:00:55']
- **Claim**: The agent is the model plus the environment. The environment defines rules, tools, checks, and hooks that shape the model's behavior. Most developers only use the provided environment, which is just the first level.
- **Role**: definition

### Level 1: Configuration
- **Anchor Timestamps**: ['00:04:10']
- **Claim**: Configuration involves using a vendor tool like Claude Code and setting rules via memory files (agents.md) and hooks. This is the baseline, but it's limited to what the vendor provides.
- **Role**: definition

### Level 2: Custom Tools
- **Anchor Timestamps**: ['00:07:47']
- **Claim**: Building your own tools can dramatically improve model performance. Examples: LangChain boosted GPT-5.2 from 53% to 66% with a custom CLI; Ken Bullock raised Grok Code Fast from 6.7% to 70% by changing the toolkit. Custom tools also enable organizational control and provider flexibility.
- **Role**: evidence

### Level 3: Orchestration
- **Anchor Timestamps**: ['00:12:14']
- **Claim**: Orchestration harnesses manage multiple agents, like AutoForge or a 3D software factory. These systems assign tasks, run agents in parallel, and integrate with real project management tools, enabling large-scale autonomous development.
- **Role**: synthesis

## Evidence and caveats

The speaker cites LangChain's experiment with GPT-5.2 (53% to 66%) and Ken Bullock's post (6.7% to 70%) as evidence that custom tools are a bottleneck. He also shares his own experience with open-weight models, noting that standard tools consume 30,000+ tokens in context, while his custom tool uses only 1,400 tokens. He cautions that these results are anecdotal and not universally replicated. He mentions that creating custom tools is accessible to everyone, with a course in his community, but acknowledges that orchestration systems are more complex and open-source projects like AutoForge are available for reference.

## Concepts surfaced

[[ai-agents]] · [[claude-code]] · [[environment-engineering]] · [[orchestration]] · [[custom-tools]] · [[agents-md]]
