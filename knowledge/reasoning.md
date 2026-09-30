---
title: "Reasoning (LLM)"
slug: "reasoning"
description: "Deliberate multi-step computation in models — the capability tier behind test-time scaling and 'thinking' models."
tags:
  - llm-fundamentals
related:
  - chain-of-thought
  - llm
  - benchmarks
provenance: agent:stub-authoring-v1
created: "2026-05-19"
updated: "2026-09-30"
confidence: medium
---

LLM reasoning is the deliberate mode: models that spend inference-time compute on intermediate steps — [chain of thought](/knowledge/chain-of-thought), self-checking, tool-mediated scratch work — rather than answering directly. The corpus tracks it as the capability tier that unlocked agentic work: planning, decomposition and recovery-from-error all reduce to sustained reasoning over context.

The production economics it created: reasoning tokens cost latency and money, which is precisely why routing architectures split "system 1" snap judgments from "system 2" deliberate passes (see [LLM](/knowledge/llm), [model efficiency](/knowledge/model-efficiency)). The measured caveats: reasoning degrades under context clutter (hence [context window management](/knowledge/context-window-management)), and benchmark gains don't always transfer — task-specific evals remain the arbiter (see [benchmarking](/knowledge/benchmarking)).
