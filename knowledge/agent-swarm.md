---
title: "Agent Swarm"
slug: "agent-swarm"
description: "Many agents working in parallel on decomposed tasks under an orchestrator — the 'AI software factory' pattern at scale."
tags:
  - ai-agents
  - ai-strategy
related:
  - multi-agent-systems
  - agent-orchestration
  - task-decomposition
  - ai-software-factory
provenance: agent:stub-authoring-v1
created: "2026-05-19"
updated: "2026-09-30"
confidence: medium
---

An agent swarm is the scaled form of [multi-agent systems](/knowledge/multi-agent-systems): a fleet of agents executing [decomposed](/knowledge/task-decomposition) tasks concurrently, coordinated by an orchestrator that assigns, merges and verifies. The corpus's "AI software factory" pattern is the flagship instance — parallel generation with structured integration and human gates — and the evidence is consistent: swarms multiply throughput on decomposable work and multiply coordination cost on anything with tight interdependencies.

The engineering rules that survived contact: decompose along seams that minimize cross-task state; verify at integration, not just per-task; cap concurrency against the [blast radius](/knowledge/blast-radius) of a bad merge; and keep a human accountable node in the loop (see [agent orchestration](/knowledge/agent-orchestration)).
