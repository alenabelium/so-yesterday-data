---
video_id: VBwO5A546F8
template_id: concept
template_version: 1
source_summary: ../summaries/2026-09-20-elections-ultrafilters-and-hyperreals-elite-mathematicians-h.md
source_transcript: ../transcripts/2026-09-20-elections-ultrafilters-and-hyperreals-elite-mathematicians-h.md
source_summary_hash: sha256:6f518437b6ae03ca618c7563b4ce28b581230376baa929562b8edd38e5771bdb
source_transcript_hash: sha256:a14fc0319cfe1466bbc5704906c1a4f1c59c1a9d0d080e91b14770fc89a99de4
fill_id: 2543bb53-a277-4dd5-b525-726689613c3b
published_at: '2026-10-12T07:42:05.703006'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

Numbers voting on comparisons between functions leads to a surprising mathematical structure: free ultrafilters. These ultrafilters allow us to define a coherent notion of 'bigger on average' for arbitrary functions, even with infinitely many voters. This construction yields the hyperreal numbers, a number system containing infinitesimals and infinities, which has a controversial history and profound implications for calculus.

## The argument

### Define the voter-based comparison
- **Anchor Timestamps**: ['00:00:00']
- **Claim**: To compare functions 'on average', let each natural number n vote on whether f(n) > g(n), f(n) < g(n), or f(n) = g(n). The winning candidate, determined by a majority of voters, defines the average comparison. This works even for functions like sine and cosine, which are translates of each other.
- **Role**: definition

### Axioms for majorities
- **Anchor Timestamps**: ['00:03:36']
- **Claim**: For a set of voters to be a 'majority', it must satisfy three intuitive axioms: non-triviality (empty set is not a majority), monotonicity (supersets of majorities are majorities), and unambiguity (for any set, either it or its complement is a majority). A fourth, less intuitive axiom—closure under intersection—is needed to ensure transitivity of the average comparison.
- **Role**: definition

### Escape Arrow's impossibility
- **Anchor Timestamps**: ['00:10:26']
- **Claim**: With finitely many voters, satisfying the first four axioms forces a dictator, as Arrow's impossibility theorem states. However, with infinitely many voters (the naturals), we can satisfy all five axioms, including no dictator. This is equivalent to the existence of a free ultrafilter on the naturals.
- **Role**: evidence

### Construct hyperreals via equivalence classes
- **Anchor Timestamps**: ['00:12:51']
- **Claim**: By blurring together functions that are equivalent on a majority of inputs, we obtain equivalence classes called hyperreal numbers. These hyperreals extend the real numbers and include infinite and infinitesimal elements, such as the class of the identity function (infinite) and the class of 1/x (infinitesimal).
- **Role**: synthesis

## Evidence and caveats

The video demonstrates that the identity function is larger than every real number, and 1/x is smaller than every positive real but still positive, illustrating the existence of infinities and infinitesimals. It also notes that the construction yields a non-linear ordering because non-equal functions can be equivalent, but this is resolved by taking equivalence classes. The speaker acknowledges that the transitivity axiom is counterintuitive and that the trivial dictatorial solution is 'stupid', but it is ruled out by the fifth axiom. The video also mentions that Arrow's impossibility theorem does not apply because it assumes finitely many voters, whereas here there are infinitely many.

## Concepts surfaced

[[arrow-impossibility-theorem]] · [[infinitesimals]] · [[nonstandard-analysis]] · [[ultrafilters]]
