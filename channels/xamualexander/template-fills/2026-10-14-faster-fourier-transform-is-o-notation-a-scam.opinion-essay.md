---
video_id: C-lYf2OvU8I
template_id: opinion-essay
template_version: 1
source_summary: ../summaries/2026-10-14-faster-fourier-transform-is-o-notation-a-scam.md
source_transcript: ../transcripts/2026-10-14-faster-fourier-transform-is-o-notation-a-scam.md
source_summary_hash: sha256:28cdf2bb4b7f7c6d1e62e3b0b770c67356bab1645de81021f510f97d34127363
source_transcript_hash: sha256:9b44c8d13f497e5b72948a0e6b0efa432d4e6ae5a152029efcb70572cdbcd916
fill_id: 6142ebf5-cbe0-4a3c-8569-343fd7651268
published_at: '2026-10-19T17:25:53.996505'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## Thesis

OpenAI's faster Fourier transform is a mathematically valid but practically useless 'galactic algorithm,' exposing how big O notation and theoretical computer science culture have become disconnected from real-world computing.

## Argument

The mechanism is the abuse of big O notation. An algorithm can be asymptotically faster yet utterly impractical because big O ignores constants and only cares about behavior as n approaches infinity. OpenAI's algorithm runs in O(n^(1 - 10^-13) log n), which is technically faster than Cooley-Tukey's O(n log n), but the hidden constant is astronomically large—around 10^100—so it only beats Cooley-Tukey when n exceeds a googolplex. For any realistic input, Cooley-Tukey is vastly faster. The algorithm also relies on an unrealistic computational model: exact complex arithmetic with unbounded coefficients, requiring memory exponential in input length. This is not a real breakthrough but an artifact of poorly formalized requirements, as Morgenstern and Ailon showed that faster Fourier transforms are impossible under more realistic constraints. The deeper issue is a cultural rot in theoretical computer science that rewards such impractical results, discourages running algorithms, and has become disconnected from actual computers. AI is automating these worst tendencies, producing useless theoretical papers that nonetheless follow the rules of the mathematical game.

## Counterpoints

- Some argue the result is a genuine mathematical breakthrough, not just a practical oddity.
- Galactic algorithms can stimulate research that eventually leads to practical algorithms.
- Big O notation is like Einstein's relativity: useless for everyday tasks but reveals true nature at extremes.
- The algorithm is correct if verified in Lean, so it's mathematically valid even if impractical.

## Concepts surfaced

[[big-o-notation]] · [[galactic-algorithms]] · [[fast-fourier-transform]] · [[theoretical-computer-science]] · [[ai-research]]
