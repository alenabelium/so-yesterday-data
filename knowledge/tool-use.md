---
title: "Tool Use"
slug: "tool-use"
description: "The ability of LLMs to interact with external tools, APIs, and systems to extend their capabilities."
tags:
  - ai-agents
  - ai-tools
related:
  - ai-agents
  - mcp
sources:
  - {type: "video", id: "h7dbkDcb3hA", date: "2026-01-14", title: "Task Queues Are Replacing Chat Interfaces. Here's Why (plus a Claude Cowork Demo)"}
  - {type: "video", id: "japT66frdhM", date: "2026-03-13", title: "One Simple System Gave All My AI Tools a Memory. Here's How."}
  - {type: "video", id: "09sFAO7pklo", date: "2026-03-06", title: "Claude Code vs Codex: The Decision That Compounds Every Week You Delay That Nobody Is Talking About"}
created: "2026-03-19"
updated: "2026-03-19"
confidence: high
---

Tool use is the mechanism by which large language models extend beyond text generation to interact with the real world. By calling external tools — APIs, code interpreters, file systems, web browsers, databases — LLMs transform from knowledge repositories into action-taking systems.

Tool use is the foundational capability that makes [AI agents](/knowledge/ai-agents) possible. Without tools, an LLM can only generate text. With tools, it can write and execute code, search the web, create files, send messages, and orchestrate complex workflows. The standardization of tool interfaces through protocols like [MCP](/knowledge/mcp) is accelerating the ecosystem of tools available to agents.

## Key Aspects

- **Function calling** — LLMs generate structured tool invocations (function name + arguments) that the host system executes, returning results back to the model
- **Tool selection** — agents must decide which tool to use and when, a form of planning that improves with model capability
- **Composability** — complex tasks often require chaining multiple tool calls, where the output of one tool becomes the input of another
- **Safety boundaries** — tool use requires careful permission systems to prevent agents from taking destructive or unauthorized actions

The [Builder](/personas/03-builder) persona navigates two distinct tool paths: builder platforms (Lovable, Bolt, Replit) for fast prototyping with less control, and command-line tools (Claude Code, Cursor, Windsurf) for full ownership and deeper capability. The choice between these paths shapes the Builder's entire workflow and skill development.

## Related Content

- [Task Queues Are Replacing Chat Interfaces](/videos/h7dbkDcb3hA) — evolution from chat to tool-based agent interfaces
- [One Simple System Gave All My AI Tools a Memory](/videos/japT66frdhM) — connecting tools to persistent memory
- [Claude Code vs Codex](/videos/09sFAO7pklo) — comparing tool-use capabilities across coding agents
- [The Orchestrator](/personas/04-orchestrator) — persona managing tool-equipped agent fleets
- [The Builder](/personas/03-builder) — persona navigating the choice between builder platforms and CLI tools
