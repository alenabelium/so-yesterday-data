---
title: "Context Engineering"
slug: "context-engineering"
description: "The art of structuring information provided to LLMs for optimal performance."
tags:
  - prompting
  - llm-fundamentals
related:
  - prompt-engineering
  - specification-quality
  - context-window
  - rag
created: "2026-03-19"
updated: "2026-03-19"
---

Context engineering goes beyond prompt engineering by focusing on the entire information environment presented to a language model — not just the prompt itself, but the system message, retrieved documents, conversation history, and tool definitions.

## Core Principles

- **Relevance** — only include information the model needs for the current task
- **Structure** — organize context with clear headers, delimiters, and hierarchy
- **Recency** — place the most important information near the end of the context window where models attend most strongly

## Relationship to Prompt Engineering

While [prompt engineering](/knowledge/prompt-engineering) focuses on how you ask the question, context engineering focuses on what information surrounds that question. Both are essential for production AI systems. The next evolution connects to [specification quality](/knowledge/specification-quality) — structuring context not just for comprehension but for reliable execution.

For the [Practitioner](/personas/02-practitioner) persona, context assembly is the defining skill gap. Dumping entire documents into an AI is amateur; curating context carefully — selecting what's relevant, structuring it for the model's attention patterns, and maintaining context across interactions — is the skill that separates effective practitioners from those stuck at the [70% problem](/knowledge/the-70-percent-problem).

## Related Content

- [Prompt Engineering Is Dead. Context Engineering Is Dying.](/videos/QWzLPn164w0) — the evolution beyond context engineering
- ['Prompting' Just Split Into 4 Skills](/videos/BpibZSMGtdY) — context engineering as one of the four successor skills
- [The AI Failure Mode Nobody Warned You About](/videos/T74uZgfu6mU) — failure modes from poor context engineering
- [The Orchestrator](/personas/04-orchestrator) — persona whose specs are essentially context engineering artifacts
- [The Practitioner](/personas/02-practitioner) — persona for whom context assembly is the defining skill gap
- [The 70% Problem](/knowledge/the-70-percent-problem) — poor context engineering is a primary cause of the 70% ceiling
