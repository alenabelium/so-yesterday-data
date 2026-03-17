---
title: "Stop Using Claude Code Like a Beginner"
video_id: bL1PYhogwp0
date: 2026-02-03
url: https://www.youtube.com/watch?v=bL1PYhogwp0
channel: Leon van Zyl
tags:
  - coding
  - ai-tools
  - productivity
  - tutorials
transcript: ../transcripts/2026-02-03-stop-using-claude-code-like-a-beginner.md
---

# Stop Using Claude Code Like a Beginner

## Executive Summary

After six months of daily Claude Code use, the author shares a comprehensive set of power-user tips: use subscriptions over API keys, always enable thinking mode, start every feature in planning mode, break implementation plans into individual feature files, delegate work to specialized sub-agents (coder on Sonnet, reviewer on Haiku), prefer skills over MCP servers to save context tokens, and use the CLAUDE.md file, custom commands, and .claudeignore to control agent behavior. The overarching theme is protecting the main context window by keeping it lean and delegating aggressively.

## Key Points

- Opus is actually cheaper than Sonnet over the long run because it requires fewer reprompts to get correct results; the recommended model strategy is Opus for planning and complex coding, Sonnet for implementation with detailed plans, and Haiku for file exploration and code reviews. [00:00](https://www.youtube.com/watch?v=bL1PYhogwp0&t=0)
- When a build goes off the rails, rather than trying to course-correct mid-conversation, update the implementation plan with what went wrong, discard all changes, and start fresh -- this produces better results than fighting a degraded context. [10:08](https://www.youtube.com/watch?v=bL1PYhogwp0&t=608)
- Skills use dramatically fewer context tokens than MCP servers because they only load detailed instructions when invoked, while MCP server tool metadata sits in memory permanently -- the Playwright skill used a tiny fraction of the tokens compared to the Playwright MCP server. [16:26](https://www.youtube.com/watch?v=bL1PYhogwp0&t=986)
