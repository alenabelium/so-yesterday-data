---
video_id: 4HvFqhtCb-A
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-08-21-stop-paying-200-for-work-an-18-model-can-do-inside-claude-co.md
source_transcript: ../transcripts/2026-08-21-stop-paying-200-for-work-an-18-model-can-do-inside-claude-co.md
source_summary_hash: sha256:90b3ba07e9ad46df99e8b963dc0142e508ef15c73b49f1357048d97465834fa3
source_transcript_hash: sha256:bb81100e80efb2514b8ee5e07c3cb9ff1df21575faa0e39bde147dabfd245898
fill_id: ef4c20e5-1dd9-4a36-8ce3-45bb89aba7a7
published_at: '2026-09-29T11:22:59.945114'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Save money by running GLM 5.3 inside Claude Code or Codex for bounded tasks.

## Prerequisites

### Z.ai Account
- **Kind**: account
- **Note**: Requires a Z.ai subscription starting at $18/month to access GLM models.

### Claude Code or Codex
- **Kind**: tool
- **Note**: Existing harness installation needed to configure the external model provider.

### API Key Management
- **Kind**: knowledge
- **Note**: Understand how to store secrets securely, not in project files.

## Steps

### Launch GLM session via CLI
- **Timestamp**: [07:22](https://www.youtube.com/watch?v=4HvFqhtCb-A&t=442)
- **Action**: Create a private launch command that supplies the Z.ai API key, address, and model mapping before opening Claude Code.
- **Command Or Clicks**: Launch custom command supplying z.ai API key, address, and GLM 5.3 model names.

### Verify context loading
- **Timestamp**: [08:34](https://www.youtube.com/watch?v=4HvFqhtCb-A&t=514)
- **Action**: Open the same repository to confirm that project files, hooks, and permissions load correctly while using the new model.
- **Command Or Clicks**: Open repository in new session to verify file and hook inheritance.

### Configure Codex profile
- **Timestamp**: [12:45](https://www.youtube.com/watch?v=4HvFqhtCb-A&t=765)
- **Action**: Add Z.ai as a provider in Codex config, set the environment variable for the key, and create a GLM profile.
- **Command Or Clicks**: Set z.ai address and env var in Codex config; create GLM profile.

### Execute handoff protocol
- **Timestamp**: [09:58](https://www.youtube.com/watch?v=4HvFqhtCb-A&t=598)
- **Action**: Write a handoff file detailing goals, state, constraints, and tests before switching models to avoid lost context.
- **Command Or Clicks**: Create handoff file with goal, state, constraints, and test commands.

## Gotchas

### Switching providers mid-session reloads history without prompt caches, increasing cost and latency significantly.
- **Severity**: serious
- **Timestamp**: [04:24](https://www.youtube.com/watch?v=4HvFqhtCb-A&t=264)

### Never store API keys in project files; use environment variables or secret managers instead.
- **Severity**: blocking
- **Timestamp**: [07:22](https://www.youtube.com/watch?v=4HvFqhtCb-A&t=442)

### Forked sub-agents must use the same model as the parent, preventing provider switching within a single thread.
- **Severity**: serious
- **Timestamp**: [11:03](https://www.youtube.com/watch?v=4HvFqhtCb-A&t=663)

## Where to go next

Download companion guides on Substack for launcher scripts, handoff templates, and comparison scorecards to implement these configurations safely.

## Concepts surfaced

[[model-unbundling]] · [[cost-optimization]] · [[context-hygiene]] · [[multi-agent-workflows]] · [[prompt-caching]]
