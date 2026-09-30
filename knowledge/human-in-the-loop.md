---
title: "Human-in-the-Loop"
slug: "human-in-the-loop"
description: "Workflow designs where human judgment gates consequential AI actions — the accountability pattern that makes autonomous systems deployable."
tags:
  - ai-strategy
  - ethics-safety
related:
  - evals
  - ai-governance
  - three-layers-of-work
  - the-70-percent-problem
  - constraint-encoding
provenance: agent:stub-authoring-v1
created: "2026-05-19"
updated: "2026-09-30"
confidence: medium
---

Human-in-the-loop (HITL) is the architectural pattern in which AI drafts, proposes, or executes within bounds, and humans decide at defined checkpoints. The corpus treats it not as a temporary crutch but as the durable division of labor: agents supply tireless execution ([the 70%](/knowledge/the-70-percent-problem)), humans supply authority, accountability and taste (see [three layers of work](/knowledge/three-layers-of-work)). Regulatory frameworks hard-code the same intuition — consequential decisions need an accountable human or equivalent guarantees.

The design space is richer than "human reviews everything": gating by blast radius, sampling-based review with escalation, proposal queues (agents file structured changes, moderators accept), and specification-time control where humans encode intent once and verify outcomes continuously. This platform itself is a reference implementation — its Cortex agents never publish directly; everything lands in a moderator queue with an audit trail. The anti-pattern is equally well documented: rubber-stamp review, where the human becomes the bottleneck that either stalls the pipeline or gets automated around by social pressure.
