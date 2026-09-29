---
video_id: MFzxIT88zfg
template_id: concept
template_version: 1
source_summary: ../summaries/2026-05-27-your-board-deck-has-a-wrong-formula-excel-wont-flag-it.md
source_transcript: ../transcripts/2026-05-27-your-board-deck-has-a-wrong-formula-excel-wont-flag-it.md
source_summary_hash: sha256:5645357fef8c542f9bd5cf273917fc6ee9cd3ca201b907cd966a906e822fdf19
source_transcript_hash: sha256:e8215186a908b07d57104be9dbda1a5e152fa2cfbdd2f7473d036d31dfa19e70
fill_id: 36a29dc5-ff24-4bf8-a43e-c8a79a618b75
published_at: '2026-06-02T17:46:11.978351'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

AI-generated Excel and PowerPoint files often contain silent, visually polished errors that standard tools won't flag. To prevent costly business mistakes, professionals must shift from prompt-centric generation to a four-stage workflow: source prep, structural blueprints, constrained creation, and hostile verification. This pipeline ensures that truth is owned by the human, not the model.

## The argument

### Define the Silent Failure Mode
- **Anchor Timestamps**: ['00:02:28']
- **Claim**: AI artifacts like financial models often have correct layouts but incorrect formulas. Excel does not flag these errors, creating a 'costume' that looks valid but contains no truth, leading to dangerous business decisions.
- **Role**: definition

### Establish Source Discipline
- **Anchor Timestamps**: ['00:08:12']
- **Claim**: Before generation, you must create an index of evidence. This involves verifying ownership, dates, status (current vs. superseded), and removing sensitive data. A messy folder leads to blended data; a controlled work packet prevents AI from guessing.
- **Role**: definition

### Enforce Structural Blueprints
- **Anchor Timestamps**: ['00:09:06']
- **Claim**: AI must produce a file specification before building the artifact. For decks, this is a narrative spine in plain English; for Excel, it is a tab architecture defining where raw data, assumptions, and calculations live. Without this blueprint, the file has no foundation.
- **Role**: definition

### Execute Constrained Creation
- **Anchor Timestamps**: ['00:10:34']
- **Claim**: Build artifacts in layers to separate logic from polish. For Excel, use three layers: load raw data, build calculation logic, then produce output views. For decks, separate storyboard (claims/evidence) from visual rendering. This prevents visual polish from hiding weak arguments.
- **Role**: evidence

### Deploy Hostile Verification
- **Anchor Timestamps**: ['00:12:48']
- **Claim**: Use a second model to act as a skeptical reviewer that enumerates issues without fixing them. This flips the task from generation to enumeration, catching unsupported claims and inconsistent formulas. The human then reviews the edit list, maintaining ownership of the truth.
- **Role**: synthesis

## Evidence and caveats

The speaker cites a personal experience where an Excel file had incorrect revenue growth formulas copied across years, yet looked like a valid financial model. He notes that models are goal-oriented and will optimize for the artifact if sources are bad. He recommends using CodeEx for building and Claude Opus 4.7 for reviewing. Caveat: Knowledge work is 'profoundly contingent on domain knowledge,' so generic 'push-button' solutions are impossible because reality has too much detail to be fully abstracted.

## Concepts surfaced

[[agentic-workflows]] · [[human-in-the-loop-verification]] · [[source-discipline]] · [[ai-reliability]] · [[office-automation]]
