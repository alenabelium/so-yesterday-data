---
title: "Agentic Coding"
slug: "agentic-coding"
description: "Software development where AI agents execute against human-written specifications and tests — the disciplined successor to vibe coding."
tags:
  - coding
  - ai-agents
related:
  - vibe-coding
  - claude-code
  - codex
  - specification-quality
  - evals
  - dark-code
provenance: agent:stub-authoring-v1
created: "2026-05-19"
updated: "2026-09-30"
confidence: medium
---

Agentic coding is the mature form of AI-assisted development: instead of prompting for snippets, engineers write specifications, scaffold tests, and let agents iterate against them inside a bounded workspace. The corpus frames it as the shift from generation to delegation — the human owns the what and the verification, the agent owns the typing. [Vibe coding](/knowledge/vibe-coding) is the casual, prototype-grade version; agentic coding is the production discipline that grows out of it.

The failure modes define the practice: agents produce plausible code that misses edge cases ([the 70% problem](/knowledge/the-70-percent-problem)), accumulate unreviewed "dark code", and stretch [blast radius](/knowledge/blast-radius) when given write access without gates. The countermeasures are the corpus's densest cluster: [specification quality](/knowledge/specification-quality), [evals](/knowledge/evals), scoped permissions, and regeneration-from-spec as the recoverability test. Teams that treat the agent as a junior engineer with infinite stamina — reviewed, tested, promoted gradually — ship weekly; teams that treat it as an oracle stall.
