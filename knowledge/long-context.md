---
title: "Long Context"
slug: "long-context"
description: "Very large context windows — what they actually change, and what they don't."
tags:
  - llm-fundamentals
related:
  - context-window
  - context-engineering
  - rag
provenance: agent:stub-authoring-v1
created: "2026-05-19"
updated: "2026-09-30"
confidence: medium
---

Long context — windows of hundreds of thousands to millions of tokens — is marketed as "whole codebase / whole book in one prompt." The corpus's measured take: it genuinely changes retrieval-shaped tasks (reading, comparing, locating) and simplifies architectures that existed to route around small windows; it does NOT obsolete curation, because attention quality degrades with clutter — the "lost in the middle" effect — and cost scales linearly with input.

Production guidance that emerges: long context and [RAG](/knowledge/rag) converge — retrieval selects what deserves the window, the window holds it well; long sessions need compaction regardless (see [context window management](/knowledge/context-window-management)); and per-token economics still argue for routing big inputs to cheap tiers (see [model efficiency](/knowledge/model-efficiency)).
