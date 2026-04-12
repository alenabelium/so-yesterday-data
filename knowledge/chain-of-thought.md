---
title: "Chain of Thought"
slug: "chain-of-thought"
description: "A reasoning technique where LLMs break problems into intermediate steps before answering."
tags:
  - prompting
  - llm-fundamentals
related:
  - prompt-engineering
  - context-engineering
  - inference
created: "2026-03-19"
updated: "2026-03-19"
confidence: high
---

Chain-of-thought (CoT) prompting is a technique that encourages language models to generate intermediate reasoning steps before arriving at a final answer. First described by Wei et al. (2022), it has become one of the most impactful techniques for improving LLM performance on complex tasks.

## How It Works

Instead of asking for a direct answer, you instruct the model to "think step by step" or provide examples that demonstrate the reasoning process. This activates the model's ability to decompose problems.

## Variants

- **Zero-shot CoT** — simply append "Let's think step by step" to any prompt
- **Few-shot CoT** — provide examples with explicit reasoning chains
- **Self-consistency** — generate multiple CoT paths and take the majority answer

## When It Helps

Chain-of-thought is most effective for math, logic, multi-step reasoning, and code generation. For simple factual recall, it adds unnecessary overhead.

## Related Content

- [Prompt Engineering](/knowledge/prompt-engineering) covers the broader landscape of prompting techniques
- [Why Andrej Karpathy Feels "Behind"](/videos/fyHnGHxGuhI) — chain-of-thought reasoning in practice
- [Claude Opus 4.6: The Biggest AI Jump](/videos/JKk77rzOL34) — model advances in reasoning capabilities
- [Codex 5.3 vs Opus 4.6](/videos/41UDGsBEjoI) — comparing reasoning approaches across models
