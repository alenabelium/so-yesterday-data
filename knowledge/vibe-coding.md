---
title: "Vibe Coding"
slug: "vibe-coding"
description: "A development approach where developers describe intent in natural language and let AI write the code."
tags:
  - coding
  - ai-tools
related:
  - specification-quality
  - ai-coding-levels
sources:
  - {type: "video", id: "sLz4mAyykeE", date: "2026-02-07", title: "90% of People Fail at Vibe Coding. Here's the Actual Reason: You're Skipping the Hard Part."}
  - {type: "video", id: "2ghhiPLg-jg", date: "2026-02-28", title: "My 10-Year-Old Vibe Codes. She Also Does Math by Hand. Why That's the Only Strategy That Works."}
  - {type: "video", id: "bDcgHzCBgmQ", date: "2026-02-18", title: "The 5 Levels of AI Coding (Why Most of You Won't Make It Past Level 2)"}
  - {type: "digest", date: "2026-03-17", title: "Daily Digest — March 17, 2026"}
  - {type: "essay", slug: "2026-03-13-01-start-with-ai-today", date: "2026-03-13", title: "Stop Overthinking It: A Working Professional's No-Nonsense Guide to Starting With AI Today"}
created: "2026-03-19"
updated: "2026-03-19"
confidence: high
---

Vibe coding is a development approach where programmers describe what they want in natural language and let AI generate the code. Coined in early 2026, the term captures a spectrum — from casual prototyping where you barely look at the generated code, to disciplined specification-driven development where the "vibe" is a carefully crafted spec.

The appeal of vibe coding is speed: what took hours of manual coding can be generated in minutes. The risk is that 90% of practitioners fail because they skip the hard part — [specification quality](/knowledge/specification-quality). Without clear specs, vibe coding produces code that looks right but breaks in production. The skill progression from casual vibe coding to professional AI-assisted development is mapped in [The 5 Levels of AI Coding](/knowledge/ai-coding-levels). The [Builder](/personas/03-builder) persona navigates this progression daily, armed with five core practices: save points (git commit before every change), fresh starts (know when context is exhausted), standing orders (persistent rules files), small bets (limit blast radius per change), and corner questions (proactively handle errors, security, scale).

## Key Aspects

- **Speed vs. reliability tradeoff** — vibe coding is fastest for prototypes and [disposable software](/knowledge/disposable-software), but requires more discipline for production code
- **The specification bottleneck** — the quality ceiling of vibe-coded output is set by the quality of the input specification
- **Review burden** — as AI writes more code, the human role shifts from writing to reviewing, requiring different skills
- **Accessibility** — vibe coding lowers the barrier to building software, enabling non-programmers to create functional tools
- **Security awareness** — approximately 10% of vibe-coded applications contain vulnerabilities (exposed databases, visible API keys, missing validation), making security discipline essential even in rapid prototyping

## Related Content

- [90% of People Fail at Vibe Coding](/videos/sLz4mAyykeE) — why specification is the hard part
- [My 10-Year-Old Vibe Codes](/videos/2ghhiPLg-jg) — vibe coding as an accessible entry point
- [The 5 Levels of AI Coding](/videos/bDcgHzCBgmQ) — the progression from vibe coding to agent orchestration
- [The Builder](/personas/03-builder) — persona shipping software with AI, from vibe coding to production
- [Daily Digest — March 17, 2026](/digests/2026-03-17) — vibe-coding-to-agent-management skill gap
- [Stop Overthinking It](/essays/2026-03-13-01-start-with-ai-today) — practical guide including AI tool ecosystem for builders
