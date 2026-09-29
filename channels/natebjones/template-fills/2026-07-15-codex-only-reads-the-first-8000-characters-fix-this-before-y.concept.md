---
video_id: PDJfciNhyHU
template_id: concept
template_version: 1
source_summary: ../summaries/2026-07-15-codex-only-reads-the-first-8000-characters-fix-this-before-y.md
source_transcript: ../transcripts/2026-07-15-codex-only-reads-the-first-8000-characters-fix-this-before-y.md
source_summary_hash: sha256:974e5c809e15ef69b0bfed7a27c8adcca93cb7592b7290c787d8264df4bdbaf5
source_transcript_hash: sha256:39800ba3d01e4b0317a8e789716e13aad36e2d65c27314b2d830f964f4f57fc0
fill_id: 0cdbafd8-5119-49fc-86f7-072c5902b624
published_at: '2026-09-29T11:20:24.639587'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

AI harnesses—the custom instructions, skills, and files surrounding a model—accumulate as 'bloat' that degrades performance. This concept introduces a systematic auditing method to map these components and identify redundant or mis-timed rules. By cleaning the harness, users can shift from blaming model failures to fixing structural configuration issues.

## The argument

### Define the AI Harness
- **Anchor Timestamps**: ['00:00:00']
- **Claim**: A harness is everything wrapped around the model—custom instructions, skills, tools, and permissions—that shapes the answer before the prompt is typed. It is often built accidentally through incremental corrections, leading to bloat.
- **Role**: definition

### Map Before Cleaning
- **Anchor Timestamps**: ['00:03:45']
- **Claim**: You must map the harness to see where controls live, when they load, and who owns them. This reveals that some controls are 'locks' (schemas/permissions) while others are just text, preventing the model from confusing instruction types.
- **Role**: definition

### Blame the Setup, Not the Model
- **Anchor Timestamps**: ['00:04:59']
- **Claim**: Testing showed that a 'thicker' harness produced richer analysis but failed delivery constraints (JSON/word limits), while a 'compact' setup succeeded. This proves that failures are often caused by the surrounding setup, not the model's capability.
- **Role**: evidence

### Enforce Hard Constraints via Schema
- **Anchor Timestamps**: ['06:56']
- **Claim**: Hard requirements (e.g., word counts, JSON formats) should be enforced via schemas that the model can test against, rather than verbose text instructions. This makes the harness lighter and safer by letting the system verify what a machine can check.
- **Role**: synthesis

## Evidence and caveats

The speaker audited their own setup, finding 66 skills and 172 instruction files, with one file containing 18,000 words. This exceeded the 8,000-character discovery budget for Codex, meaning the model couldn't read the full context. The speaker notes that 'short prompts don't always win'; the goal is to load specialist knowledge only when needed, not to starve the model of context. The cleaner skill helps identify which rules are 'locks' versus 'polite reminders' and ensures consistency across models like Fable 5 and ChatGPT 5.6.

## Concepts surfaced

[[context-window-management]] · [[system-prompt-optimization]] · [[ai-harness-design]] · [[model-evaluation]] · [[prompt-engineering]]
