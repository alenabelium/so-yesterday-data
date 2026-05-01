---
title: "Consensus AI + Claude Code = No More Hallucinations"
video_id: 5LCjeni0Z-U
date: 2026-04-21
url: https://www.youtube.com/watch?v=5LCjeni0Z-U
channel: Leon van Zyl
tags:
  - coding
  - ai-agents
  - ai-tools
  - productivity
transcript: ../transcripts/2026-04-21-consensus-ai-claude-code-no-more-hallucinations.md
---

# Consensus AI + Claude Code = No More Hallucinations

## Executive Summary

Leon van Zyl demonstrates Claude Code Routines, a new Anthropic feature that enables automated, scheduled agent workflows running in the cloud. He walks through building two routines from scratch: an auto-improver that identifies and implements app improvements via pull requests, and a security audit routine based on the OWASP Top 10 that automatically finds and fixes vulnerabilities. The video shows how routines differ from normal Claude usage by running autonomously on schedules or events, creating isolated feature branches, and integrating with GitHub and Slack without requiring the user's machine to be running.

## Key Points

- Claude Code Routines run autonomously in the cloud on configurable triggers (schedules, GitHub events, or API calls), enabling fully hands-off automation like hourly app improvements or daily security audits that create pull requests without human intervention. [01:42](https://www.youtube.com/watch?v=5LCjeni0Z-U&t=102)
- The auto-improver routine independently identified a missing edit feature in a to-do app, implemented click-to-edit functionality with an escape-key close bonus, and created a reviewable pull request -- all without any human guidance beyond the initial prompt. [04:33](https://www.youtube.com/watch?v=5LCjeni0Z-U&t=273)
- The OWASP-based security scanner found 75 critical issues in a simple Next.js app including hardcoded API keys, broken access control, missing CORS policies, and potential SQL injection, then automatically fixed the vulnerabilities and merged the changes. [08:34](https://www.youtube.com/watch?v=5LCjeni0Z-U&t=514)
