---
title: "Model Efficiency"
slug: "model-efficiency"
description: "The discipline of getting equal capability from less compute — distillation, quantization, routing and architecture choices that set the price floor of AI workloads."
tags:
  - llm-fundamentals
  - ai-infrastructure
related:
  - model-distillation
  - inference
  - token-economics
  - scaling-laws
  - open-weight-models
provenance: agent:stub-authoring-v1
created: "2026-05-19"
updated: "2026-09-30"
confidence: medium
---

Model efficiency is the engineering layer that converts capability into affordable capability: smaller models trained to match larger ones ([distillation](/knowledge/model-distillation)), quantized weights that trade negligible accuracy for multiples of throughput, mixture-of-experts architectures that activate only the parameters a token needs, and routing schemes that reserve expensive models for the requests that demonstrably require them. In the corpus it is the quiet constant under the model-release news: every efficiency generation moves last year's frontier quality down the cost curve by an order of magnitude.

Efficiency is also the strategic variable in the two-tier stack that now dominates production designs: cheap "system-1" tier models handle classification, routing and high-volume passes; frontier models are reserved for hard reasoning (see [token economics](/knowledge/token-economics)). The second-order effect the platform tracks is the "so yesterday" one — efficiency gains commoditize capability faster than capability itself advances, so workflows built around a *specific* model's cost or latency profile expire on a quarterly clock. Design for the routing layer, not the model.
