---
video_id: 3mUslD_jtV4
template_id: concept
template_version: 1
source_summary: ../summaries/2026-10-26-busy-beaver-number-world-records-bb10-is-bigger-than-grahams.md
source_transcript: ../transcripts/2026-10-26-busy-beaver-number-world-records-bb10-is-bigger-than-grahams.md
source_summary_hash: sha256:cf6640da9f443dea7a51ae93fc04be270e320c4517adcc542a58c122a28d56e0
source_transcript_hash: sha256:d4235eff98d75bde68214e33e6ad46bb26ed792e1b15f8895fffdf9e76142e8f
fill_id: 2065867a-f473-4bff-9daf-629f12c91494
published_at: '2026-11-03T07:50:42.429800'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

The busy beaver function measures the longest-running halting programs of a given size, making it a canonical uncomputable function. Recent AI-assisted results have pushed records to new extremes, including a 230-state machine whose halting is independent of ZFC and a proof that BB(10) exceeds Graham's number. These breakthroughs are sparking controversy about AI's role in mathematics and raising deep questions about the limits of computation.

## The argument

### Define the Busy Beaver Function
- **Anchor Timestamps**: ['00:00:55']
- **Claim**: The busy beaver function is a family of functions that measure the maximum number of steps (shift function) or output (sigma function) a Turing machine of a given size can perform before halting, starting from a blank tape. It is a canonical example of an uncomputable function.
- **Role**: definition

### ZFC-Independent Machines Shrink to 230 States
- **Anchor Timestamps**: ['00:02:19']
- **Claim**: A 230-state Turing machine has been constructed whose halting is independent of ZFC, meaning set theory cannot decide whether it halts. This dramatically improves on the original 8,000-state machine and shows that such independence arises at surprisingly small sizes.
- **Role**: evidence

### BB(10) Surpasses Graham's Number
- **Anchor Timestamps**: ['00:10:52']
- **Claim**: Using Claude code agents, Jeffrey Ketcheson proved that the 10th busy beaver number exceeds Graham's number, a famous astronomically large number. This improves the previous bound of BB(13) and highlights the function's extraordinary growth rate.
- **Role**: evidence

### AI's Role Sparks Controversy
- **Anchor Timestamps**: ['00:16:57']
- **Claim**: The busy beaver community is debating whether AI-assisted results should be credited to humans, with some arguing that prompt engineering is not real work. This controversy mirrors broader discussions about human accountability in AI-driven mathematics.
- **Role**: counter

### Uncomputability Limits AI's Reach
- **Anchor Timestamps**: ['00:19:12']
- **Claim**: Despite AI's successes, the busy beaver function is uncomputable, so no AI can ever solve all its values. This underscores a fundamental limit: while AI can push boundaries, it cannot fully automate the search for busy beaver numbers.
- **Role**: synthesis

## Evidence and caveats

The 230-state machine was verified by Roque and beats previous records (Aaronson's 243-state and Mira's 254-state). The BB(10) result is confirmed by a specific machine, but the analysis is credited to Claude and has not yet been independently verified, though it has been checked in Coq. The presenter notes that computing exact busy beaver values remains extremely difficult due to the exponential number of machines to analyze. The biological busy beaver numbers, inspired by ancestry simulations, are a new research direction but are based on probabilistic assumptions.

## Concepts surfaced

[[turing-machines]] · [[uncomputability]] · [[zfc]] · [[grahams-number]] · [[ai-in-mathematics]]
