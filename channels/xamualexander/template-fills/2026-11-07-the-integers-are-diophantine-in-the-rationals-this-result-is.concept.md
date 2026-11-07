---
video_id: CxeX6v2Cjlk
template_id: concept
template_version: 1
source_summary: ../summaries/2026-11-07-the-integers-are-diophantine-in-the-rationals-this-result-is.md
source_transcript: ../transcripts/2026-11-07-the-integers-are-diophantine-in-the-rationals-this-result-is.md
source_summary_hash: sha256:5be846c3b61d90c4c8c6b984c4ea8cc7256133d0ba8f7d4619ff0c40f03bffff
source_transcript_hash: sha256:1b768592bf91c10a49deec2fdb789f51e17ded73ae867f867049187da3ff3a96
fill_id: 330a688a-0f79-48f6-bb14-3460c4788974
published_at: '2026-11-07T16:42:54.364475'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

A polynomial with integer coefficients can be built so that its rational zeros project exactly onto the integers. This refutes Mazur's conjecture and completes Hilbert's tenth problem for rationals. The result was announced with 300 billion variables and rapidly improved to a quartic with 962 variables.

## The argument

### Define the Diophantine definition
- **Anchor Timestamps**: ['00:01:04']
- **Claim**: There exists a polynomial with integer coefficients such that a rational number is an integer if and only if it can be substituted into the first variable and other rationals found for the rest to make the polynomial zero.
- **Role**: definition

### The original construction and its scale
- **Anchor Timestamps**: ['00:01:29']
- **Claim**: The initial polynomial had about 300 billion variables, with degree and coefficients bounded by tower notation (2↑↑8). This was the first proof, but it was impractical and served as a starting point.
- **Role**: evidence

### Rapid improvement to a quartic
- **Anchor Timestamps**: ['00:06:03']
- **Claim**: Within hours, the community produced a quartic polynomial with about 5,000 variables and coefficients less than 2^80, then a second quartic with only 962 variables but larger coefficients (64·3^(2^28)). The two are incomparable: one minimizes variables, the other minimizes coefficient size.
- **Role**: evidence

### Refutation of Mazur's conjecture
- **Anchor Timestamps**: ['00:12:08']
- **Claim**: A direct consequence is that Mazur's conjecture is false: the topological closure of rational points on a manifold can have infinitely many connected components. This overturns a long-standing belief in arithmetic geometry.
- **Role**: synthesis

### Verification in Lean is still pending
- **Anchor Timestamps**: ['00:28:08']
- **Claim**: The Lean formalization is not yet complete; it will take weeks. The proof currently relies on some published theorems that are assumed in Lean, not fully verified. This leaves a small but real gap in certainty.
- **Role**: counter

## Evidence and caveats

The result builds on OpenAI's earlier solution to Hilbert's tenth problem for rational numbers, which provided the key elliptic curve strategy. The community rapidly iterated: from 300 billion variables to 5,000 and then 962, with a proof that degree four is minimal. The manuscript itself is confusingly written, mixing the original theorem with later improvements. The Lean verification is ongoing and not yet complete, so the result is not fully machine-checked. The host notes that the proof may be independent of OpenAI's work, which would make it a separate solution to Hilbert's tenth problem for rationals.

## Concepts surfaced

[[hilberts-tenth-problem]] · [[mazurs-conjecture]] · [[diophantine-equations]] · [[lean-proof-assistant]] · [[openai-mathematics-breakthroughs]] · [[dprm-theorem]]
