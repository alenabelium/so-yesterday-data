---
title: "Claude Code Skills - The Only Tutorial You Need"
video_id: vIUJ4Hd7be0
date: 2026-02-09
url: https://www.youtube.com/watch?v=vIUJ4Hd7be0
channel: Leon van Zyl
tags:
  - ai-tools
  - coding
  - tutorials
  - prompting
transcript: ../transcripts/2026-02-09-claude-code-skills-the-only-tutorial-you-need.md
---

# Claude Code Skills - The Only Tutorial You Need

## Executive Summary

Skills are markdown-based instruction files that teach Claude Code specialized workflows it cannot perform natively, like generating images or enforcing design systems. Unlike MCP servers that preload all tool metadata into context, skills only inject detailed instructions when activated, consuming far fewer tokens. The video covers finding skills on skills.sh, installing them via CLI commands, and creating custom skills -- including a Nano Banana Pro image generator and an image optimizer -- with secure API key handling through environment variables.

## Key Points

- Skills use dramatically less context than MCP servers because only a brief description is loaded initially; the full skill instructions are pulled in only when the agent decides to use the skill, keeping the context window lean for all other tasks. [02:21](https://www.youtube.com/watch?v=vIUJ4Hd7be0&t=141)
- The skills.sh marketplace from Vercel makes finding and installing skills trivial -- copy a single command, select your CLI tool, and choose project or global scope; the "find skills" skill even lets the agent search and install skills autonomously. [05:45](https://www.youtube.com/watch?v=vIUJ4Hd7be0&t=345)
- When creating custom skills that require API keys, never hardcode them -- store keys in a .env file excluded from git, and instruct the skill's Python script to read from environment variables to prevent accidental exposure. [16:24](https://www.youtube.com/watch?v=vIUJ4Hd7be0&t=984)
