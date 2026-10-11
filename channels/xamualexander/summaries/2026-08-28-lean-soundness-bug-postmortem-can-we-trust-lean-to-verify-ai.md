---
title: "Lean soundness bug postmortem: Can we trust Lean to verify AI-generated mathematics?"
video_id: 7oJcB1zBi4A
date: 2026-08-28
url: https://www.youtube.com/watch?v=7oJcB1zBi4A
channel: Dr. Samuel Allen Alexander
tags:
  - ai-safety
  - ai-strategy
  - llm-fundamentals
  - industry-news
transcript: ../transcripts/2026-08-28-lean-soundness-bug-postmortem-can-we-trust-lean-to-verify-ai.md
relevant: true
knowledge: true
highlight: true
---

# Lean soundness bug postmortem: Can we trust Lean to verify AI-generated mathematics?

## Executive Summary

This video is a postmortem analysis of a soundness bug hunt in the Lean theorem prover, prompted by a false refutation of the Collatz conjecture. The hunt, conducted with OpenAI's internal models, uncovered several kernel and runtime bugs that could be exploited to prove false statements. The Lean team has responded with fixes, new verification tools, and plans for more robust kernels. The video also discusses the implications for using Lean to verify AI-generated mathematics and raises questions about the trustworthiness of such systems.

## Key Points

- The Lean soundness bug hunt, prompted by a false Collatz refutation, used OpenAI internal models to find multiple kernel and runtime bugs that could prove false statements. [00:01:07](https://www.youtube.com/watch?v=7oJcB1zBi4A&t=67)
- The OpenAI internal model found two runtime exploits: one overflowing reference counters to corrupt memory and another exploiting an outdated GMP version in the Linux distribution. [00:03:00](https://www.youtube.com/watch?v=7oJcB1zBi4A&t=180)
- The Lean team is adding new verification tools like 'lake check' and multiple kernels (including Lean for Lean and Nanoda) to increase trust, but acknowledges that absolute certainty of no bugs is impossible. [00:09:22](https://www.youtube.com/watch?v=7oJcB1zBi4A&t=562)
