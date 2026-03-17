---
title: "Claude Code + Ollama = Free Forever"
video_id: 3x2q6-5XbQ8
date: 2026-01-25
url: https://www.youtube.com/watch?v=3x2q6-5XbQ8
channel: Leon van Zyl
tags:
  - ai-tools
  - coding
  - tutorials
  - llm-fundamentals
transcript: ../transcripts/2026-01-25-claude-code-ollama-free-forever.md
---

# Claude Code + Ollama = Free Forever

## Executive Summary

Claude Code can run entirely free using local open-source models via Ollama, with no subscription or API key required. The setup involves installing Ollama, downloading a model (Qwen 3 Coder recommended), and launching Claude Code with the `ollama launch claude` command. While local models cannot match Opus or Sonnet quality, they provide full access to all Claude Code features -- sub-agents, skills, MCP servers, and custom commands -- making them ideal for beginners or quick edits.

## Key Points

- Qwen 3 Coder (19GB, 30B parameters) is the recommended local model because it supports a 256K token context window that comfortably exceeds Claude Code's 200K limit, whereas GPT-OSS models only have 128K tokens and degrade at 50% usage. [08:12](https://www.youtube.com/watch?v=3x2q6-5XbQ8&t=492)
- To start Claude Code with Ollama without any subscription, run `ollama launch claude` -- this skips the authentication step entirely and lets you select between downloaded models using the `--config` flag. [04:46](https://www.youtube.com/watch?v=3x2q6-5XbQ8&t=286)
- Local models are best suited for quick code edits, codebase exploration, and learning agentic coding on consumer hardware, but they will not match the quality of cloud models like Opus for complex implementations. [06:06](https://www.youtube.com/watch?v=3x2q6-5XbQ8&t=366)
