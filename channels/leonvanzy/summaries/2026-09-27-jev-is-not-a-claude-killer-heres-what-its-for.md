---
title: "Jev Is Not a Claude Killer. Here's What It's For"
video_id: iyIAdmeKeMM
date: 2026-09-27
url: https://www.youtube.com/watch?v=iyIAdmeKeMM
channel: Leon van Zyl
tags:
  - ai-strategy
  - coding
  - productivity
  - ai-tools
transcript: ../transcripts/2026-09-27-jev-is-not-a-claude-killer-heres-what-its-for.md
relevant: true
---

# Jev Is Not a Claude Killer. Here's What It's For

## Executive Summary

The video argues that Jeff from TypeSafe AI is not a general-purpose LLM like Claude but rather a specialized 'System 1' model designed for instant, low-cost classification tasks. The presenter demonstrates how to use Jeff to automatically categorize GitHub issues and route them to appropriate coding agents within a software factory workflow. By leveraging Jeff's deterministic output structure and confidence scores, developers can build efficient, automated pipelines that significantly reduce operational costs compared to using larger reasoning models.

## Key Points

- Jeff is categorized as a 'System 1' model optimized for fast, cheap classification tasks like choice, score, or zero decisions, rather than complex reasoning or chat. [00:02:38](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=158)
- The presenter builds a GitHub workflow where Jeff classifies new issues as bugs, enhancements, or documentation and assigns them to specific agents like Codex or Claude Haiku based on the task type. [00:00:54](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=54)
- Using Jeff for classification is drastically cheaper than using advanced models, costing approximately $21 for one million classifications compared to $1,500 for Sonnet 5. [00:05:35](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=335)
- The implementation involves setting up a GitHub Action that triggers Jeff via API whenever a new issue is created, parsing the deterministic JSON response to apply labels and route the ticket. [00:13:36](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=816)
