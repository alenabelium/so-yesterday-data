---
title: "Token"
slug: "token"
description: "The fundamental unit of text processed by LLMs, determining context limits and inference costs."
tags:
  - llm-fundamentals
  - ai-strategy
  - productivity
related:
  - context-window
  - inference
  - prompt-engineering
  - token-economics
confidence: medium
created: "2026-04-27"
updated: "2026-04-27"
---

In the context of Large Language Models (LLMs), a token is the smallest unit of text that the model processes, generates, and charges for. Unlike human words, tokens are not strictly one-to-one with words; they represent sub-word units, characters, or whitespace. For example, the word "transformer" might be split into two tokens ("trans" and "former"), while a common word like "the" is often a single token. This segmentation is handled by a tokenizer, a critical component of the model's architecture that converts raw text into numerical IDs the neural network can understand.

Understanding tokens is essential for managing both the technical constraints and the economic costs of AI transformation. The total number of tokens in a conversation defines the "context window" limit, determining how much information the model can retain at once. Furthermore, AI service providers typically charge based on the volume of input and output tokens, making token efficiency a key metric for optimizing operational expenses and system performance.

## Key Aspects
- **Variable Length**: One token typically equals 0.75 words in English, though this ratio varies significantly across different languages and technical jargon.
- **Context Limits**: The maximum number of tokens an LLM can process simultaneously defines its context window, directly impacting its ability to handle long documents or complex multi-turn conversations.
- **Cost Driver**: Inference costs are calculated per token; optimizing prompts to reduce unnecessary token usage is a primary strategy for lowering AI operational budgets.
- **Semantic Granularity**: Tokenization splits rare words or complex terms into smaller sub-word units, allowing models to generalize better across unseen vocabulary.
