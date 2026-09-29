---
video_id: gYtQ1LKSgXY
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-09-14-the-harness-that-runs-claude-code-and-codex-together.md
source_transcript: ../transcripts/2026-09-14-the-harness-that-runs-claude-code-and-codex-together.md
source_summary_hash: sha256:a1d412756501fee052de961b9b70536c5b17fac76facb90e4d6319d656ed25be
source_transcript_hash: sha256:e4022e9dbc82e6c2b44999fd4a73f668fa5e0b757081a84c72655bc578ba48e9
fill_id: 115ece11-6a35-4488-bce5-6068a1fb70d8
published_at: '2026-09-29T11:24:33.123279'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Omnigen unifies Claude Code and Codex into a single harness with shared context, multi-agent debate via Debbie, and safety policies against the lethal trifecta.

## Prerequisites

### WSL
- **Kind**: os
- **Note**: Windows users must use WSL to run Omnigen.

### Claude Code/Codex Keys
- **Kind**: account
- **Note**: Provider API keys or subscriptions configured for the agents.

## Steps

### Install Omnigen via CLI
- **Timestamp**: [01:10](https://www.youtube.com/watch?v=gYtQ1LKSgXY&t=70)
- **Action**: Run the setup command in your terminal. Windows users must use WSL.
- **Command Or Clicks**: omni setup

### Launch Omnigen Interface
- **Timestamp**: [01:45](https://www.youtube.com/watch?v=gYtQ1LKSgXY&t=105)
- **Action**: Start the browser-based UI to manage sessions and agents.
- **Command Or Clicks**: omni

### Configure Safety Policies
- **Timestamp**: [04:10](https://www.youtube.com/watch?v=gYtQ1LKSgXY&t=250)
- **Action**: Add global or session-level policies to block the 'lethal trifecta' of data exfiltration.
- **Command Or Clicks**: Policies -> Add Policy -> Deny PII in LLM requests

### Start a Coding Session
- **Timestamp**: [06:02](https://www.youtube.com/watch?v=gYtQ1LKSgXY&t=362)
- **Action**: Launch a specific agent like Claude Code within the harness.
- **Command Or Clicks**: omni claude

### Initiate Multi-Agent Debate
- **Timestamp**: [08:46](https://www.youtube.com/watch?v=gYtQ1LKSgXY&t=526)
- **Action**: Fork a session to the Debbie agent to consolidate reviews from multiple providers.
- **Command Or Clicks**: Fork -> Select 'Debbie' -> Clone and Start

### Distribute Implementation Work
- **Timestamp**: [11:35](https://www.youtube.com/watch?v=gYtQ1LKSgXY&t=695)
- **Action**: Use Polly to break plans into components and distribute them across different sub-agents.
- **Command Or Clicks**: Fork -> Select 'Polly' -> Clone and Start

## Gotchas

### The 'lethal trifecta' (reading private files, reading external text, sending data out) allows data theft if not blocked by policies.
- **Severity**: blocking
- **Timestamp**: [04:10](https://www.youtube.com/watch?v=gYtQ1LKSgXY&t=250)

### Windows users cannot run Omnigen natively and must use WSL.
- **Severity**: blocking
- **Timestamp**: [01:10](https://www.youtube.com/watch?v=gYtQ1LKSgXY&t=70)

## Where to go next

Explore Polly's orchestration capabilities for complex multi-step workflows or configure custom agents with specific MCP servers.

## Concepts surfaced

[[multi-agent-debate]] · [[ai-safety-policies]] · [[coding-harness]] · [[lethal-trifecta]]
