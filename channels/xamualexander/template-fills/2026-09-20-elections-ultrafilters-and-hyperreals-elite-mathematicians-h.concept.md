---
video_id: VBwO5A546F8
template_id: concept
template_version: 1
source_summary: ../summaries/2026-09-20-elections-ultrafilters-and-hyperreals-elite-mathematicians-h.md
source_transcript: ../transcripts/2026-09-20-elections-ultrafilters-and-hyperreals-elite-mathematicians-h.md
source_summary_hash: sha256:6f518437b6ae03ca618c7563b4ce28b581230376baa929562b8edd38e5771bdb
source_transcript_hash: sha256:a14fc0319cfe1466bbc5704906c1a4f1c59c1a9d0d080e91b14770fc89a99de4
fill_id: 66d7c6f4-75c0-478f-80a2-ccee8f0ca213
published_at: '2026-10-11T18:46:48.973747'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

A voter-based analogy where natural numbers vote on function comparisons leads to the axioms of majority decisions. With infinitely many voters, these axioms can be satisfied without a dictator, yielding free ultrafilters and hyperreal numbers that include infinitesimals and infinities. This intuitive route bypasses Arrow's impossibility theorem and revives the historical infinitesimals.

## The argument

### Define the Voting Setup
- **Anchor Timestamps**: ['00:00:00']
- **Claim**: Numbers vote on comparisons between functions: each natural number n votes based on whether f(n) is greater, less, or equal to g(n). Tallying these votes yields a notion of which function is bigger on average, even for functions like sine and cosine that are translates of each other.
- **Role**: definition

### Axioms for Majorities
- **Anchor Timestamps**: ['00:03:36']
- **Claim**: Majorities must satisfy four axioms: non-triviality (empty set is not a majority), monotonicity (supersets of majorities are majorities), unambiguity (either a set or its complement is a majority), and transitivity (intersection of two majorities is a majority). The transitivity axiom is counterintuitive but necessary for coherent comparisons.
- **Role**: definition

### Escape Arrow's Theorem
- **Anchor Timestamps**: ['00:10:26']
- **Claim**: With finitely many voters, the first four axioms force a dictator, as Arrow's impossibility theorem shows. But with infinitely many voters, the axioms are satisfiable without a dictator, because the theorem fails for infinite voter sets. This allows a decision method that avoids dictatorship.
- **Role**: counter

### Construct Hyperreals
- **Anchor Timestamps**: ['00:12:51']
- **Claim**: By taking equivalence classes of functions under majority agreement, we obtain hyperreal numbers. These include the ordinary reals as constant functions, plus infinite numbers like the identity function and infinitesimals like 1/x, which are larger or smaller than every real respectively.
- **Role**: synthesis

## Evidence and caveats

The video demonstrates that the identity function represents an infinite hyperreal, as a majority of naturals vote it larger than any fixed real. Similarly, 1/x represents a positive infinitesimal, since a majority of naturals vote it smaller than any positive real. The speaker notes that the trivial dictator solution satisfies the first four axioms, but is ruled out by the fifth requirement. He also mentions that the equivalence classes are not a linear order until we 'squint' and blur non-equal functions that are equivalent. The proof of existence of free ultrafilters is shown in Lean code from mathlib, but the speaker does not detail the proof.

## Concepts surfaced

[[free-ultrafilters]] · [[hyperreal-numbers]] · [[arrows-impossibility-theorem]] · [[infinitesimals]] · [[non-archimedean-fields]]
