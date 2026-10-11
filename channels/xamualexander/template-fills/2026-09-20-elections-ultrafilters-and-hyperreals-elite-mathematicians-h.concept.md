---
video_id: VBwO5A546F8
template_id: concept
template_version: 1
source_summary: ../summaries/2026-09-20-elections-ultrafilters-and-hyperreals-elite-mathematicians-h.md
source_transcript: ../transcripts/2026-09-20-elections-ultrafilters-and-hyperreals-elite-mathematicians-h.md
source_summary_hash: sha256:6f518437b6ae03ca618c7563b4ce28b581230376baa929562b8edd38e5771bdb
source_transcript_hash: sha256:a14fc0319cfe1466bbc5704906c1a4f1c59c1a9d0d080e91b14770fc89a99de4
fill_id: f40aecf7-0520-4549-af1d-5166c0174d46
published_at: '2026-10-11T22:43:22.637856'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

Numbers can vote on comparisons between functions, leading to a majority-based ordering. With infinitely many voters, we can satisfy intuitive axioms without a dictator, yielding a free ultrafilter. This constructs hyperreal numbers, which include infinitesimals and infinities, resolving a centuries-old controversy.

## The argument

### Define Majority Voting for Functions
- **Anchor Timestamps**: ['00:01:26']
- **Claim**: Each natural number n votes on whether f(n) > g(n), f(n) < g(n), or f(n) = g(n). Tallying these votes decides which function is 'bigger on average'. This works even for sine vs cosine, which are translates of each other.
- **Role**: definition

### Axioms for Majorities
- **Anchor Timestamps**: ['00:03:36']
- **Claim**: Majorities must satisfy: non-triviality (empty set is not a majority), monotonicity (supersets of majorities are majorities), unambiguity (either S or its complement is a majority), and transitivity (intersection of two majorities is a majority). These ensure coherent decisions.
- **Role**: definition

### Escape Arrow's Impossibility
- **Anchor Timestamps**: ['00:10:26']
- **Claim**: With finitely many voters, satisfying the first four axioms forces a dictator (Arrow's theorem). But with infinitely many voters, we can satisfy all five axioms, including no dictator. This is equivalent to the existence of a free ultrafilter on the naturals.
- **Role**: evidence

### Construct Hyperreals
- **Anchor Timestamps**: ['00:12:51']
- **Claim**: Blurring equivalent functions into equivalence classes yields hyperreal numbers. These include the reals, plus infinite numbers (like the identity function) and infinitesimals (like 1/x). This gives a rigorous foundation for infinitesimals, vindicating Archimedes, Newton, and Leibniz.
- **Role**: synthesis

## Evidence and caveats

The video demonstrates that the identity function is larger than every real number, and 1/x is a positive infinitesimal. It notes that the hyperreal ordering is not linear until we take equivalence classes. The speaker acknowledges the transitivity axiom is counterintuitive and that the trivial dictator solution exists but is rejected. The proof of existence is shown in Lean code, but the video does not detail the proof itself.

## Concepts surfaced

[[arrow-impossibility-theorem]] · [[infinitesimals]] · [[non-archimedean-ordered-fields]] · [[model-theory]] · [[ultrafilters]]
