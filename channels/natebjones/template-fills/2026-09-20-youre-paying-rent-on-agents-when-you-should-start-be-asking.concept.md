---
video_id: eLpRDIvOMEw
template_id: concept
template_version: 1
source_summary: ../summaries/2026-09-20-youre-paying-rent-on-agents-when-you-should-start-be-asking.md
source_transcript: ../transcripts/2026-09-20-youre-paying-rent-on-agents-when-you-should-start-be-asking.md
source_summary_hash: sha256:f6480151d841495ca5589e6f39a2e18234588642f58f3d08a186bc4113fd8180
source_transcript_hash: sha256:809db9dc72ae0ab7729bb65531015fd83d14abba26d67a30ef626c14d6ec9b55
fill_id: 2c600476-87d5-4b85-a392-2001a9b82a1c
published_at: '2026-09-29T11:24:56.580606'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

AI costs explode not from model pricing alone, but from automating inefficient legacy workflows. By wiping the slate clean and redesigning processes around business outcomes, organizations can eliminate unnecessary handoffs. This allows cheaper models to handle routine tasks while reserving expensive frontier intelligence only for complex exceptions.

## The argument

### The Cost of Legacy Automation
- **Anchor Timestamps**: ['00:06:03']
- **Claim**: Agents increase token consumption by performing more investigative work per request. Automating old processes with agents just speeds up inefficient handoffs, causing costs to multiply without delivering proportional value.
- **Role**: definition

### The Blank Sheet Redesign
- **Anchor Timestamps**: ['00:10:12']
- **Claim**: Start with the final business outcome and draw the path to get there. Eliminate steps that exist only because legacy systems couldn't share data, reducing handoffs and ensuring zero cost for obsolete work.
- **Role**: evidence

### Task-Model Matching
- **Anchor Timestamps**: ['00:18:20']
- **Claim**: Not all work requires frontier intelligence. Use classifiers to route routine, deterministic tasks to cheaper open-weight models and reserve expensive frontier models only for probabilistic edge cases.
- **Role**: synthesis

### Harness Thickness Trade-off
- **Anchor Timestamps**: ['00:23:16']
- **Claim**: Cheaper models need a 'thick harness' of structure and tools to work predictably. Frontier models need a 'thin harness' with freedom to reason. The system setup must evolve with the model choice.
- **Role**: evidence

## Evidence and caveats

The speaker notes that identifying ordinary work reliably is challenging and requires robust [[evals]]. He emphasizes that cheaper models aren't automatically right for every task; they require a 'thick harness' of specific instructions and tools. Conversely, forcing frontier models into rigid structures wastes their intelligence. The goal is to remove administrative overhead ('coral accumulating') rather than just speeding it up.

## Concepts surfaced

[[agent-harness]] · [[model-routing]] · [[eval-driven-design]] · [[process-redesign]]
