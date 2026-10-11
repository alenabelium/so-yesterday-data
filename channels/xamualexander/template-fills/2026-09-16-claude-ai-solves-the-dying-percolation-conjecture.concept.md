---
video_id: D5T9GwgeR8o
template_id: concept
template_version: 1
source_summary: ../summaries/2026-09-16-claude-ai-solves-the-dying-percolation-conjecture.md
source_transcript: ../transcripts/2026-09-16-claude-ai-solves-the-dying-percolation-conjecture.md
source_summary_hash: sha256:75408fe03f4a8272cfb1d9cf45309438b35df133d248ca6005166e22710f08aa
source_transcript_hash: sha256:44d2495429301b209f73ef023e22de7169b5c0d47b56b4d39fc0f3e8b62aac62
fill_id: cccc1841-4a5b-49ee-85dd-c5bd1d955f77
published_at: '2026-10-11T15:56:16.195687'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

The Dying Percolation Conjecture, posed in 1982, asks whether percolation at the critical threshold is impossible in all dimensions. An AI system, Anthropic's Claude, autonomously produced a proof, formalized and verified in Lean, settling the conjecture. This marks a milestone in AI-driven mathematical discovery, though experts urge careful verification of the formalization.

## The argument

### Define the Critical Threshold and the Conjecture
- **Anchor Timestamps**: ['00:02:14']
- **Claim**: In Bernoulli bond percolation on the integer lattice, each edge is open with probability p. The critical threshold p_c is the supremum of p where no infinite cluster exists. The Dying Percolation Conjecture asks whether the probability of an infinite cluster at p_c is zero for all dimensions d ≥ 2.
- **Role**: definition

### Simulate the Critical Behavior
- **Anchor Timestamps**: ['00:05:08']
- **Claim**: A grid simulation shows that below p_c, paths from top to bottom fail as the grid grows; above p_c, they succeed. At exactly p_c, the outcome is ambiguous in finite grids, but the conjecture asserts that in the infinite limit, no infinite cluster exists. This intuition is trivial for p < p_c and p > p_c, but the critical point itself was open.
- **Role**: evidence

### AI Proof and Lean Verification
- **Anchor Timestamps**: ['00:07:25']
- **Claim**: Anthropic's Claude, working autonomously under Justin Ladder's direction, produced the proof, formalized in Lean. The repository's provenance section states no human wrote or edited the Lean code. The formalization covers dimensions 3 ≤ d ≤ 10 via a reduction to a conjecture by Cosma and Nitsan, and the proof is verified in Lean at a specific commit.
- **Role**: evidence

### Expert Endorsement and Remaining Doubts
- **Anchor Timestamps**: ['00:09:24']
- **Claim**: Gil Kalai, a prominent mathematician, calls the result a remarkable breakthrough if verified. He notes that the proof is not yet an official Claude document and that experts need to see the details. The main risk is that the formalization might accidentally encode a different conjecture, a subtle but real concern.
- **Role**: counter

### Synthesis: The Pace of AI Discovery
- **Anchor Timestamps**: ['00:16:18']
- **Claim**: The result, though only two weeks old, already feels ancient due to the rapid acceleration of AI-driven proofs. This pace creates a risk of overlooking important results. The Dying Percolation Conjecture's solution exemplifies both the power of AI in mathematics and the need for careful human oversight.
- **Role**: synthesis

## Evidence and caveats

The simulation demonstrates the critical threshold: below p_c (e.g., 50%) paths fail, above p_c (e.g., 70%) they succeed, and near p_c (59.273 vs 59.28) the behavior matches the conjecture. The proof is verified in Lean, but Gil Kalai cautions that the formalization might be incorrect, possibly encoding a different conjecture. He also notes that the proof details are not yet fully provided for expert digestion. The result is stronger than noise sensitivity, as Cosma reminded Kalai. The video also mentions that the AI's theorem on the 2/3 of the zeta zeros was improved by a human, showing that human refinement remains relevant.

## Concepts surfaced

[[lean-proof-assistant]] · [[ai-mathematical-discovery]] · [[bernoulli-bond-percolation]] · [[critical-threshold]] · [[formal-verification]] · [[open-problems-in-mathematics]]
