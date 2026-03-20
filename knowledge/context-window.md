---
title: "Context Window"
slug: "context-window"
description: "The maximum amount of text (measured in tokens) that a language model can process in a single interaction."
tags:
  - llm-fundamentals
  - ai-tools
related:
  - context-engineering
  - token-economics
  - agent-orchestration
  - inference
created: "2026-03-19"
updated: "2026-03-19"
---

The context window is the maximum amount of text — measured in [tokens](/knowledge/token-economics) — that a language model can receive as input and generate as output in a single interaction. It determines how much information the model can "see" at once: a larger context window means the model can process longer documents, maintain longer conversations, and work with more complex codebases.

Context window size is one of the most practically important model characteristics. Claude Opus 4.6's expansion to 1 million tokens (roughly 750,000 words) was a landmark — enabling agents to comprehend entire codebases, process full legal documents, or maintain coherent multi-day work sessions. However, larger context windows come with higher [inference](/knowledge/inference) costs and attention degradation: models perform worse on information buried in the middle of very long contexts.

The [Orchestrator](/personas/04-orchestrator) persona experiences context window limits as "context window fragility" — around message 30 in a conversation, agents start ignoring earlier instructions. This drives practices like scaffold documents, rules files, and fresh starts. Effective [context engineering](/knowledge/context-engineering) is largely the art of working within and around context window constraints.

## Key Aspects

- **Size progression** — context windows have grown from 4K tokens (early GPT-3) to 1M tokens (Claude Opus 4.6), roughly a 250x increase
- **Attention patterns** — models attend most strongly to the beginning and end of the context; information in the middle is more likely to be missed ("lost in the middle" problem)
- **Cost scaling** — larger context windows mean more [tokens](/knowledge/token-economics) processed per interaction, directly increasing cost
- **Practical limits vs. theoretical limits** — a model may accept 1M tokens but perform best with focused, well-structured context of 10-50K tokens

## Related Content

- [Claude Opus 4.6: The Biggest AI Jump](/videos/JKk77rzOL34) — 1M token context window and its implications
- [Codex 5.3 vs Opus 4.6](/videos/41UDGsBEjoI) — comparing context handling across models
- [The Orchestrator](/personas/04-orchestrator) — persona managing context window fragility daily
