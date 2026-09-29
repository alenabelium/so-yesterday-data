---
video_id: na-sQ-g2MAc
template_id: tech-overview
template_version: 1
source_summary: ../summaries/2026-05-29-exciting-ai-updates-weekly-may-29-2026.md
source_transcript: ../transcripts/2026-05-29-exciting-ai-updates-weekly-may-29-2026.md
source_summary_hash: sha256:17938a01b6916f60fc213e6b459ec298f30299425113db677a8b8117fd353bd0
source_transcript_hash: sha256:65f51e4af35103d5972bd02728b8a1d80d709c9b404482dfec97aff3e3554ffd
fill_id: e5dee370-d839-4529-847d-ea35af424fcf
published_at: '2026-05-31T15:06:01.372953'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Claude Opus 4.8 ships with "ultra code" dynamic workflows spawning up to 1,000 parallel sub-agents, as Anthropic closes the largest private AI raise in history: $65B at a $900B valuation.

## Tools covered

### GLM 5.1
- **Vendor**: Zhipu
- **Category**: multimodal
- **Timestamp**: [00:20](https://www.youtube.com/watch?v=na-sQ-g2MAc&t=20)
- **Why It Matters**: A Chinese model now sits second on the host's arena leaderboard, placing immediately behind Claude Opus and ahead of Gemini and the other frontier entrants.
- **Sota Comparison**: Ranks #2 on the leaderboard, behind only Claude Opus.
- **Sota Band**: parity
- **Access Constraint**: Open weights

### Claude Opus 4.8
- **Vendor**: Anthropic
- **Category**: agent
- **Timestamp**: [01:15](https://www.youtube.com/watch?v=na-sQ-g2MAc&t=75)
- **Why It Matters**: New default model, better than 4.7 on many benchmarks at the same price. "Ultra code" dynamic workflows orchestrate up to 1,000 parallel sub-agents with judge agents that verify completion, cutting hallucinations and mistakes.
- **Sota Comparison**: Beats Opus 4.7 across many benchmarks while holding the same price point.
- **Sota Band**: beats
- **Access Constraint**: Fast mode is 2.5x faster at 2x price

### Cursor Composer 2.5
- **Vendor**: Cursor
- **Category**: coding
- **Timestamp**: [02:38](https://www.youtube.com/watch?v=na-sQ-g2MAc&t=158)
- **Why It Matters**: A coding model built on the open-source Kimi K2.5, further trained on Cursor's proprietary coding data using Musk-company data centers. It runs only inside the Cursor editor at 10x cheaper than other models on the platform.
- **Sota Comparison**: Priced ~10x cheaper than other models in the Cursor editor.
- **Sota Band**: new
- **Access Constraint**: Cursor editor only

### Cohere Command A+
- **Vendor**: Cohere
- **Category**: coding
- **Timestamp**: [06:33](https://www.youtube.com/watch?v=na-sQ-g2MAc&t=393)
- **Why It Matters**: Cohere open-sourced its 218-billion-parameter enterprise model, which runs on just two H100 GPUs, putting a large enterprise-grade model within reach of modest hardware.
- **Sota Comparison**: 218B params running on only two H100s shows efficient open-weight enterprise scale.
- **Sota Band**: new
- **Access Constraint**: Open source

### Gemini 3.5 Flash
- **Vendor**: Google
- **Category**: multimodal
- **Timestamp**: [08:56](https://www.youtube.com/watch?v=na-sQ-g2MAc&t=536)
- **Why It Matters**: Praised for speed and raw intelligence, but users complain it was tuned to maximize benchmark scores: the model learned that doing extra steps correlates with higher scores, so it over-acts and does more than asked in iterative work.
- **Sota Comparison**: Trails Claude on iterative back-and-forth workflows despite strong benchmarks.
- **Sota Band**: behind
- **Access Constraint**: Google

### MCP Tunnels
- **Vendor**: Anthropic
- **Category**: tool
- **Timestamp**: [10:44](https://www.youtube.com/watch?v=na-sQ-g2MAc&t=644)
- **Why It Matters**: Lets a cloud-hosted managed agent reach data behind a company firewall without exposing it: you install cloudflared, dial out an encrypted outbound-only tunnel, and keep the keys inside your network instead of handing them to an external agent.
- **Sota Comparison**: Both Anthropic and OpenAI now ship this outbound-tunnel capability.
- **Sota Band**: new
- **Access Constraint**: Requires cloudflared

### Hermes Agent
- **Vendor**: Open Source
- **Category**: agent
- **Timestamp**: [13:49](https://www.youtube.com/watch?v=na-sQ-g2MAc&t=829)
- **Why It Matters**: An open-source agent that runs OpenAI's Codex and Claude inside one agent, combining two harnesses into a single collaborative workflow. The repo has roughly 172,000 stars and is built on top of Claude Code.
- **Sota Comparison**: Combines Codex and Claude in one harness; ~172k GitHub stars.
- **Sota Band**: new
- **Access Constraint**: Open source

### Devin
- **Vendor**: Cognition
- **Category**: coding
- **Timestamp**: [13:49](https://www.youtube.com/watch?v=na-sQ-g2MAc&t=829)
- **Why It Matters**: Cognition's high-quality coding assistant raised $1B at a $26B valuation. Revenue grew from $37M to nearly $500M in a year, and the system now writes 89% of its own code.
- **Sota Comparison**: Revenue from $37M to ~$500M in one year; writes 89% of its own code.
- **Sota Band**: new
- **Access Constraint**: Paid

### Cloudflare Managed Agents
- **Vendor**: Cloudflare
- **Category**: tool
- **Timestamp**: [19:12](https://www.youtube.com/watch?v=na-sQ-g2MAc&t=1152)
- **Why It Matters**: Anthropic-Cloudflare integration uses Cloudflare's global network to give agents secure isolated sandboxes, decoupling the agent "brain" from the "hands" execution environment running on Cloudflare.
- **Sota Comparison**: Decouples reasoning from execution via Cloudflare's edge sandboxes.
- **Sota Band**: new
- **Access Constraint**: Cloudflare

### Auto Research Claw
- **Vendor**: Open Source
- **Category**: agent
- **Timestamp**: [19:12](https://www.youtube.com/watch?v=na-sQ-g2MAc&t=1152)
- **Why It Matters**: An open-source self-reinforcing autonomous-research framework from Carnegie Mellon, Google, Stanford and UC Berkeley, built on Open Claw and Claude for science, alongside Google's AI co-scientist Nature paper on agent idea tournaments.
- **Sota Comparison**: Google's co-scientist cut liver-fibrosis scarring 91% in one Stanford test.
- **Sota Band**: new
- **Access Constraint**: Open source

### DeepSeek visual thinking
- **Vendor**: DeepSeek
- **Category**: reasoning
- **Timestamp**: [21:19](https://www.youtube.com/watch?v=na-sQ-g2MAc&t=1279)
- **Why It Matters**: DeepSeek can think in visual primitives rather than only text, handling counting and topological reasoning directly on images while using 90% fewer visual tokens than top commercial models.
- **Sota Comparison**: Uses 90% fewer visual tokens than leading commercial models.
- **Sota Band**: new
- **Access Constraint**: Open source

### OpenSpec
- **Vendor**: Open Source
- **Category**: coding
- **Timestamp**: [22:39](https://www.youtube.com/watch?v=na-sQ-g2MAc&t=1359)
- **Why It Matters**: An open-source spec-driven development framework for coding assistants like Claude Code and Cursor. It preserves intent and requirements in structured plain-markdown spec files in the repo, fixing the problem of context lost across scattered chat sessions.
- **Sota Comparison**: Plain-markdown specs solve intent loss across scattered AI chat sessions.
- **Sota Band**: new
- **Access Constraint**: Open source

### Atlas
- **Vendor**: Boston Dynamics
- **Category**: agent
- **Timestamp**: [29:39](https://www.youtube.com/watch?v=na-sQ-g2MAc&t=1779)
- **Why It Matters**: Boston Dynamics upgraded the Atlas humanoid so it can carry a 100-pound fridge, and Hyundai (which acquired Atlas) plans to mass-produce and deploy units.
- **Sota Comparison**: Hyundai plans mass production and deployment of Atlas units.
- **Sota Band**: new
- **Access Constraint**: Enterprise

### Obsidian
- **Vendor**: Obsidian
- **Category**: tool
- **Timestamp**: [31:08](https://www.youtube.com/watch?v=na-sQ-g2MAc&t=1868)
- **Why It Matters**: A local-first personal wiki storing everything as a directory tree of plain markdown files with wiki-style links and no database, making it an excellent memory, RAG source, and MCP target for AI agents that rescans on external edits.
- **Sota Comparison**: Plain-markdown vault, no proprietary format; ripgrep-searchable.
- **Sota Band**: parity
- **Access Constraint**: Freemium

### Cloudflare Managed Agents
- **Timestamp**: [19:12](https://www.youtube.com/watch?v=na-sQ-g2MAc&t=1152)
- **One Liner**: Host says Anthropic Claude and Cloudflare are his two most favorite tools and highly recommends looking into the managed-agents integration.
- **Sota Band**: new

### Obsidian
- **Timestamp**: [31:08](https://www.youtube.com/watch?v=na-sQ-g2MAc&t=1868)
- **One Liner**: Host strongly recommends Obsidian as a simple, useful markdown paradigm for memory and knowledge bases, noting Andrej Karpathy famously recommends it too.
- **Sota Band**: parity

## Wider context

The week's mechanism is orchestration eating economics: Opus 4.8's 1,000-agent ultra code and tools like Hermes and OpenSpec push value from single-model quality toward multi-agent workflows, while enterprises discover those agents now burn tokens at human-salary scale. The response is hybrid routing (frontier model for planning, cheap or local models for execution) and cheaper infrastructure like cloudflared MCP tunnels, and Google's and Amazon's billions into Anthropic are bids to be the compute vendor under the market leader rather than to beat it on models.

## Read next

[[agent-orchestration]] · [[sub-agents]] · [[spec-driven-development]] · [[ai-token-economics]] · [[model-context-protocol]] · [[open-source-models]]
