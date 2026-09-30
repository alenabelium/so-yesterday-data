---
title: "AI Security"
slug: "ai-security"
description: "Defending AI systems and the systems AI touches — adversarial inputs, agent abuse, and the new attack surface agents create."
tags:
  - ethics-safety
  - ai-agents
related:
  - prompt-injection
  - permission-gap
  - evals
  - ai-governance
provenance: agent:stub-authoring-v1
created: "2026-05-19"
updated: "2026-09-30"
confidence: medium
---

AI security is the defensive discipline for the agentic era: prompt-injection and jailbreak resistance, output filtering, permission architecture for agents with real credentials, and supply-chain risks in models and tools. The corpus treats agents as a genuine new attack surface — a system that reads untrusted content and then takes actions ([prompt injection](/knowledge/prompt-injection) is the canonical exploit path), which is why blast-radius scoping and sandboxed contexts are security controls, not just hygiene (see [permission gap](/knowledge/permission-gap)).

The corpus's reference defenses mirror this platform's own architecture: treat content as data never instructions; scope credentials per task; audit-log every agent action; and gate consequential effects on human or automated verification ([evals](/knowledge/evals), [governance](/knowledge/ai-governance)). Security here accelerates adoption — it is what makes handing agents responsibility defensible.
