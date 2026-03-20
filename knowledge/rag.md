---
title: "Retrieval Augmented Generation (RAG)"
slug: "rag"
description: "A technique that enhances LLM responses by retrieving relevant documents from external sources before generating output."
tags:
  - llm-fundamentals
  - ai-tools
related:
  - context-engineering
  - second-brain
  - context-window
  - fine-tuning
  - hallucination
created: "2026-03-19"
updated: "2026-03-19"
---

Retrieval Augmented Generation (RAG) is a technique where an AI system retrieves relevant documents or data from an external knowledge base before generating a response. Instead of relying solely on what the model learned during training, RAG gives the model access to current, specific, and verifiable information at the moment it needs it.

RAG is the technical foundation behind several concepts in the knowledge base. [Building a second brain](/knowledge/second-brain) is essentially creating a personal RAG system. [Context engineering](/knowledge/context-engineering) often involves deciding what to retrieve and how to structure it in the [context window](/knowledge/context-window). RAG also directly addresses [hallucination](/knowledge/hallucination) — by grounding responses in retrieved documents, the model is less likely to fabricate information.

The so-yesterday.ai knowledge base itself functions as a RAG-ready corpus: structured markdown files with YAML frontmatter, tags, and cross-references that an AI system can search, retrieve, and synthesize.

## Key Aspects

- **Retrieve → Augment → Generate** — the three-step process: find relevant documents, add them to the model's context, then generate a grounded response
- **vs. fine-tuning** — RAG keeps knowledge external and updatable; [fine-tuning](/knowledge/fine-tuning) embeds it in the model. RAG is better for knowledge that changes frequently
- **Chunking and embedding** — documents must be split into chunks and converted to numerical representations (embeddings) for efficient retrieval
- **Context window as bottleneck** — retrieved documents consume [context window](/knowledge/context-window) space; retrieving too much can be as harmful as retrieving too little

## Related Content

- [One Simple System Gave All My AI Tools a Memory](/videos/japT66frdhM) — building RAG-like memory systems
- [Why 2026 Is the Year to Build a Second Brain](/videos/0TpON5T-Sw4) — personal RAG systems
- [You Don't Need SaaS. The $0.10 System](/videos/2JiMmye2ezg) — lightweight RAG alternatives
- [The Practitioner](/personas/02-practitioner) — persona learning to assemble context effectively
