---
title: "Claude Code /loop Does the Work Nobody Wants to Do"
video_id: 7JKTLLW856I
date: 2026-03-11
url: https://www.youtube.com/watch?v=7JKTLLW856I
channel: Leon van Zyl
tags:
  - coding
  - productivity
  - ai-tools
  - tutorials
transcript: ../transcripts/2026-03-11-claude-code-loop-does-the-work-nobody-wants-to-do.md
---

# Claude Code /loop Does the Work Nobody Wants to Do

## Executive Summary

The `/loop` command in Claude Code creates scheduled cron jobs that automatically run prompts at specified intervals, automating tedious maintenance tasks that developers typically forget. The video demonstrates practical use cases: auto-updating CLAUDE.md every 30 minutes, keeping public-facing documentation in sync every 2 hours, running test suites automatically, scheduling UI design system review sub-agents hourly, and monitoring pull requests for merge-ready changes. Jobs can also invoke custom commands and can be bootstrapped together via a single `/init-loops` custom command.

## Key Points

- The `/loop` command creates cron jobs that run prompts on intervals (e.g., every 30 minutes, every weekday at 9am), with a maximum of 50 jobs per session; jobs expire after 3 days and only run while the Claude Code session is open. [00:00](https://www.youtube.com/watch?v=7JKTLLW856I&t=0)
- Combining `/loop` with custom commands and sub-agents automates complex workflows -- for example, scheduling an hourly loop that invokes a custom `/review-refactor-ui` command, which in turn triggers a UI design system reviewer sub-agent to enforce design consistency. [11:01](https://www.youtube.com/watch?v=7JKTLLW856I&t=661)
- All loop jobs can be defined in a single custom command file (e.g., `init-loops.md`) so they can be spun up at the start of any session with one slash command, making it easy to maintain and update the full set of scheduled automation. [15:49](https://www.youtube.com/watch?v=7JKTLLW856I&t=949)
