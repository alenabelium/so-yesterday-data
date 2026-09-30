---
title: "AI Governance"
slug: "ai-governance"
description: "The organizational system of rules, permissions and accountability that governs how AI agents may act — the internal counterpart to external regulation."
tags:
  - ai-strategy
  - ethics-safety
related:
  - ai-regulation
  - ai-safety-research
  - evals
  - constraint-encoding
  - permission-gap
provenance: agent:stub-authoring-v1
created: "2026-05-19"
updated: "2026-09-30"
confidence: medium
---

AI governance is the machinery an organization builds so its AI systems act within intent: who may deploy what, with which data, under which permissions, with what review, and who is accountable when it errs. The corpus treats it as the precondition for scaling adoption — the failure-mode literature (stalled pilots, dark code, agent incidents) is uniformly a governance story, and the regulatory wave (EU AI Act, DORA, NIS 2 — see [AI regulation](/knowledge/ai-regulation)) mostly codifies the same requirements with deadlines attached.

Working governance in the corpus has a recognizable shape: scoped [permissions](/knowledge/permission-gap) and blast-radius limits per agent class; [evals](/knowledge/evals) that encode organizational intent as measurable checks; proposal-and-moderation flows for consequential changes; and audit trails that make agent actions reconstructable after the fact. The design principle is to govern *actions* rather than models — the same model is safe inside a sandboxed read-only workflow and unsafe with prod credentials. Governance done well is an accelerant, not a brake: it is what lets an organization hand agents real responsibility.
