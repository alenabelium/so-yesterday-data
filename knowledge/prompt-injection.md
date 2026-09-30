---
title: "Prompt Injection"
slug: "prompt-injection"
description: "The attack where untrusted content carries instructions that hijack an agent — the defining security problem of the agentic stack."
tags:
  - ethics-safety
  - ai-agents
related:
  - ai-security
  - permission-gap
  - evals
provenance: agent:stub-authoring-v1
created: "2026-05-19"
updated: "2026-09-30"
confidence: medium
---

Prompt injection is the exploit native to LLM systems: instructions hidden in content the agent legitimately reads — web pages, documents, tool results — that the model follows as if they were the operator's. The corpus treats it as the SQL-injection of the agentic era, unsolved at the model layer and load-bearing for every architecture where agents consume untrusted input and then act (see [AI security](/knowledge/ai-security)).

The defense-in-depth doctrine the corpus converges on — and this platform implements — is structural, not prompt-based: content is data, never instructions (enforced by system design); credentials scoped per task so a hijacked agent's [blast radius](/knowledge/blast-radius) is small; consequential actions gated on verification; tool-permission separation so a content-fed agent literally lacks the tools to act on injected instructions ([permission gap](/knowledge/permission-gap)); and audit trails for post-hoc detection.
