---
video_id: 07Ee9Z0B-zQ
template_id: concept
template_version: 1
source_summary: ../summaries/2026-08-21-simple-proof-lean-cant-self-verify-itself-no-godels-2nd-inco.md
source_transcript: ../transcripts/2026-08-21-simple-proof-lean-cant-self-verify-itself-no-godels-2nd-inco.md
source_summary_hash: sha256:d57eb871efb9689766bf31d1aa4215078a92a34f075ff8f36719145343cdf6f6
source_transcript_hash: sha256:1d19c29d50486b917ae2e400c23b0d4ccff5a352acf06660cc32e94b60a5748f
fill_id: a4aee63a-119d-44f8-88a6-b0eca0603028
published_at: '2026-10-19T22:46:30.953788'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

Lean cannot verify its own correctness, and a simple proof avoids Gödel's second incompleteness theorem by using computable ordinals—programs that encode levels of infinity. This approach works because Lean can reason about second-order logic, where the barrier is more direct. The proof is arithmetic-free and offers a cleaner explanation for why self-verification fails.

## The argument

### The Naive Fallacy and Its Flaw
- **Anchor Timestamps**: ['00:01:29']
- **Claim**: A first attempt defines 'the largest number definable in under a million characters that Lean verifies, plus one' to force a contradiction. This fails because it requires a truth predicate for Lean, which Tarski's theorem says cannot be formalized inside Lean.
- **Role**: definition

### Computable Ordinals as Programs
- **Anchor Timestamps**: ['00:02:37']
- **Claim**: Computable ordinals are computer programs that denote levels of infinity. Some are verifiable by Lean, others are not. This distinction is key: Lean can recognize some programs as ordinals, but not all, creating a gap to exploit.
- **Role**: definition

### The Function f and Diagonalization
- **Anchor Timestamps**: ['00:03:45']
- **Claim**: There exists a function f such that for any algorithm a enumerating an infinite sequence of computable ordinals, f(a) outputs a computable ordinal greater than all of a's outputs. Lean can verify this property of f, making f a tool for diagonalization.
- **Role**: evidence

### The Contradiction
- **Anchor Timestamps**: ['00:05:03']
- **Claim**: Assume Lean self-verifies and is true. Let A enumerate all ordinals Lean verifies. Since Lean is true, A's outputs are genuine ordinals. Then f(A) is an ordinal greater than all of A's outputs, but Lean can verify f(A) is an ordinal, contradicting A's completeness.
- **Role**: synthesis

### Why Gödel Remains Relevant
- **Anchor Timestamps**: ['00:07:55']
- **Claim**: This proof works because Lean can handle second-order logic. Gödel's second incompleteness theorem applies to first-order systems, which are more general. Thus, Gödel is still necessary for first-order cases, but this simpler method suffices for systems like Lean.
- **Role**: counter

## Evidence and caveats

The speaker demonstrates computable ordinals with Python programs: 0 is an empty program, 1 outputs 0, 2 outputs 1, and so on. Omega is built via an infinite loop that outputs successive finite ordinals. Omega+1, omega+2, and omega*2 are constructed similarly, and the pattern extends to omega*omega and omega^omega, which the speaker notes took two days to code. The proof is published in the Journal of Symbolic Logic (2020) and is arithmetic-free. Caveats: the proof assumes Lean is true; if Lean is false, self-verification is meaningless. The speaker also notes that the naive proof fails due to Tarski's theorem, and that this method does not replace Gödel for first-order systems.

## Concepts surfaced

[[goedel-incompleteness]] · [[lean-theorem-prover]] · [[tarski-undefinability]] · [[second-order-logic]] · [[diagonalization]] · [[ordinal-notation]]
