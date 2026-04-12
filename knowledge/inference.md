---
title: "Inference"
slug: "inference"
description: "The process of running a trained AI model to generate outputs from inputs — the computational step that costs money."
tags:
  - llm-fundamentals
  - ai-strategy
related:
  - token-economics
  - ai-infrastructure
  - context-window
  - scaling-laws
created: "2026-03-19"
updated: "2026-03-19"
confidence: high
---

Inference is the process of feeding input to a trained AI model and getting output back. Every time you send a message to Claude, ask GPT to write code, or have an agent execute a task, you're running inference. While training a model happens once (at enormous cost), inference happens billions of times and is the primary ongoing cost of AI operations.

Inference economics shape everything downstream. The cost of inference determines which applications are viable ([token economics](/knowledge/token-economics)), how many agents you can run simultaneously ([agent orchestration](/knowledge/agent-orchestration)), and whether [AI-native economics](/knowledge/ai-native-economics) pencil out. The $1,000/day AI spend that productive teams report is almost entirely inference cost. [AI infrastructure](/knowledge/ai-infrastructure) — GPUs, data centers, networking — exists primarily to serve inference at scale.

## Key Aspects

- **Cost per token** — inference is priced per token processed; larger [context windows](/knowledge/context-window) and longer outputs cost proportionally more
- **Latency vs. throughput** — fast inference enables interactive use; high throughput enables batch processing and parallel agents
- **Inference-time compute** — newer models use "thinking" or chain-of-thought at inference time, trading more compute for better answers
- **Optimization competition** — [frontier labs](/knowledge/frontier-labs) compete aggressively on inference cost; Google's Gemini 3.1 Pro achieves comparable quality at one-seventh the cost of Claude Opus 4.6

## Related Content

- [Google's New AI Is Smarter But Costs HALF as Much](/videos/8jKAT8GNDE0) — inference cost competition
- [$1,000 a Day in AI Costs. Three Engineers.](/videos/-bQcWs1Z9a0) — inference costs in practice
- [Why the Smartest AI Teams Are Panic-Buying Compute](/videos/pSgy2P2q790) — infrastructure for inference at scale
