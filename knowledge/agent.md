---
title: "Agent"
slug: "agent"
description: "An AI system that pursues goals by planning, using tools, and acting with limited supervision — the general term the corpus uses for both single agents and agent fleets."
tags:
  - ai-agents
  - ai-tools
related:
  - ai-agents
  - tool-use
  - mcp
  - autonomous-agents
provenance: agent:stub-authoring-v1
created: "2026-05-19"
updated: "2026-09-30"
confidence: medium
---

An agent is an AI system wrapped in a loop: it takes a goal, plans steps, calls tools, observes results, and iterates until done or blocked. The corpus uses "agent" as the umbrella for everything from a single scripted tool-caller to persistent, stateful systems that operate across sessions. What separates an agent from a chat session is ownership of a task rather than a turn.

In practice the agent pattern has consolidated around a small set of primitives: a capable model, a tool interface (increasingly standardized via [MCP](/knowledge/mcp)), a memory or context strategy, and permission boundaries that define what the agent may do without asking. The engineering discipline around agents — specifications, evals, blast-radius control — matters as much as the agents themselves; see [AI agents](/knowledge/ai-agents) and [autonomous agents](/knowledge/autonomous-agents) for the capability ladder, and [task decomposition](/knowledge/task-decomposition) for how agents break goals into executable steps.

## Key Aspects

- **Goal ownership** — the agent holds the objective across many tool calls, not just one reply
- **Tool access** — [tool use](/knowledge/tool-use) turns a language model into an acting system
- **Permissions** — scoped authority; anything consequential needs human sign-off (see [evals](/knowledge/evals), [constraint encoding](/knowledge/constraint-encoding))
- **Observability** — logs and audit trails so agent actions are reconstructable
