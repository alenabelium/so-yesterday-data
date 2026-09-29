---
video_id: up0Bsf3f0Xc
template_id: concept
template_version: 1
source_summary: ../summaries/2026-08-01-i-used-to-install-claude-skills-now-i-only-use-the-ones-i-re.md
source_transcript: ../transcripts/2026-08-01-i-used-to-install-claude-skills-now-i-only-use-the-ones-i-re.md
source_summary_hash: sha256:fc04347dd652671cf50e91e8a05e1fc2310f6e708100a7ab89b3179850595f93
source_transcript_hash: sha256:54ef546f3c6917e6dfef382aed1bfda0e0dc24ab9b4739d0a8fe418302d32bbf
fill_id: 9aca9e7e-b28e-41d0-9cc0-083d7b5ff0e7
published_at: '2026-09-29T11:21:37.571718'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

AI skills are executable instructions, not static apps. Most users install unvetted skills blindly, risking security and context bloat. The core shift is treating skills as dual-audience artifacts: readable by humans for trust, and optimized for agents to avoid performance degradation.

## The argument

### Define Skills as Agent Instructions
- **Anchor Timestamps**: ['00:00:00']
- **Claim**: Skills are sets of instructions for agents, not apps. They function as recipes that activate only when needed, unlike static software installations.
- **Role**: definition

### Audit the Dual Audience
- **Anchor Timestamps**: ['00:02:12']
- **Claim**: Skills must be readable by humans for auditing and optimized for agents. If humans can't read them, trust is lost; if agents can't use them, power is lost.
- **Role**: definition

### Avoid Context Bloat
- **Anchor Timestamps**: ['00:03:52']
- **Claim**: Badly written skills fail by bloating context windows. Agents load full instructions only when invoked; vague descriptions or huge files cause confusion and poor performance.
- **Role**: evidence

### Rebuild for Lineage
- **Anchor Timestamps**: ['00:08:55']
- **Claim**: Instead of collecting skills like Pokémon cards, rebuild them to encode unique judgment. This creates a lineage of evolving capabilities rather than a static, conflicting stack.
- **Role**: synthesis

## Evidence and caveats

The speaker cites Matt Pocock's 'Grill Me' skill as a trusted, reusable example (00:06:26). However, he notes that even good skills need modification for specific goals, such as making context persistent (00:10:15). He warns against installing skills from untrusted GitHub repos, which may contain malicious instructions or simply not work with existing tasks (00:01:24). The speaker also highlights that adding skills without auditing creates a 'dangerous loop' of performance degradation due to conflicting instructions (00:15:05). He offers a 'skill builder' and an 'audit skill' to help users manage this complexity, emphasizing that most people are 'early' in adopting skills (00:06:26).

## Concepts surfaced

[[agent-skills]] · [[context-window-management]] · [[ai-auditing]] · [[skill-lineage]] · [[prompt-engineering]]
