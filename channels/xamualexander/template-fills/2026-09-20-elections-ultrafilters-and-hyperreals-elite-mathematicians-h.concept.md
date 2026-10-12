---
video_id: VBwO5A546F8
template_id: concept
template_version: 1
source_summary: ../summaries/2026-09-20-elections-ultrafilters-and-hyperreals-elite-mathematicians-h.md
source_transcript: ../transcripts/2026-09-20-elections-ultrafilters-and-hyperreals-elite-mathematicians-h.md
source_summary_hash: sha256:6f518437b6ae03ca618c7563b4ce28b581230376baa929562b8edd38e5771bdb
source_transcript_hash: sha256:a14fc0319cfe1466bbc5704906c1a4f1c59c1a9d0d080e91b14770fc89a99de4
fill_id: b37d67fd-5a1a-40bc-b0b2-702553d3bd9c
published_at: '2026-10-12T04:42:22.600463'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

Numbers can vote on comparisons between functions, and with infinitely many voters, we can design majority rules that avoid a dictator. This leads to free ultrafilters and hyperreal numbers, which include infinitesimals and infinities. The trick: infinite voters escape Arrow's impossibility theorem.

## The argument

### Define the Voting Framework
- **Anchor Timestamps**: ['00:00:00']
- **Claim**: Each natural number votes on whether f(n) > g(n), f(n) < g(n), or f(n) = g(n). Tallying these votes decides which function is bigger on average, even for functions like sine and cosine that are translates of each other.
- **Role**: definition

### Impose Majority Axioms
- **Anchor Timestamps**: ['00:05:01']
- **Claim**: To ensure coherent decisions, majorities must satisfy non-triviality, monotonicity, non-ambiguity, and transitivity. Transitivity forces the intersection of any two majorities to be a majority, a counterintuitive requirement that becomes possible with infinite voters.
- **Role**: definition

### Reject the Dictator Solution
- **Anchor Timestamps**: ['00:07:49']
- **Claim**: A trivial solution is to let one number be a dictator, but we rule that out by requiring no singleton is a majority. Surprisingly, these five axioms are still mutually satisfiable, leading to the existence of a free ultrafilter on any infinite voter set.
- **Role**: counter

### Escape Arrow's Impossibility
- **Anchor Timestamps**: ['00:10:26']
- **Claim**: Arrow's theorem says finite elections with those four axioms must have a dictator. But with infinitely many voters, the theorem fails, so we can have non-dictatorial majorities. This is the key that unlocks the construction.
- **Role**: synthesis

### Construct Hyperreal Numbers
- **Anchor Timestamps**: ['00:12:51']
- **Claim**: By taking equivalence classes of functions under the majority relation, we get hyperreal numbers. These include the reals as constant functions, plus infinite numbers like the identity function and infinitesimals like 1/x, which are bigger than zero yet smaller than every positive real.
- **Role**: evidence

## Evidence and caveats

The video demonstrates that the identity function is infinite because infinitely many naturals vote it larger than any real R, while only finitely many vote otherwise. Similarly, 1/x is infinitesimal because infinitely many naturals vote it smaller than any positive real. The speaker notes that defining 1/x at zero is irrelevant since one voter doesn't matter. He also acknowledges that the equivalence relation is not a linear order until we 'squint' and take equivalence classes. The historical controversy: Archimedes, Newton, and Leibniz accepted infinitesimals, but later mathematicians rejected them until Abraham Robinson's 1961 discovery of hyperreals.

## Concepts surfaced

[[free-ultrafilters]] · [[hyperreal-numbers]] · [[arrows-impossibility-theorem]] · [[infinitesimals]] · [[non-archimedean-ordered-fields]]
