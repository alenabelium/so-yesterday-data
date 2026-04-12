---
title: "AI Agents"
slug: "ai-agents"
description: "Autonomous AI systems that can plan, use tools, and take actions to accomplish goals."
tags:
  - ai-agents
  - llm-fundamentals
related:
  - agent-orchestration
  - tool-use
  - mcp
  - emergent-behavior
  - evals
created: "2026-03-19"
updated: "2026-03-21"
confidence: high
---

AI agents are systems built on large language models that go beyond simple question-answering to autonomously plan, reason, and execute multi-step tasks. Unlike chatbots that respond to individual prompts, agents maintain context across actions, use external tools, and make decisions about what to do next — often without human intervention at each step.

The rise of AI agents represents a fundamental shift in how we interact with AI. Rather than crafting the perfect prompt for a single response, users define goals and constraints, then let the agent figure out the steps. This has enormous implications for productivity, software development, and the future of work — agents can browse the web, write and execute code, manage files, and coordinate with other agents.

A useful framework for understanding personal agents identifies three essential primitives: memory (a persistent database via [MCP](/knowledge/mcp)), proactivity (scheduled action via commands like `/loop`), and tools (API connections to external services). Remove any one and the system degrades — without memory it's a chatbot, without proactivity it's a passive assistant, without tools it's a brain without hands.

The challenge with AI agents is managing their autonomy. As agents become more capable, questions of safety, oversight, and [blast radius management](/knowledge/blast-radius) become critical. The skill of working with agents is rapidly evolving from prompt engineering to [agent orchestration](/knowledge/agent-orchestration) — managing fleets of agents rather than writing code yourself.

## Key Aspects

- **Autonomy spectrum** — agents range from simple tool-calling assistants to fully autonomous systems that plan and execute complex workflows without human approval at each step
- **Tool use** — agents extend LLM capabilities by calling external tools: APIs, code execution, file systems, browsers ([Tool Use](/knowledge/tool-use))
- **Planning and reasoning** — effective agents decompose complex goals into subtasks, a skill covered in [Task Decomposition](/knowledge/task-decomposition)
- **Memory and context** — agents maintain state across interactions, building up knowledge that informs future actions

## Related Content

- [OpenClaw Agents Are Hiring Each Other](/videos/WEEKBlQfGt8) — demonstrates emergent agent behaviors
- [Google Just Proved More Agents Can Make Things WORSE](/videos/2EXyj_fHU48) — the limits of multi-agent systems
- [4 AI Labs Built the Same System Without Talking to Each Other](/videos/LO0Ws-l6brg) — convergent evolution in agent architectures
- [The Last Hands on the Keyboard](/essays/2026-03-17-01-the-last-hands-on-keyboard) — how development is shifting to agent management
- [The Orchestrator](/personas/04-orchestrator) — the persona focused on managing agent fleets
- [The Builder](/personas/03-builder) — persona transitioning from building to agent supervision
- [The Solo Operator](/personas/07-solo-operator) — persona using agents as their AI-native operations team
- [Daily Digest — March 18, 2026](/digests/2026-03-18) — agent supervision as essential skill
- [Anthropic Just Gave Your AI Agent the One Thing OpenClaw Has](/videos/vqnAOV8NMZ4) — the three-primitive agent framework
