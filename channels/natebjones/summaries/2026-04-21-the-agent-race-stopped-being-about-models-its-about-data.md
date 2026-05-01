---
title: "The Agent Race Stopped Being About Models. It's About Data."
video_id: tJB_8mfRgCo
date: 2026-04-21
url: https://www.youtube.com/watch?v=tJB_8mfRgCo
channel: NateBJones
tags:
  - ai-tools
  - llm-fundamentals
  - coding
  - opinion
transcript: ../transcripts/2026-04-21-the-agent-race-stopped-being-about-models-its-about-data.md
---

# The Agent Race Stopped Being About Models. It's About Data.

## Executive Summary

Nate Jones delivers a comprehensive review of Claude Opus 4.7, testing it head-to-head against GPT 5.4 on a realistic 465-file data migration benchmark. While 4.7 shows genuine improvements in agentic persistence and knowledge work (scoring highest on GDP-Val), it introduces a new tokenizer that maps the same text to up to 35% more tokens, effectively raising costs. The model is more literal, more combative, and removes developer controls like temperature and thinking budgets. Jones also reviews Claude Design, which cost him $42 in a single session due to correction loops, and frames the release as a strategic bridge before Anthropic's next frontier model Mythos, amid fierce competition with OpenAI's upcoming releases.

## Key Points

- Opus 4.7 fixes the premature task abandonment problem of 4.6, with teams reporting 10-15% lifts in task success and significantly fewer infinite loops, but it regressed on web research (Browse Comp dropped from 83 to 79) and trails GPT 5.4 on terminal tasks by six points. [02:14](https://www.youtube.com/watch?v=tJB_8mfRgCo&t=134)
- In a head-to-head 465-file data migration test, Opus 4.7 built a shippable front-end UI but hallucinated processing a file it never touched and missed obvious fake customers (Mickey Mouse, Test Customer), while GPT 5.4 produced a superior 7,200-line merge log with per-row source citations. [07:05](https://www.youtube.com/watch?v=tJB_8mfRgCo&t=425)
- The new tokenizer increases input tokens by up to 35% for the same text, adaptive thinking removes user control over reasoning depth in chat, and temperature/top-P/top-K parameters are gone entirely -- making 4.7 effectively more expensive while giving developers fewer levers to manage cost and behavior. [33:43](https://www.youtube.com/watch?v=tJB_8mfRgCo&t=2023)
