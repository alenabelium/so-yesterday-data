---
title: "Hallucination"
slug: "hallucination"
description: "When AI models generate plausible-sounding but factually incorrect or fabricated information."
tags:
  - llm-fundamentals
  - ethics-safety
related:
  - rejection-competency
  - the-70-percent-problem
  - sniff-checking
  - alignment
created: "2026-03-19"
updated: "2026-03-19"
confidence: high
---

Hallucination is the phenomenon where language models generate text that sounds confident and plausible but is factually wrong, internally inconsistent, or entirely fabricated. Models don't "know" they're hallucinating — they produce the most statistically likely next token regardless of truth. This is not a bug that will be fixed; it's a structural property of how LLMs work.

Hallucination is the root cause of several key challenges in the knowledge base. [The 70% problem](/knowledge/the-70-percent-problem) exists partly because hallucinated details hide in otherwise correct output. [Rejection competency](/knowledge/rejection-competency) is fundamentally about catching hallucinations before they propagate. [Sniff-checking](/knowledge/sniff-checking) is rapid hallucination detection at scale. The [Domain Translator](/personas/06-domain-translator) persona's value comes from knowing which domain-specific hallucinations are dangerous — a chatbot hallucinating medical advice differs from hallucinating a recipe.

## Key Aspects

- **Confident incorrectness** — hallucinated content is presented with the same fluency and confidence as correct content, making detection harder
- **Domain-dependent severity** — hallucinations in creative writing are harmless; in medical advice, legal analysis, or code, they can be dangerous
- **Mitigation, not elimination** — techniques like RAG ([Retrieval Augmented Generation](/knowledge/rag)), chain-of-thought reasoning, and grounding reduce hallucination rates but cannot eliminate them
- **Verification burden** — hallucinations shift the burden of verification from the writer to the reader, requiring new skills like [rejection competency](/knowledge/rejection-competency)

## Related Content

- [Stop accepting AI output that "looks right"](/videos/-FhtPUkXKO4) — the danger of undetected hallucinations
- [The AI Failure Mode Nobody Warned You About](/videos/T74uZgfu6mU) — hallucination as a failure mode
- [ChatGPT Health fails critical triage cases](/digests/2026-03-19) — real-world hallucination consequences
- [The Domain Translator](/personas/06-domain-translator) — persona who knows which hallucinations are dangerous in their field
- [The Practitioner](/personas/02-practitioner) — persona building the skill to detect hallucinations
