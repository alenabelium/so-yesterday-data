---
title: "Sniff-Checking"
slug: "sniff-checking"
description: "The meta-skill of rapidly evaluating AI-generated output for correctness without re-deriving it from scratch."
tags:
  - productivity
  - coding
related:
  - rejection-competency
  - agent-orchestration
  - specification-quality
  - hallucination
sources:
  - {type: "video", id: "-bQcWs1Z9a0", date: "2026-02-20", title: "$1,000 a Day in AI Costs. Three Engineers. No Writing Code. No Code Review. But More Output."}
  - {type: "video", id: "-FhtPUkXKO4", date: "2026-03-10", title: "Stop accepting AI output that \"looks right.\" The other 17% is everything and nobody is ready for it."}
  - {type: "essay", slug: "2026-03-17-01-the-last-hands-on-keyboard", date: "2026-03-17", title: "The Last Hands on the Keyboard: How Software Development Became Agent Orchestration"}
created: "2026-03-19"
updated: "2026-03-19"
confidence: high
---

Sniff-checking is the skill of quickly evaluating whether AI-generated output is correct without re-doing the work yourself. As [AI agents](/knowledge/ai-agents) generate code, analysis, and content faster than humans can review it line-by-line, the ability to rapidly assess quality — catching structural errors, logical inconsistencies, and domain violations at a glance — becomes the most valuable competency in [agent orchestration](/knowledge/agent-orchestration).

The term captures a specific skill gap: agents generate output at the speed of tokens, but orchestrators must evaluate that output fast enough to keep the pipeline moving. Traditional code review assumes the reviewer could have written the code; sniff-checking assumes the reviewer's value is pattern recognition and domain judgment, not implementation ability. It's what separates effective orchestrators from those who become bottlenecks in their own workflows.

The [Orchestrator](/personas/04-orchestrator) persona identifies sniff-checking as one of five core skills, alongside decomposition, [constraint encoding](/knowledge/constraint-encoding), [blast radius management](/knowledge/blast-radius), and recovery design. The [Displaced Expert](/personas/05-displaced-expert) has a natural advantage here — their deep domain knowledge makes them excellent sniff-checkers, even if they didn't write the code themselves.

## Key Aspects

- **Pattern recognition over line-by-line review** — effective sniff-checking relies on recognizing structural patterns (correct error handling, proper data flow, sensible architecture) rather than verifying every line
- **Domain-informed shortcuts** — knowing what "wrong" looks like in your domain lets you spot errors that general-purpose review would miss
- **Calibrated confidence** — knowing when a sniff-check is sufficient vs. when deep review is needed, based on the [blast radius](/knowledge/blast-radius) of the change
- **Speed as the bottleneck** — agents generate faster than you review; the evaluation bottleneck determines throughput for the entire orchestration pipeline

## Related Content

- [$1,000 a Day in AI Costs. Three Engineers.](/videos/-bQcWs1Z9a0) — sniff-checking at production scale
- [Stop accepting AI output that "looks right"](/videos/-FhtPUkXKO4) — the danger of insufficient evaluation
- [The Last Hands on the Keyboard](/essays/2026-03-17-01-the-last-hands-on-keyboard) — sniff-checking as one of five critical orchestrator skills
- [The Orchestrator](/personas/04-orchestrator) — persona for whom sniff-checking is a core competency
- [The Displaced Expert](/personas/05-displaced-expert) — persona whose domain knowledge makes them natural sniff-checkers
