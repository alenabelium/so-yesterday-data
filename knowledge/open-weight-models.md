---
title: "Open-Weight Models"
slug: "open-weight-models"
description: "Models whose trained parameters are published for download and local deployment — distinct from open-source code, and the enabler of sovereign, cost-controlled AI."
tags:
  - llm-fundamentals
  - ai-tools
related:
  - open-source-ai
  - open-source
  - hugging-face
  - model-distillation
  - local-inference
  - inference
provenance: agent:stub-authoring-v1
created: "2026-05-19"
updated: "2026-09-30"
confidence: medium
---

Open-weight models are AI models whose parameters can be downloaded, inspected, fine-tuned and served by anyone — Qwen, DeepSeek, Llama and Mistral families being the corpus's recurring examples. The distinction from "open source" proper matters: open weights usually arrive without training code or data, but they still transfer the two properties buyers actually need — the ability to run the model inside your own perimeter ([local inference](/knowledge/local-inference)) and the ability to specialize it ([fine-tuning](/knowledge/fine-tuning), [distillation](/knowledge/model-distillation)).

Strategically, open weights are the price-setter for capability: whatever a frontier lab shipped a year ago is now roughly free to self-host, which is why build-vs-rent calculations in the corpus always include a "this will commoditize" line. For regulated and sovereignty-sensitive deployments they are the only compliant substrate; for cost-sensitive pipelines they anchor the cheap tier of a two-tier routing stack. The trade is honest: open weights trail the frontier in peak capability and the operator owns ops, safety patching and evals.
