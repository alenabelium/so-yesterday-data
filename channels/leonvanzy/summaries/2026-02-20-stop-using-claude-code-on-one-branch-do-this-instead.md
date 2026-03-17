---
title: "Stop Using Claude Code on One Branch (Do This Instead)"
video_id: 6nFRJftouI0
date: 2026-02-20
url: https://www.youtube.com/watch?v=6nFRJftouI0
channel: Leon van Zyl
tags:
  - coding
  - ai-tools
  - productivity
  - tutorials
transcript: ../transcripts/2026-02-20-stop-using-claude-code-on-one-branch-do-this-instead.md
---

# Stop Using Claude Code on One Branch (Do This Instead)

## Executive Summary

Git worktrees let you create multiple independent copies of your project, each with its own Claude Code instance running in parallel. This enables side-by-side comparison of different approaches -- different design skills, reference images, or even different AI models (Claude vs Gemini) -- without the slow cycle of implementing, reverting, and reimplementing on a single branch. Once you pick your favorite variant, git knows the relationship between worktrees and main, so merging the winning changes back is seamless.

## Key Points

- Git worktrees create full replicas of your project folder that git tracks and links to the main branch -- unlike simple folder copies, they support proper merging, conflict resolution, and appear in VS Code's source control with per-worktree change tracking. [02:39](https://www.youtube.com/watch?v=6nFRJftouI0&t=159)
- The demo compares three parallel approaches to redesigning a fitness app: one using a front-end design skill, one using a design system from a Dribbble reference image, and one using Gemini 3.1 Pro instead of Claude -- all running simultaneously on the same codebase. [05:07](https://www.youtube.com/watch?v=6nFRJftouI0&t=307)
- Worktrees are essential for model comparison: running the same prompt through different models or techniques in parallel worktrees gives you concrete side-by-side results to evaluate, rather than relying on benchmarks or opinions. [12:11](https://www.youtube.com/watch?v=6nFRJftouI0&t=731)
