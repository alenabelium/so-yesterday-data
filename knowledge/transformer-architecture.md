---
title: "Transformer Architecture"
slug: "transformer-architecture"
description: "The neural network architecture behind all modern LLMs, based on the self-attention mechanism."
tags:
  - llm-fundamentals
related:
  - scaling-laws
  - inference
  - context-window
  - multimodal-ai
  - emergent-behavior
confidence: high
created: "2026-04-15"
updated: "2026-04-15"
---

The transformer is the neural network architecture underlying all modern large language models, introduced in the 2017 paper "Attention Is All You Need." Its core innovation is the self-attention mechanism, which allows each token in a sequence to compute relevance scores against every other token, enabling the model to capture long-range dependencies that previous architectures (RNNs, LSTMs) struggled with. The architecture processes input through tokenization (breaking text into subword units), input embeddings (converting tokens into high-dimensional vectors), positional encoding (using sine/cosine functions to represent word order), multiple layers of multi-head attention, feed-forward neural networks, and residual connections.

The multi-head attention mechanism is the engine that makes transformers work. For each token, the model computes query, key, and value vectors to determine which other tokens are most relevant. Multiple attention heads run in parallel, each capturing different types of contextual relationships -- subject-verb agreement, pronoun references, semantic similarity, and more. Residual (skip) connections after each attention and feed-forward block are critical for deep networks: they add the original input back into the transformed output, preventing the model from losing meaning and position information through many layers of computation. Training starts with entirely random weights and, through billions of iterations of backpropagation and gradient descent, the model learns word meanings, grammar, and subtle long-range relationships.

The transformer architecture's dominance is being reinforced even as researchers explore alternatives. Silicon is being reorganized around the transformer as the primary workload -- Apple's M5 chips embed neural accelerators inside each GPU core specifically optimized for transformer inference. DeepSeek's research on manifold constrained hyperconnections expanded internal transformer data flow by 400%, challenging the fundamental residual connection design. Meanwhile, Sam Altman has reportedly used frontier models to discover post-transformer architectures, and a research team hard-coded a WebAssembly interpreter into transformer weights, proving neural nets are practical general-purpose computers. The architecture's relationship to [scaling laws](/knowledge/scaling-laws) remains the strategic foundation: predictable performance improvement with more compute, data, and parameters.

## Key Aspects

- **Self-attention mechanism** -- each token computes relevance scores against all other tokens via query, key, and value vectors, enabling long-range dependency capture that prior architectures could not achieve
- **Multi-head attention** -- multiple parallel attention heads capture different types of relationships (syntax, semantics, coreference), giving the model rich contextual understanding
- **Residual connections** -- skip connections after each layer prevent signal degradation in deep networks by preserving original token representations through many layers of transformation
- **Decoder-only dominance** -- modern LLMs use decoder-only transformers (dropping the encoder) for autoregressive text generation, optimized by [inference-time scaling](/knowledge/inference)

## Related Content

- [How does AI actually work? Transformers explained](/videos/U2hZFMVNSE0) -- comprehensive walkthrough of the decoder-only transformer architecture
- [DeepSeek is back, realtime upscaler, 3D worlds](/videos/7kPNA86G_GA) -- manifold constrained hyperconnections challenging residual connection design
- [Scaling Laws](/knowledge/scaling-laws) -- the empirical finding that transformer performance scales predictably with compute
- [Context Window](/knowledge/context-window) -- the token limit that defines how much information a transformer can process at once
- [Inference](/knowledge/inference) -- the computational process of running a trained transformer to generate outputs
- [Multimodal AI](/knowledge/multimodal-ai) -- extending the transformer architecture to process multiple input modalities
