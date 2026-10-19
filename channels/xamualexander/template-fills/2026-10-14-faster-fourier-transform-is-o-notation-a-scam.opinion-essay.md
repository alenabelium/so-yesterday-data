---
video_id: C-lYf2OvU8I
template_id: opinion-essay
template_version: 1
source_summary: ../summaries/2026-10-14-faster-fourier-transform-is-o-notation-a-scam.md
source_transcript: ../transcripts/2026-10-14-faster-fourier-transform-is-o-notation-a-scam.md
source_summary_hash: sha256:28cdf2bb4b7f7c6d1e62e3b0b770c67356bab1645de81021f510f97d34127363
source_transcript_hash: sha256:9b44c8d13f497e5b72948a0e6b0efa432d4e6ae5a152029efcb70572cdbcd916
fill_id: a78e8568-99eb-4876-9208-bf03a6689346
published_at: '2026-10-19T17:05:30.402645'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## Thesis

OpenAI's faster Fourier transform is a mathematically valid but practically useless 'galactic algorithm' that exposes how big O notation can be abused, yet the notation remains indispensable because no simpler alternative exists.

## Argument

The mechanism is the abuse of big O notation. An algorithm can be asymptotically faster while being absurdly slower for any realistic input. OpenAI's algorithm runs in O(n^(1 - 10^-13) log n), which is technically better than Cooley-Tukey's O(n log n), but the hidden constant is around 10^100, and it only wins for n greater than a googolplex. This is a textbook 'galactic algorithm,' a term coined by Lipton and Regan. The algorithm's computational model is also unrealistic: it assumes exact complex arithmetic with unbounded precision, requiring memory exponential in the input length. This is not a practical breakthrough; it's an artifact of how computer scientists formalize problems. Morgenstern (1973) and Ailon (2013) showed that faster FFTs are impossible under more realistic constraints, so OpenAI's result exploits a loophole in the model. The deeper issue is a cultural one: theoretical computer science rewards asymptotic improvements regardless of practicality, and AI is now automating that tendency, producing papers that are mathematically correct but disconnected from real computers. Yet, big O notation is not a scam. It's like Einstein's relativity: useless for building bridges but essential for understanding the universe at extreme scales. Similarly, big O tells us what happens as n approaches infinity, which is irrelevant for everyday computations but fundamental to the theory. The challenge is that replacing big O with something simpler is impossible, as my Socratic dialogue shows: any attempt to map complexity classes to real numbers leads to arbitrary choices

## Counterpoints

- The result is a mathematical breakthrough, not just an oddity of bad formalization.
- Galactic algorithms can stimulate research that eventually leads to practical algorithms.
- Big O notation is impractical and should be replaced with something simpler.
- The algorithm's computational model is unrealistic, so the result is irrelevant to real computing.

## Concepts surfaced

[[galactic-algorithms]] · [[big-o-notation]] · [[fast-fourier-transform]] · [[theoretical-computer-science]] · [[ai-mathematical-discovery]]
