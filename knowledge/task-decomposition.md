---
title: "Task Decomposition"
slug: "task-decomposition"
description: "Breaking complex goals into smaller, well-defined subtasks that AI agents can execute reliably."
tags:
  - ai-agents
  - productivity
related:
  - agent-orchestration
  - specification-quality
created: "2026-03-19"
updated: "2026-03-19"
confidence: high
---

Task decomposition is the practice of breaking complex goals into smaller, well-defined subtasks that can be independently executed and verified. It is one of the most important skills for working effectively with [AI agents](/knowledge/ai-agents), because agents perform dramatically better on focused, well-scoped tasks than on vague, open-ended ones.

Effective task decomposition requires understanding both the problem domain and the capabilities of the AI tools being used. The goal is to create subtasks that are small enough for reliable AI execution but large enough to be meaningful. This connects directly to [specification quality](/knowledge/specification-quality) — each subtask needs a clear spec — and [agent orchestration](/knowledge/agent-orchestration) — managing the execution of decomposed tasks across multiple agents. The [Orchestrator](/personas/04-orchestrator) persona lists decomposition as core skill #1 — breaking goals into agent-sized tasks with clear verification criteria. The key is finding the right granularity: too coarse and agents struggle with ambiguity; too fine and the orchestrator spends more time managing than the agents save.

## Key Aspects

- **Granularity sweet spot** — too coarse and the agent struggles; too fine and you spend more time managing than doing
- **Dependency mapping** — understanding which subtasks depend on others and which can run in parallel
- **Verification points** — building checkpoints between subtasks where human review can catch errors before they compound
- **Progressive delegation** — start with decomposing into subtasks you execute, then gradually delegate subtasks to agents

## Related Content

- [THIS is Why You're Still Slow Even With AI](/videos/hpDC29JdgjI) — the bottleneck is task definition, not execution
- [The Last Hands on the Keyboard](/essays/2026-03-17-01-the-last-hands-on-keyboard) — how decomposition enables agent-driven development
- [The Orchestrator](/personas/04-orchestrator) — persona whose core skill is decomposing work for agents
- [Constraint Encoding](/knowledge/constraint-encoding) — each decomposed task needs encoded constraints to guide agent execution
- [The Builder](/personas/03-builder) — persona learning decomposition as they transition toward orchestration
