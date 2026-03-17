---
title: "Your Claude Code Terminal Should Look Like This"
video_id: fiZfVTsPy-w
date: 2026-01-08
url: https://www.youtube.com/watch?v=fiZfVTsPy-w
channel: Leon van Zyl
tags:
  - coding
  - ai-tools
  - productivity
  - tutorials
transcript: ../transcripts/2026-01-08-your-claude-code-terminal-should-look-like-this.md
---

# Your Claude Code Terminal Should Look Like This

## Executive Summary

The built-in `/status-line` command in Claude Code lets you display critical session info -- model name, context token usage with a progress bar, git branch, and project folder -- directly in your terminal. This prevents accidentally pushing changes to the wrong branch and eliminates the need to interrupt your workflow with `/context` checks. The setup works on Windows, Mac, and Linux (Linux/Mac require JQ installed), and the status line can be customized with different colors and data points.

## Key Points

- The status line displays context window usage as a live progress bar, which is critical because exceeding the token limit causes conversation compaction that drops important context and degrades response quality. [00:00](https://www.youtube.com/watch?v=fiZfVTsPy-w&t=0)
- When setting up the status line, always tell Claude your operating system and request a separate script file (PS1 for Windows, .sh for Linux/Mac) to avoid bloating your global settings file. [01:50](https://www.youtube.com/watch?v=fiZfVTsPy-w&t=110)
- If the status line shows incorrect values, use a debugging technique: ask Claude to write the raw JSON structure to a debug file, then reference that file to identify the correct properties -- a general tip applicable to any Claude Code troubleshooting. [07:00](https://www.youtube.com/watch?v=fiZfVTsPy-w&t=420)
