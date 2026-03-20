---
title: "Benchmarks"
slug: "benchmarks"
description: "Standardized tests and evaluation frameworks used to compare AI model capabilities and track progress."
tags:
  - llm-fundamentals
  - industry-news
related:
  - frontier-labs
  - frontier-recognition
  - scaling-laws
created: "2026-03-19"
updated: "2026-03-19"
---

Benchmarks are standardized tests used to measure and compare AI model capabilities. They range from narrow skill tests (math problems, code generation, factual recall) to broad capability evaluations (ARC-AGI for general reasoning, GPQA for graduate-level science, SWE-bench for real-world software engineering). When [frontier labs](/knowledge/frontier-labs) release new models, benchmark results are the primary language used to communicate what improved.

Benchmarks matter because they shape research priorities, investment decisions, and public perception. However, they're also deeply imperfect. Models can be optimized for specific benchmarks without genuine capability improvement ("teaching to the test"), and the skills measured by benchmarks may not reflect real-world usefulness. Google's Gemini 3.1 Pro leading on 13/16 benchmarks while costing one-seventh of Claude Opus 4.6 illustrates both the value and the limits of benchmark comparison.

For practitioners, [frontier recognition](/knowledge/frontier-recognition) — understanding what models can actually do in your domain — requires going beyond benchmarks to hands-on testing. Benchmarks tell you what a model *might* do; only experience tells you what it *will* do on your specific tasks.

## Key Aspects

- **Common benchmarks** — MMLU (general knowledge), HumanEval/SWE-bench (coding), ARC-AGI (reasoning), MATH (mathematical problem-solving), GPQA (expert-level science)
- **Benchmark saturation** — as models approach perfect scores on existing benchmarks, new harder benchmarks must be created (ARC-AGI2 replaced ARC-AGI)
- **Goodhart's Law** — when a measure becomes a target, it ceases to be a good measure; labs optimizing for benchmarks may not improve real capability
- **Benchmark vs. deployment gap** — strong benchmark performance doesn't guarantee strong real-world performance; the gap is where [the 70% problem](/knowledge/the-70-percent-problem) lives

## Related Content

- [Codex 5.3 vs Opus 4.6: The Benchmark Nobody Expected](/videos/41UDGsBEjoI) — benchmark comparison in practice
- [LeCun Said LLMs Are a Dead End—Then Revealed Meta Fudged Their Benchmarks](/videos/RgQtTvneqPY) — benchmark manipulation
- [Google's New AI Is Smarter But Costs HALF as Much](/videos/8jKAT8GNDE0) — benchmark leadership vs. cost
- [Claude Opus 4.6: The Biggest AI Jump](/videos/JKk77rzOL34) — benchmark breakthroughs
