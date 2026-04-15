---
title: "How does AI actually work? Transformers explained"
video_id: U2hZFMVNSE0
date: 2026-03-25
url: https://www.youtube.com/watch?v=U2hZFMVNSE0
channel: The AI Search
tags:
  - llm-fundamentals
  - tutorials
transcript: ../transcripts/2026-03-25-how-does-ai-actually-work-transformers-explained.md
---

# How does AI actually work? Transformers explained

## Executive Summary

This educational deep-dive explains how transformer-based large language models like GPT and Gemini actually work, walking through the complete decoder-only architecture from the original "Attention Is All You Need" paper. The video covers tokenization (breaking text into meaningful subwords), input embeddings (converting tokens into high-dimensional vectors capturing meaning), positional encoding (using sine/cosine functions to encode word order), masked multi-head attention (the core mechanism that lets each word understand context by computing relevance to every other word), feed-forward neural networks, residual connections, and the final softmax layer that produces next-word probabilities. It also explains training via backpropagation and gradient descent.

## Key Points

- The masked multi-head attention mechanism is the core innovation: for each word, it computes query, key, and value vectors to determine which other words are most relevant, with multiple attention heads running in parallel to capture different types of contextual relationships (subject-verb agreement, pronoun references, etc.). [09:43](https://www.youtube.com/watch?v=U2hZFMVNSE0&t=583)
- Residual (skip) connections after each attention and feed-forward block are critical -- they add the original input vectors back into the transformed output, preventing the model from losing the original meaning and position information through many layers of computation. [20:07](https://www.youtube.com/watch?v=U2hZFMVNSE0&t=1207)
- Training starts with entirely random values across all matrices and neural network weights; through billions of iterations of backpropagation and gradient descent, the model gradually learns word meanings, grammar, sentence structure, and subtle long-range relationships in text. [28:03](https://www.youtube.com/watch?v=U2hZFMVNSE0&t=1683)
