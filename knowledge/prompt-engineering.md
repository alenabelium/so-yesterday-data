---
title: "Prompt Engineering"
slug: "prompt-engineering"
description: "Techniques for crafting effective prompts to get better results from LLMs."
tags:
  - prompting
  - ai-tools
related:
  - context-engineering
  - chain-of-thought
  - context-window
created: "2026-03-19"
updated: "2026-03-19"
---

Prompt engineering is the practice of designing inputs to large language models to elicit more accurate, useful, and relevant outputs. As LLMs have become central to AI workflows, prompt engineering has emerged as a critical skill for both developers and end users. However, as models become more capable, the emphasis is shifting. The progression from prompt engineering through [context engineering](/knowledge/context-engineering) to [intent engineering](/knowledge/intent-engineering) reflects a move up the abstraction ladder — from crafting specific inputs to structuring information environments to expressing high-level goals. The [Practitioner](/personas/02-practitioner) persona develops prompting skill as their entry point, but the most effective practitioners quickly discover that clarity of thought matters more than prompt tricks.

## Key Techniques

- **Zero-shot prompting** — asking the model directly without providing examples. Works well for straightforward tasks.
- **Few-shot prompting** — providing examples in the prompt to guide the model's output format and reasoning ([Context Engineering](/knowledge/context-engineering)).
- **Chain-of-thought** — asking the model to reason step by step before answering ([Chain of Thought](/knowledge/chain-of-thought)).
- **System prompts** — setting behavioral instructions that persist across a conversation.

## When to Use What

For simple factual queries, zero-shot is usually sufficient. For complex reasoning tasks, chain-of-thought prompting consistently improves accuracy. Few-shot prompting shines when you need a specific output format.

## Related Content

- [90% of AI Users Are Getting Mediocre Output](/videos/KX0GurmgAoo) — why most people need better prompting skills
- ['Prompting' Just Split Into 4 Skills](/videos/BpibZSMGtdY) — the evolution from prompting to four distinct disciplines
- [Prompt Engineering Is Dead. Context Engineering Is Dying.](/videos/QWzLPn164w0) — what comes after prompt engineering
- [The Practitioner](/personas/02-practitioner) — persona refining prompting skills through daily AI use
- [Intent Engineering](/knowledge/intent-engineering) — the next evolution beyond prompt and context engineering
