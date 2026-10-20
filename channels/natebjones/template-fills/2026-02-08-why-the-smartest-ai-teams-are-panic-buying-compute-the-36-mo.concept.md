---
video_id: pSgy2P2q790
template_id: concept
template_version: 1
source_summary: ../summaries/2026-02-08-why-the-smartest-ai-teams-are-panic-buying-compute-the-36-mo.md
source_transcript: ../transcripts/2026-02-08-why-the-smartest-ai-teams-are-panic-buying-compute-the-36-mo.md
source_summary_hash: sha256:83e5f433b784f301606452fbde785bbbcd30de4cf220efcdcc8f087069523fa3
source_transcript_hash: sha256:e385dcf0408a7116e58e3daab432e9bd2db4450b3bd4c5a7736095a9993404e5
fill_id: 8be0de40-673d-4864-b001-a9bd9f710c36
published_at: '2026-10-20T01:12:24.695191'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

A structural crisis is emerging in global technology infrastructure: demand for inference compute is growing exponentially while supply is physically constrained through 2028. DRAM prices are surging, fabs are fully allocated, and hyperscalers are hoarding capacity. Enterprises must secure capacity now, build routing layers, and treat hardware as a consumable to survive.

## The argument

### Demand is exponential and uncapped
- **Anchor Timestamps**: ['00:01:02']
- **Claim**: Enterprise AI consumption grows at least 10x annually, driven by per-worker usage and agentic systems. A single agentic workflow can consume more tokens in an hour than a human generates in a month. There is no demand limit for intelligence.
- **Role**: definition

### Supply is physically constrained through 2028
- **Anchor Timestamps**: ['00:08:04']
- **Claim**: AI inference is memory-bound. DRAM prices have risen 50%+ and are projected to rise another 55-60% in Q1 2026. New fabs take 3-4 years and $20B to build. TSMC's advanced nodes are fully allocated, and HBM is sold out. No near-term supply response exists.
- **Role**: evidence

### Hyperscalers are not neutral suppliers
- **Anchor Timestamps**: ['00:12:53']
- **Claim**: AWS, Azure, and Google Cloud compete directly with their enterprise customers. When compute is scarce, every GPU allocated to an enterprise is a GPU not available for their own AI products. They will choose their own products, making them unreliable partners in this crisis.
- **Role**: counter

### Traditional planning frameworks are broken
- **Anchor Timestamps**: ['00:18:41']
- **Claim**: Capex models, depreciation schedules, and multi-year procurement cycles assume predictable demand and available supply. Neither holds. A 4-year depreciation schedule on AI workstations becomes obsolete in 2 years as agentic workloads demand 10x more tokens.
- **Role**: evidence

### The playbook: secure, route, consume, diversify
- **Anchor Timestamps**: ['00:21:01']
- **Claim**: Sharp CTOs secure capacity before they need it, build a routing layer for model and provider optionality, treat hardware as a consumable with 2-year depreciation, and invest in efficiency as a competitive advantage. Diversify across the stack to reduce dependence on any single player.
- **Role**: synthesis

## Evidence and caveats

Google processed 1.3 quadrillion tokens per month, a 130x increase in just over a year, serving as a leading indicator for enterprise demand. DRAM prices spiked 300% during the 2016 shortage, and GPU prices doubled during the crypto mining boom, showing the potential for severe spikes. Notion disclosed AI costs consume 10 percentage points of its 90% gross margin. DeepSeek's work on engram reduces token usage for factual lookups, and quantization can match larger model performance on specific tasks. Caveats: The speaker notes that pricing projections vary (47% vs 55% DRAM increase) and that committed use agreements can become traps if predictions are off. The speaker also admits that large-scale leasing has not been successfully executed by enterprises yet.

## Concepts surfaced

[[agentic-systems]] · [[inference-compute]] · [[high-bandwidth-memory]] · [[gpu-allocation]] · [[hyperscaler-conflict]] · [[routing-layer]]
