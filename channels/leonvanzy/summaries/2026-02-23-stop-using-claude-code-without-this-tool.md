---
title: "Stop Using Claude Code Without This Tool"
video_id: CQeKmG1o85E
date: 2026-02-23
url: https://www.youtube.com/watch?v=CQeKmG1o85E
channel: Leon van Zyl
tags:
  - ai-tools
  - coding
  - productivity
  - tutorials
transcript: ../transcripts/2026-02-23-stop-using-claude-code-without-this-tool.md
---

# Stop Using Claude Code Without This Tool

## Executive Summary

N8N and Claude Code are complementary tools, not competitors. The video demonstrates four powerful integration patterns: converting N8N workflow prototypes into full applications with Claude Code, exposing N8N workflows as webhook-backed backends for Claude-built UIs, turning any N8N workflow into an MCP server that Claude Code can call directly (e.g., to-do lists, Gmail, Slack), and using N8N webhooks with Claude Code hooks to send Telegram notifications when agents complete their work. The Claude browser extension can even create N8N workflows visually without touching the N8N UI.

## Key Points

- N8N workflows can be exposed as MCP servers that Claude Code accesses directly -- in the demo, a data table with to-dos becomes queryable and writable from Claude Code by publishing the workflow with an MCP trigger and adding the SSE endpoint to mcp.json. [07:22](https://www.youtube.com/watch?v=CQeKmG1o85E&t=442)
- Claude Code's built-in hooks feature (configured via `/hooks`) can call an N8N webhook on session stop, sending the agent's final message to Telegram, Slack, or any platform -- enabling you to walk away while Claude works and get notified when done. [10:29](https://www.youtube.com/watch?v=CQeKmG1o85E&t=629)
- The fastest prototyping workflow is building in N8N first (e.g., a Sora 2 video generator was created in under 5 minutes), then either converting the workflow to a standalone app with Claude Code or keeping N8N as the backend behind a Claude-built UI. [00:00](https://www.youtube.com/watch?v=CQeKmG1o85E&t=0)
