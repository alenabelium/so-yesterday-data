---
video_id: VBwO5A546F8
template_id: concept
template_version: 1
source_summary: ../summaries/2026-09-20-elections-ultrafilters-and-hyperreals-elite-mathematicians-h.md
source_transcript: ../transcripts/2026-09-20-elections-ultrafilters-and-hyperreals-elite-mathematicians-h.md
source_summary_hash: sha256:6f518437b6ae03ca618c7563b4ce28b581230376baa929562b8edd38e5771bdb
source_transcript_hash: sha256:a14fc0319cfe1466bbc5704906c1a4f1c59c1a9d0d080e91b14770fc89a99de4
fill_id: 18df13c0-2795-47f2-9007-1daf2821abcb
published_at: '2026-10-11T17:46:26.178945'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

Numbers can vote on comparisons between functions, leading to a democracy of natural numbers. By imposing intuitive axioms on what counts as a majority, we can escape Arrow's impossibility theorem and define a coherent ordering. This yields hyperreal numbers, which include infinitesimals and infinities, making calculus rigorous without epsilons and deltas.

## The argument

### Define Majority via Voting
- **Anchor Timestamps**: ['00:03:36']
- **Claim**: A set S of voters is a majority if its support guarantees a win, regardless of other votes. This definition allows us to tally votes even with infinitely many voters, where proportional counts are meaningless.
- **Role**: definition

### Axioms for Coherent Decisions
- **Anchor Timestamps**: ['00:05:01']
- **Claim**: To ensure transitivity of the 'bigger on average' relation, we require that the intersection of any two majorities is a majority. This axiom, along with non-triviality, monotonicity, and unambiguity, forms the foundation for a coherent decision procedure.
- **Role**: definition

### Escape Arrow's Impossibility
- **Anchor Timestamps**: ['00:10:26']
- **Claim**: Arrow's theorem forces a dictator for finite voter sets, but with infinitely many natural numbers, we can satisfy all axioms without a dictator. This is equivalent to the existence of a free ultrafilter on an infinite set.
- **Role**: evidence

### Construct Hyperreals
- **Anchor Timestamps**: ['00:12:51']
- **Claim**: By taking equivalence classes of functions under the majority relation, we obtain hyperreal numbers. This system includes the reals, infinite numbers like the identity function, and infinitesimals like 1/x, which are smaller than every positive real.
- **Role**: synthesis

## Evidence and caveats

The video demonstrates the construction with sine and cosine, showing that a majority of natural numbers vote sine > cosine, despite the functions being translates. The identity function is shown to be infinite, and 1/x is infinitesimal. The speaker notes that the definition of 1/x at zero is irrelevant because a single voter doesn't affect the outcome. The proof of the free ultrafilter theorem is shown in Lean code from mathlib, but the video does not detail the proof itself. The speaker acknowledges that the transitivity axiom is counterintuitive and that our finite intuitions fail with infinity.

## Concepts surfaced

[[arrow-impossibility-theorem]] · [[hyperreal-numbers]] · [[infinitesimals]] · [[non-archimedean-ordered-fields]] · [[lean-proof-assistant]]
