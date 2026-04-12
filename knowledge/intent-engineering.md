---
title: "Intent Engineering"
slug: "intent-engineering"
description: "Expressing high-level goals and intent in ways AI systems can reliably interpret and execute."
tags:
  - ai-strategy
  - prompting
related:
  - context-engineering
  - domain-translation
created: "2026-03-19"
updated: "2026-03-19"
confidence: high
---

Intent engineering is the emerging discipline of expressing what you want to achieve — your goals, constraints, and success criteria — in a way that AI systems can reliably interpret and execute. It sits above [prompt engineering](/knowledge/prompt-engineering) and [context engineering](/knowledge/context-engineering) in the abstraction hierarchy: instead of crafting specific prompts, you define outcomes and let AI figure out the steps.

As AI agents become more autonomous, the skill shifts from telling AI *how* to do something to telling it *what* you want done and *why*. Intent engineering requires clarity of thought about your actual goals, not just the immediate task. It draws on [domain translation](/knowledge/domain-translation) to express domain-specific intent in AI-accessible terms. The [Domain Translator](/personas/06-domain-translator) persona takes intent engineering furthest — moving beyond prompts to machine-readable goal structures with delegation frameworks, value trade-offs, and escalation boundaries. Their insight: encoding organizational *intent* (not just what AI needs to know, but what AI needs to *want*) as machine-readable parameters is the highest form of intent engineering.

## Key Aspects

- **Outcome over process** — define what success looks like rather than prescribing each step
- **Constraint specification** — clearly articulating what the AI should NOT do is as important as what it should do
- **Ambiguity elimination** — natural language is inherently ambiguous; intent engineering is the skill of reducing that ambiguity
- **Evolution from prompting** — as models improve, the emphasis shifts from prompt tricks to clear intent expression

## Related Content

- ['Prompting' Just Split Into 4 Skills](/videos/BpibZSMGtdY) — intent engineering as one of the four successor skills to prompting
- [Prompt Engineering Is Dead. Context Engineering Is Dying.](/videos/QWzLPn164w0) — what comes after prompt and context engineering
- [The Orchestrator](/personas/04-orchestrator) — persona focused on expressing intent for agent execution
- [The Domain Translator](/personas/06-domain-translator) — persona building intent specifications as machine-readable goal structures
- [Constraint Encoding](/knowledge/constraint-encoding) — the mechanism for encoding intent as persistent AI instructions
