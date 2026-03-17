---
title: "Stop Using Claude Code Like This (Use Sub-Agents Instead)"
video_id: P60LqQg1RH8
date: 2026-01-14
url: https://www.youtube.com/watch?v=P60LqQg1RH8
channel: Leon van Zyl
tags:
  - tutorials
  - coding
  - llm-fundamentals
  - ai-agents
transcript: ../transcripts/2026-01-14-stop-using-claude-code-like-this-use-sub-agents-instead.md
---

# Stop Using Claude Code Like This (Use Sub-Agents Instead)

## Executive Summary

Sub-agents are the key to protecting Claude Code's main context window, which degrades quality when it fills up and compacts. The video demonstrates how to create specialized sub-agents (coder, UI expert, code reviewer) and use them to offload work into separate context windows that don't consume the main thread's tokens. The culminating workflow has the main Opus agent act as an orchestrator that delegates coding to parallel Sonnet sub-agents and code review to Haiku sub-agents, implementing a complex full-stack app with authentication and Postgres while keeping the main context at only 68%.

## Key Points

- Sub-agents run in their own context windows, so their token usage does not affect the main thread -- in a complex build, the main agent stayed at 68% utilization instead of the 100%+ that would have required compaction with a single-thread approach. [12:09](https://www.youtube.com/watch?v=P60LqQg1RH8&t=729)
- Creating specialized agents (coder on Sonnet, code reviewer on Haiku, UI expert on Opus) via the `/agents` command lets you bake domain-specific rules into each agent's system prompt, ensuring consistent behavior without cluttering the main conversation. [07:02](https://www.youtube.com/watch?v=P60LqQg1RH8&t=422)
- The orchestrator workflow -- where the main agent identifies parallel tracks from an implementation plan and delegates coding and review to sub-agents running concurrently -- produced a fully functional app with auth and database in a single session. [24:09](https://www.youtube.com/watch?v=P60LqQg1RH8&t=1449)
