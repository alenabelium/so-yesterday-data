---
title: "Why Frontier AI Labs Fight to Hide Chain of Thought — Ilia Shumailov & Alexander Panfilov"
video_id: gasgivVCl2U
date: 2026-08-22
url: https://www.youtube.com/watch?v=gasgivVCl2U
channel: Machine Learning Street Talk
tags:
  - ai-safety
  - ai-agents
  - llm-fundamentals
  - industry-news
transcript: ../transcripts/2026-08-22-why-frontier-ai-labs-fight-to-hide-chain-of-thought-ilia-shu.md
relevant: true
knowledge: true
highlight: true
---

# Why Frontier AI Labs Fight to Hide Chain of Thought — Ilia Shumailov & Alexander Panfilov

## Executive Summary

Researchers Ilia Shumailov and Alexander Panfilov discuss their discovery that encrypted chain-of-thought reasoning blocks from frontier AI models (OpenAI, Anthropic, Google) can be decrypted and replayed using smaller models from the same family, enabling attacks like prompt injection, jailbreaking, and privacy breaches. They highlight that this architectural vulnerability is widespread across major labs and can be exploited without breaking cryptography, simply by having smaller models reveal the decrypted thoughts. The conversation covers the implications for model distillation, the strange and often incomprehensible nature of model reasoning, and the ongoing efforts to mitigate these risks through architectural changes and monitoring.

## Key Points

- Researchers found that encrypted reasoning blocks from frontier models can be decrypted and replayed using smaller models, enabling attacks like prompt injection and jailbreaking. [00:02:07](https://www.youtube.com/watch?v=gasgivVCl2U&t=127)
- The vulnerability is architectural: reasoning blocks are portable across users and models, allowing fabricated conversations and extraction of sensitive data from public traces. [00:05:44](https://www.youtube.com/watch?v=gasgivVCl2U&t=344)
- The researchers demonstrated that pre-filling a small model with a few tokens from a larger model's reasoning can cause it to adopt the larger model's style and even visible response patterns, suggesting potential distillation. [00:18:09](https://www.youtube.com/watch?v=gasgivVCl2U&t=1089)
