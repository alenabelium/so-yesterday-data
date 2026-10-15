---
title: "Faster matrix multiplication through Machine Learning obtained by DeepMind"
video_id: cd_xZRskv9A
date: 2026-08-19
url: https://www.youtube.com/watch?v=cd_xZRskv9A
channel: Dr. Samuel Allen Alexander
tags:
  - ai-strategy
  - ai-tools
  - llm-fundamentals
  - industry-news
transcript: ../transcripts/2026-08-19-faster-matrix-multiplication-through-machine-learning-obtain.md
relevant: true
knowledge: true
highlight: true
---

# Faster matrix multiplication through Machine Learning obtained by DeepMind

## Executive Summary

DeepMind's new paper improves the upper bound for the matrix multiplication exponent omega to less than 2.371177, a modest but significant advancement over the previous best of 2.371339. The improvement is achieved by reformulating the optimization problem, using gradient-based machine learning techniques, and applying AlphaEvolve to refine the optimization algorithm. This work is notable because matrix multiplication is a fundamental bottleneck in machine learning, so any speedup can accelerate AI systems broadly. The video highlights that this is an example of machine learning improving itself, though the gain is small and required substantial manual effort.

## Key Points

- DeepMind's paper improves the matrix multiplication exponent omega to less than 2.371177, a small but notable improvement over the previous bound of 2.371339. [00:01:17](https://www.youtube.com/watch?v=cd_xZRskv9A&t=77)
- The optimization problem is reformulated to handle larger scales (Lstar=4) with nearly 7 million parameters, using gradient descent and JAX for parallelization. [00:04:57](https://www.youtube.com/watch?v=cd_xZRskv9A&t=297)
- AlphaEvolve is used to further refine the optimization algorithm, contributing to the final improvement. [00:37:40](https://www.youtube.com/watch?v=cd_xZRskv9A&t=2260)
