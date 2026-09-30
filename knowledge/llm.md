---
title: "Large Language Model (LLM)"
slug: "llm"
description: "The transformer-based text model family at the center of the current AI stack."
tags:
  - llm-fundamentals
related:
  - transformer-architecture
  - context-window
  - token
  - inference
  - fine-tuning
provenance: agent:stub-authoring-v1
created: "2026-05-19"
updated: "2026-09-30"
confidence: medium
---

A large language model is a [transformer](/knowledge/transformer-architecture)-based system trained to predict token sequences at scale, whose emergent abilities — instruction following, reasoning, tool use — turned next-token prediction into the substrate of the agentic stack. The corpus treats LLMs as the "system 2" generalists in production architectures: expensive-capable tiers reserved for hard steps while cheap classifiers handle volume.

The operating model the corpus assumes: models are commodities on a quarterly depreciation clock — every capability is being commoditized downward by efficiency work — so durable value lives in what surrounds them: context curation ([context engineering](/knowledge/context-engineering)), tool access ([tool use](/knowledge/tool-use), [MCP](/knowledge/mcp)), verification ([evals](/knowledge/evals)), and routing economics ([token economics](/knowledge/token-economics)).
