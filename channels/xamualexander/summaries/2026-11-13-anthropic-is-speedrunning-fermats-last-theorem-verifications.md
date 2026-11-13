---
title: "Anthropic is speedrunning Fermat's Last Theorem verifications now"
video_id: icDkDQiOSX0
date: 2026-11-13
url: https://www.youtube.com/watch?v=icDkDQiOSX0
channel: Dr. Samuel Allen Alexander
tags:
  - ai-agents
  - ai-strategy
  - ai-safety
  - industry-news
transcript: ../transcripts/2026-11-13-anthropic-is-speedrunning-fermats-last-theorem-verifications.md
relevant: true
knowledge: true
highlight: true
---

# Anthropic is speedrunning Fermat's Last Theorem verifications now

## Executive Summary

Anthropic's experiment with 1,000 agents running an early version of Claude Fable 5.2 successfully formalized Fermat's Last Theorem in Lean in 28.7 hours, a dramatic speedup from the 11 days it took in September. The team used only general-purpose tools like Git and SQL, without the specialized ProveToMe platform, and the resulting proof was 1/7th the length of the original. The video highlights the agents' self-organization into teams and a task tree, as well as the layered safety measures (sandboxing, real-time and offline monitoring) that enabled the experiment. The presenter, Dr. Samuel Allen Alexander, discusses the implications for multi-agent scaling, the role of human encouragement, and the potential for future 'speedrunning' of other major mathematical proofs.

## Key Points

- Anthropic's team of 1,000 agents formalized Fermat's Last Theorem in Lean in 28.7 hours, using 1/3 the tokens and producing a proof 1/7th the length of the original September effort. [00:01:15](https://www.youtube.com/watch?v=icDkDQiOSX0&t=75)
- The agents self-organized into crews and a task tree, with the lead assigning statements and helpers splitting work into subtasks, demonstrating emergent coordination without human steering. [00:18:38](https://www.youtube.com/watch?v=icDkDQiOSX0&t=1118)
- Safety was enforced via sandboxing, a real-time classifier, and an offline monitor, which blocked any attempts to escape or tamper with monitoring, ensuring the agents couldn't access the internet or download the existing proof. [00:12:49](https://www.youtube.com/watch?v=icDkDQiOSX0&t=769)
- The experiment suggests that multi-agent teams can tackle long-horizon problems, but AI's estimates of task difficulty remain unreliable, as helpers initially judged 47 of 60 statements infeasible yet proved most of them. [00:31:11](https://www.youtube.com/watch?v=icDkDQiOSX0&t=1871)
