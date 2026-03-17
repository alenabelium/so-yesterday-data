---
title: "Stop Paying Anthropic $200/Month for Claude Code"
video_id: 3uE33T0j1w8
date: 2026-01-20
url: https://www.youtube.com/watch?v=3uE33T0j1w8
channel: Leon van Zyl
tags:
  - coding
  - ai-tools
  - ai-strategy
  - tutorials
transcript: ../transcripts/2026-01-20-stop-paying-anthropic-200month-for-claude-code.md
---

# Stop Paying Anthropic $200/Month for Claude Code

## Executive Summary

You can use ZAI's GLM 4.7 models inside the Claude Code CLI at a fraction of Anthropic's pricing by routing API calls through ZAI's anthropic-compatible endpoint. The setup involves adding environment variables to your project or user-level settings.json that remap Opus, Sonnet, and Haiku to GLM equivalents, then providing a ZAI API key. You retain full access to all Claude Code features -- sub-agents, skills, MCP servers, and custom commands -- while paying as little as $6/month instead of up to $200.

## Key Points

- ZAI's GLM 4.7 models are comparable to Opus 4.5 on coding benchmarks but cost a fraction of the price -- their light plan is $6/month (3x the usage of Claude's $20 Pro plan) and their max plan is $30/month versus Claude's $100-200. [00:00](https://www.youtube.com/watch?v=3uE33T0j1w8&t=0)
- The configuration works by adding an environment block to settings.json that redirects all inference calls to ZAI's anthropic wrapper endpoint and maps Claude model names (Sonnet, Opus, Haiku) to GLM equivalents. [02:19](https://www.youtube.com/watch?v=3uE33T0j1w8&t=139)
- For security, store the API key in a settings.local.json file that's added to .gitignore, preventing accidental exposure when deploying the project to GitHub. [05:13](https://www.youtube.com/watch?v=3uE33T0j1w8&t=313)
