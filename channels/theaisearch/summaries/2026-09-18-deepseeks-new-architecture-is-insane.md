---
title: "Deepseek's new architecture is insane"
video_id: MImgH4KMtj8
date: 2026-09-18
url: https://www.youtube.com/watch?v=MImgH4KMtj8
channel: The AI Search
tags:
  - ai-strategy
  - coding
  - productivity
  - tutorials
transcript: ../transcripts/2026-09-18-deepseeks-new-architecture-is-insane.md
relevant: true
knowledge: true
highlight: false
---

# Deepseek's new architecture is insane

## Executive Summary

DeepSeek V4.1 Flash achieves frontier-level performance with unprecedented efficiency by radically rethinking transformer architecture. The model splits processing into a causal encoder for global context and a decoder for local generation, drastically reducing memory overhead. Through techniques like Compressed Sparse Attention 2 and deleting short-term memory to recalculate on the fly, it minimizes data transfer bottlenecks. This allows the model to maintain constant compute costs even as context windows expand to one million tokens.

## Key Points

- The architecture splits layers into a causal encoder for global context and a decoder for local generation, bypassing the need for half the model to generate its own massive KV cache [00:07:49](https://www.youtube.com/watch?v=MImgH4KMtj8&t=469).
- DeepSeek uses Compressed Sparse Attention 2 (CSA2) with reindex and reuse modes to shrink the global KV cache size by over 400 times compared to previous generations [00:13:18](https://www.youtube.com/watch?v=MImgH4KMtj8&t=798).
- The model eliminates short-term memory storage by deleting local context after each turn and recalculating the last 128 tokens on the GPU, which is faster than fetching from SSDs [00:19:12](https://www.youtube.com/watch?v=MImgH4KMtj8&t=1152).
- Supplementary components like the Engram module for static facts and DS-Spark for multi-token output further optimize speed and reduce expensive GPU memory usage [00:23:52](https://www.youtube.com/watch?v=MImgH4KMtj8&t=1432). [MM:SS](https://www.youtube.com/watch?v=MImgH4KMtj8&t=SECONDS)
