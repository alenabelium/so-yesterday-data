---
title: "Mixture of Experts"
slug: "mixture-of-experts"
description: "Sparsely-activated architectures that route each token to a subset of specialist sub-networks — capability with a fraction of the compute."
tags:
  - llm-fundamentals
related:
  - model-efficiency
  - inference
  - transformer-architecture
provenance: agent:stub-authoring-v1
created: "2026-05-19"
updated: "2026-09-30"
confidence: medium
---

Mixture-of-experts (MoE) architectures embed many specialist sub-networks in one model and activate only a few per token, decoupling total parameters (knowledge capacity) from active parameters (compute cost). The corpus tracks MoE as the architectural workhorse of the efficiency curve — the reason frontier-class capability keeps arriving at falling per-token prices (see [model efficiency](/knowledge/model-efficiency), [inference](/knowledge/inference) economics).

The practitioner takeaways: MoE changes capacity planning — memory footprint scales with total parameters while throughput scales with active ones — and it underwrites the two-tier routing stacks that reserve dense reasoning models for hard steps. As with all efficiency gains, the second-order effect is the platform's core dynamic: capabilities built on MoE price advantages commoditize on a quarterly clock.
