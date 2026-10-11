---
video_id: D5T9GwgeR8o
template_id: concept
template_version: 1
source_summary: ../summaries/2026-09-16-claude-ai-solves-the-dying-percolation-conjecture.md
source_transcript: ../transcripts/2026-09-16-claude-ai-solves-the-dying-percolation-conjecture.md
source_summary_hash: sha256:75408fe03f4a8272cfb1d9cf45309438b35df133d248ca6005166e22710f08aa
source_transcript_hash: sha256:44d2495429301b209f73ef023e22de7169b5c0d47b56b4d39fc0f3e8b62aac62
fill_id: d12844df-cdc6-4080-919d-93477fac9dd5
published_at: '2026-10-11T17:46:32.949841'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

The Dying Percolation Conjecture, posed in 1982, asks whether percolation is impossible exactly at the critical threshold. An AI system, Claude, autonomously produced a proof, formalized and verified in Lean, settling the conjecture for all dimensions. This marks a major milestone in AI-driven mathematics.

## The argument

### Define the Critical Threshold
- **Anchor Timestamps**: ['00:02:14']
- **Claim**: In Bernoulli bond percolation, each bond is open with probability p. The critical threshold p_c is the supremum of p where no infinite cluster exists. Below p_c, no path spans the grid; above, it does. The threshold's existence is trivial, but behavior exactly at p_c was unknown.
- **Role**: definition

### Simulate the Critical Case
- **Anchor Timestamps**: ['00:03:20']
- **Claim**: Simulations show that below p_c, paths fail; above, they succeed. At p_c, small grids may connect, but as the grid grows, connections become blocked. This illustrates the conjecture's claim: at the critical point, percolation probability is zero.
- **Role**: evidence

### AI Proof and Lean Verification
- **Anchor Timestamps**: ['00:07:25']
- **Claim**: Claude, an Anthropic AI, autonomously produced the informal proof and Lean formalization. The Lean proof checker verified the formal statement, ensuring logical correctness. The repository's provenance section confirms no human wrote the Lean code.
- **Role**: evidence

### Expert Skepticism on Formalization
- **Anchor Timestamps**: ['00:13:37']
- **Claim**: Gil Kalai cautions that the formalization might not correctly capture the intended conjecture. A subtle error in stating the problem could lead to a proof of the wrong theorem. This mirrors human mathematics, where claims are often reported before full community vetting.
- **Role**: counter

### Synthesis: A New Era of Mathematical Discovery
- **Anchor Timestamps**: ['00:16:18']
- **Claim**: The pace of AI-driven proofs is so rapid that a two-week-old result feels ancient. Yet, we must still study these results to extract understanding. The Dying Percolation Conjecture's solution exemplifies how AI can tackle long-standing problems, but verification and human insight remain essential.
- **Role**: synthesis

## Evidence and caveats

The proof builds on a conjecture by Gady Kozma and Shahaf Nitzan, which reduces the Dying Percolation Conjecture to a more general statement. This reduction was previously known for planar and high-dimensional cases, but the intermediate dimensions (3–10) were open. The AI's proof covers all dimensions. 

Caveats: The formalization's correctness is not yet fully vetted by the mathematical community. Gil Kalai notes that the written proof lacks details for experts to digest, and the Lean verification, while promising, could contain subtle errors in the statement's encoding. Additionally, the AI model used was not specified, and the result does not address site percolation or other lattices.

## Concepts surfaced

[[lean-proof-assistant]] · [[ai-mathematical-discovery]] · [[critical-phenomena]] · [[bernoulli-percolation]] · [[formal-verification]]
