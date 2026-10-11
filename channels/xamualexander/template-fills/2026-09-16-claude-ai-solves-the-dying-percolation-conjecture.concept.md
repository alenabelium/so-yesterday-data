---
video_id: D5T9GwgeR8o
template_id: concept
template_version: 1
source_summary: ../summaries/2026-09-16-claude-ai-solves-the-dying-percolation-conjecture.md
source_transcript: ../transcripts/2026-09-16-claude-ai-solves-the-dying-percolation-conjecture.md
source_summary_hash: sha256:75408fe03f4a8272cfb1d9cf45309438b35df133d248ca6005166e22710f08aa
source_transcript_hash: sha256:44d2495429301b209f73ef023e22de7169b5c0d47b56b4d39fc0f3e8b62aac62
fill_id: 62d25158-d47b-4d67-9b57-aa20d6d30aec
published_at: '2026-10-11T18:46:57.003975'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

The Dying Percolation Conjecture, posed in 1982, asks whether percolation at the critical threshold is impossible in all dimensions. An AI system, Claude, autonomously produced a proof, formalized in Lean, that the probability of an infinite cluster at the critical point is zero. This marks a major AI-driven breakthrough in mathematics.

## The argument

### Define the Critical Threshold
- **Anchor Timestamps**: ['00:02:14']
- **Claim**: In Bernoulli bond percolation on a grid, each block is open with probability p. The critical threshold p_c is the value above which an infinite path from top to bottom almost surely exists, and below which it almost surely does not. This threshold exists by standard first-order analysis.
- **Role**: definition

### The Open Question: Behavior Exactly at p_c
- **Anchor Timestamps**: ['00:05:08']
- **Claim**: While the existence of p_c is trivial, the behavior exactly at p_c was unknown for decades. The conjecture asks whether the probability of percolation at p_c is zero for all dimensions d ≥ 2. The simulation shows that slightly below p_c, paths fail as the grid grows, but the exact threshold case remained unresolved.
- **Role**: definition

### AI Proves the Conjecture via Cosma-Nitzan
- **Anchor Timestamps**: ['00:06:23']
- **Claim**: Using an Anthropic Claude model, the conjecture was proven by establishing Cosma's Conjecture 3 and its reduction to critical percolation. This covers all dimensions, including the previously open intermediate dimensions 3 ≤ d ≤ 10. The proof was formalized in Lean, with no human writing the Lean code.
- **Role**: evidence

### Expert Caution: Formalization Might Be Wrong
- **Anchor Timestamps**: ['00:13:37']
- **Claim**: Gil Kalai cautions that while the Lean verification is promising, experts must verify that the formalized statement correctly captures the intended conjecture. A subtle error in formalization could prove a different statement, a risk not unique to AI-generated proofs.
- **Role**: counter

### Meta-Implication: Pace of Discovery
- **Anchor Timestamps**: ['00:16:18']
- **Claim**: The result, only two weeks old, already feels ancient due to the rapid acceleration of AI-driven proofs. This pace risks overlooking significant results, but it also highlights the need to derive deeper understanding from each breakthrough, not just celebrate the proof.
- **Role**: synthesis

## Evidence and caveats

The proof was verified in Lean at commit 795EB8, audited on vibemath.com. The repository's provenance states that Claude models autonomously wrote the Lean code, with human role limited to problem selection and direction. Gil Kalai, an eminent mathematician, calls it a 'remarkable breakthrough' but notes that experts need to see the details and verify the formalization. He also mentions that the Dying Percolation Conjecture is stronger than noise sensitivity, and related open questions remain in 3D. The speaker acknowledges the possibility of Lean bugs but considers accidental exploitation unlikely.

## Concepts surfaced

[[bernolli-bond-percolation]] · [[lean-proof-assistant]] · [[ai-mathematical-proof]] · [[critical-threshold]] · [[cosma-conjecture]]
