---
title: "This Agent Team Builds 100s of Features While You Sleep"
video_id: nKiPOxDpcJY
date: 2026-02-05
url: https://www.youtube.com/watch?v=nKiPOxDpcJY
channel: Leon van Zyl
tags:
  - coding
  - ai-tools
  - ai-agents
  - tutorials
transcript: ../transcripts/2026-02-05-this-agent-team-builds-100s-of-features-while-you-sleep.md
---

# This Agent Team Builds 100s of Features While You Sleep

## Executive Summary

AutoForge (formerly the author's UI wrapper for Anthropic's long-running agent harness) has evolved into a full-featured open-source platform with 1,300 GitHub stars. It provides a kanban board UI, a conversation-driven spec generator, concurrent coding agents (up to 5 in parallel), regression testing agents, a graph view of feature dependencies, and support for Claude, GLM, and Ollama models. The platform stores features in a SQLite database and uses Playwright MCP for browser-based testing, letting complex projects with hundreds of features be built unattended.

## Key Points

- AutoForge runs up to five concurrent coding agents that implement features in parallel, with an orchestrator (Maestro) that assigns work based on the dependency graph -- features without dependencies are implemented simultaneously while dependent features wait. [10:06](https://www.youtube.com/watch?v=nKiPOxDpcJY&t=606)
- The conversational spec generator lets non-technical users describe what they want in plain language, then Claude creates an app_spec file and feature list; for existing projects, it analyzes the codebase first and adds new features on top. [06:41](https://www.youtube.com/watch?v=nKiPOxDpcJY&t=401)
- AutoForge supports swapping Claude models for GLM or Ollama by uncommenting environment variables in a .env file, enabling free local inference or much cheaper cloud inference while using the same platform. [18:11](https://www.youtube.com/watch?v=nKiPOxDpcJY&t=1091)
