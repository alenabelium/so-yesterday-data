---
title: "Stop Using Claude Code the Normal Way"
video_id: lGWFlpffWk4
date: 2026-01-05
url: https://www.youtube.com/watch?v=lGWFlpffWk4
channel: Leon van Zyl
tags:
  - coding
  - ai-tools
  - tutorials
  - ai-agents
transcript: ../transcripts/2026-01-05-stop-using-claude-code-the-normal-way.md
---

# Stop Using Claude Code the Normal Way

## Executive Summary

Long-running agent harnesses are the future of agentic coding because single-context-window sessions lose critical context when compacting, producing incomplete and buggy applications. The video compares two builds from the exact same prompt: a vanilla Claude Code session that missed many features versus a long-running harness that delivered a polished, fully functional app with thumbnail generation, card editing with history, and reference image support. The harness works by splitting requirements into hundreds of granular features stored in a SQLite database, then cycling through coding agents -- each with their own context window -- that implement features and run regression tests using a real browser.

## Key Points

- The long-running agent harness splits a massive prompt into hundreds of individual features, each implemented by separate coding agents with their own context windows, avoiding the quality degradation caused by context compaction in single-session builds. [05:37](https://www.youtube.com/watch?v=lGWFlpffWk4&t=337)
- A key improvement over Anthropic's original harness is storing features in a SQLite database instead of a massive JSON file, accessed via a dedicated MCP server, which reduces token usage and improves performance. [23:54](https://www.youtube.com/watch?v=lGWFlpffWk4&t=1434)
- The coding agents use browser-based test-driven development to visually verify each feature in real time, catching UI bugs that blind implementation would miss -- though this consumes more tokens and time, it produces production-ready results. [26:02](https://www.youtube.com/watch?v=lGWFlpffWk4&t=1562)
