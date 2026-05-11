---
title: "Model Context Protocol"
slug: "mcp"
description: "An open standard for connecting AI models to external tools, data sources, and services."
tags:
  - ai-agents
  - ai-tools
related:
  - tool-use
  - ai-agents
sources:
  - {type: "video", id: "japT66frdhM", date: "2026-03-13", title: "One Simple System Gave All My AI Tools a Memory. Here's How."}
  - {type: "video", id: "DTgrzlQtOd0", date: "2026-01-22", title: "Claude Code Ends SaaS, the Gemini + Siri Partnership, and Math Finally Solves AI"}
created: "2026-03-19"
updated: "2026-03-19"
confidence: high
---

The Model Context Protocol (MCP) is an open standard developed by Anthropic that provides a universal way for AI models to connect with external tools, data sources, and services. Think of it as a USB-C port for AI — a single, standardized interface that replaces the need for custom integrations between every model and every tool.

Before MCP, connecting an LLM to a new tool required custom code for each model-tool pair. MCP defines a common protocol so that any MCP-compatible model can use any MCP-compatible tool. This dramatically reduces integration effort and creates a growing ecosystem where [tool use](/knowledge/tool-use) becomes plug-and-play.

## Key Aspects

- **Server-client architecture** — MCP servers expose tools and resources; MCP clients (AI models/agents) discover and invoke them through the standardized protocol
- **Tool discovery** — agents can dynamically discover what tools are available, their parameters, and how to call them
- **Ecosystem growth** — as more tools implement MCP, every [AI agent](/knowledge/ai-agents) that supports the protocol gains access to the entire ecosystem
- **Context provision** — beyond tools, MCP also standardizes how context (documents, data) is provided to models

For [The Builder](/personas/03-builder), MCP represents the shift from manually wiring tool integrations to plugging into a growing ecosystem. For [The Orchestrator](/personas/04-orchestrator), MCP enables managing agents that can dynamically discover and use whatever tools they need, without pre-configuring each integration.

## Related Content

- [One Simple System Gave All My AI Tools a Memory](/videos/japT66frdhM) — building connected tool ecosystems
- [Claude Code Ends SaaS](/videos/DTgrzlQtOd0) — how standardized tool access changes software
- [The Builder](/personas/03-builder) — persona shipping software with AI tool integrations
- [Constraint Encoding](/knowledge/constraint-encoding) — MCP servers can encode domain constraints alongside tool definitions
