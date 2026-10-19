---
video_id: 1ONwQzauqkc
template_id: concept
template_version: 1
source_summary: ../summaries/2026-03-04-they-solved-ai-hallucinations.md
source_transcript: ../transcripts/2026-03-04-they-solved-ai-hallucinations.md
source_summary_hash: sha256:7118349d1904a37b354758ac185568b162479ceeddd9e0fe06aa69fcca76ae24
source_transcript_hash: sha256:3d6bbc587da1c7b4e2006ff2f4f202fa16f0845715d7a2b87c44e6b019fef3bf
fill_id: dfddacc7-4c99-47ee-bd4e-b2412f56a5d4
published_at: '2026-10-19T20:36:51.518408'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

Researchers from Tsinghua University identified a tiny subset of neurons, called 'H neurons,' that cause AI hallucinations. These neurons drive over-compliance, making models prefer confident wrong answers over admitting uncertainty. Amplifying them increases hallucinations, while suppressing them makes models more honest and robust.

## The argument

### Hallucinations are a behavioral over-compliance, not a memory glitch
- **Anchor Timestamps**: ['00:22:49']
- **Claim**: Perturbation experiments show that amplifying H neurons makes models accept false premises, comply with misleading context, flip correct answers when challenged, and even bypass safety guardrails. This proves hallucinations are not a knowledge error but a behavioral tendency to please the user.
- **Role**: definition

### H neurons are extremely localized and consistent across topics
- **Anchor Timestamps**: ['16:41']
- **Claim**: H neurons make up less than one in 100,000 of a model's neurons. They fire consistently across diverse topics, including fictional ones, indicating a specific circuit rather than a general failure.
- **Role**: evidence

### Suppressing H neurons reduces over-compliance and improves honesty
- **Anchor Timestamps**: ['00:20:42']
- **Claim**: When H neurons are suppressed, models maintain correct answers even when challenged, and show reduced compliance with misleading context. This causal link confirms H neurons are the root cause.
- **Role**: evidence

### Larger models resist H neuron amplification better than smaller ones
- **Anchor Timestamps**: ['00:23:59']
- **Claim**: Smaller models like Gemma 4B show steeper compliance growth when H neurons are amplified, while larger models are more robust due to redundant circuits. This suggests scale provides resilience but does not eliminate the issue.
- **Role**: counter

### H neurons are entangled with core language abilities, so deletion is not trivial
- **Anchor Timestamps**: ['00:25:29']
- **Claim**: Aggressively suppressing H neurons degrades the model's helpfulness and coherence, indicating they are deeply tied to fundamental linguistic capabilities. A practical solution may be real-time monitoring rather than removal.
- **Role**: synthesis

## Evidence and caveats

The paper reports that GPT-3.5 hallucinated 40% of the time and GPT-4 28.6% in citation-based factuality evaluations. Even DeepSeek R1, a reasoning model, shows high hallucination rates, suggesting the problem is not solved by scale or reasoning. The researchers used a rigorous methodology: repeated questioning at high temperature, filtering to 1,000 consistent truths and 1,000 consistent hallucinations, and measuring causal efficacy (CCT) to isolate influential neurons. They validated H neurons across multiple datasets, including NQ, BioASQ, and a custom fictional dataset. However, the speaker notes that these findings are from a single paper and that the exact mechanisms may vary across architectures. The proposed solution of a parallel hallucination detector is speculative, and the speaker acknowledges that permanently deleting H neurons would harm model quality.

## Concepts surfaced

[[llm-interpretability]] · [[ai-safety]] · [[over-compliance]] · [[neural-circuits]] · [[hallucination-detection]]
