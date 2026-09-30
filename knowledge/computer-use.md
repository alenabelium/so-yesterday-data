---
title: "Computer Use (Agents)"
slug: "computer-use"
description: "Agents that operate software through the same visual interface humans use — clicking, typing, reading screens — instead of through APIs."
tags:
  - ai-agents
  - ai-tools
related:
  - tool-use
  - mcp
  - agent
  - claude
  - evals
provenance: agent:stub-authoring-v1
created: "2026-05-19"
updated: "2026-09-30"
confidence: medium
---

Computer-use agents control a machine the way a person does: they see the screen, move the pointer, type, and read the result. Where [tool use](/knowledge/tool-use) gives an agent a designed API, computer use gives it the *universal* interface — every application a human can operate becomes agent-operable, no integration required. The corpus tracked the inflection carefully: once these agents crossed reliability thresholds, they became the fallback path for long-tail automation (legacy apps, arbitrary websites) that no one will ever build an [MCP](/knowledge/mcp) connector for.

The discipline around them is the standard agentic one, intensified: a computer-use agent holds real credentials, so scoped environments, session isolation, screenshot-level audit logs, and human gating for consequential actions are the deployment pattern (see [evals](/knowledge/evals)). Strategically, computer use reframes "integration" as a spectrum — API where available, UI where not — and shifts the value question from "can it operate my software" to "can I specify and verify what it should do" ([specification quality](/knowledge/specification-quality)).
