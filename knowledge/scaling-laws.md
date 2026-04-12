---
title: "Scaling Laws"
slug: "scaling-laws"
description: "The empirical finding that AI model performance improves predictably with more compute, data, and parameters."
tags:
  - llm-fundamentals
  - ai-strategy
related:
  - frontier-labs
  - ai-infrastructure
  - inference
  - emergent-behavior
  - agi
created: "2026-03-19"
updated: "2026-03-19"
confidence: high
---

Scaling laws are the empirical observation that language model performance improves in predictable, measurable ways as you increase three inputs: compute (processing power), data (training examples), and parameters (model size). First rigorously documented by researchers at OpenAI in 2020, scaling laws have become the strategic foundation for [frontier labs](/knowledge/frontier-labs) — the reason they invest billions in [infrastructure](/knowledge/ai-infrastructure) and compete for GPU supply.

Scaling laws matter because they make AI progress partially predictable. If you know how a model performs at current scale, you can estimate how a 10x larger model will perform. This predictability drives the massive infrastructure investments documented in the repo — Amazon's $125B AI spend, Google's $175-185B capex, Goldman Sachs projecting $1.15T in hyperscaler spending. It also fuels [AGI](/knowledge/agi) timeline predictions: if capabilities keep scaling, when do they reach human level?

The open question is whether scaling alone is sufficient for continued improvement, or whether new architectures and techniques are needed. The appearance of [emergent behaviors](/knowledge/emergent-behavior) at scale — capabilities that weren't predicted by extrapolating from smaller models — suggests that scaling produces qualitative surprises, not just quantitative improvement.

## Key Aspects

- **Power law relationship** — performance improves as a power law of compute, meaning each doubling of compute produces a consistent (but diminishing) improvement
- **Chinchilla scaling** — optimal performance comes from balancing model size and training data, not just making models bigger
- **Inference-time scaling** — newer discovery: performance also improves by spending more compute at [inference](/knowledge/inference) time (thinking longer)
- **Diminishing returns debate** — critics argue scaling is hitting a wall; proponents point to inference-time scaling and architectural innovations as new scaling frontiers

## Related Content

- [NVIDIA told us exactly where AI is going](/videos/5Kp-Gj5qXL0) — the infrastructure roadmap built on scaling assumptions
- [Why $650 Billion in AI Spending ISN'T Enough](/videos/NCgdpbEvNVA) — investment driven by scaling laws
- [Claude Opus 4.6: The Biggest AI Jump](/videos/JKk77rzOL34) — a scaling breakthrough in practice
- [72 Days That Rewrote the Rules](/essays/2026-03-13-03-72-days-that-rewrote-the-rules) — infrastructure investment driven by scaling expectations
