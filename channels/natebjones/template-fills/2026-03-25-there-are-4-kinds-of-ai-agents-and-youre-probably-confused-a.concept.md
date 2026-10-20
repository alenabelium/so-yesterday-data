---
video_id: YpPcDHc3e9U
template_id: concept
template_version: 1
source_summary: ../summaries/2026-03-25-there-are-4-kinds-of-ai-agents-and-youre-probably-confused-a.md
source_transcript: ../transcripts/2026-03-25-there-are-4-kinds-of-ai-agents-and-youre-probably-confused-a.md
source_summary_hash: sha256:ce2a576790d6017f5189bfcc80ccb355a068fbec3819bbddde15793a376f4bf7
source_transcript_hash: sha256:e373c5f76cda28fb9bc08d5a49f7198c439bde66d5094a5e8c2ea7be516d74a8
fill_id: 79d71192-d83b-4ac5-8cc0-59052be50ddc
published_at: '2026-10-20T00:36:23.086445'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

The term 'AI agent' hides at least four distinct species: coding harnesses, dark factories, auto research, and orchestration frameworks. Each is built for a different job—from individual coding tasks to fully autonomous software generation to metric optimization. Misidentifying the species leads to using the wrong architecture and failing at the task.

## The argument

### Define the Four Species
- **Anchor Timestamps**: ['00:00:57']
- **Claim**: Sophisticated agents diverge into four types: coding harnesses (single LLM agent for individual coding), dark factories (fully autonomous systems from spec to software), auto research (optimizing for a metric via hill climbing), and orchestration frameworks (multiple LLMs with specialized roles handing off work). These are distinct species, not variations of one idea.
- **Role**: definition

### Coding Harnesses Scale from Individual to Project
- **Anchor Timestamps**: ['00:06:35']
- **Claim**: Coding harnesses start as a single agent replacing a developer, but at project scale they evolve into a multi-agent system where a planner agent coordinates short-running executor agents. This shift from human-managed to agent-managed is key for large projects, as seen with Cursor's browser and compiler builds.
- **Role**: evidence

### Dark Factories Remove the Human from the Middle
- **Anchor Timestamps**: ['13:56']
- **Claim**: Dark factories are fully autonomous systems that take a spec and produce software, with humans only at the start (design, spec) and end (eval, accountability). The goal is to eliminate human bottlenecks in the middle of a fast agentic process, iterating automatically until the software passes an eval.
- **Role**: definition

### Auto Research Optimizes Metrics, Not Software
- **Anchor Timestamps**: ['00:19:19']
- **Claim**: Auto research is a descendant of classical machine learning, focused on hill-climbing toward a metric (e.g., conversion rate, runtime performance, model tuning). It is not about producing software but about using LLMs to run experiments and optimize a target, as demonstrated by Toby's Shopify framework and Karpathy's recent work.
- **Role**: evidence

### Orchestration Handles Specialized Roles and Handoffs
- **Anchor Timestamps**: ['00:22:38']
- **Claim**: Orchestration frameworks like LangGraph manage multiple LLMs with specialized roles (e.g., researcher, writer, finance agent) and coordinate handoffs. This is distinct from coding harnesses because the goal is workflow routing, not a unified coding project. It requires significant human involvement at the joints and is only worth it at scale.
- **Role**: synthesis

## Evidence and caveats

The speaker cites real-world examples: Karpathy's 16-hour coding harness runs, Peter Steinberger's multiple Codex agents for OpenClaw, Cursor's multi-agent project harnesses (with a note that they tried three levels of management and it failed—simple scales better), Toby's optimization of Liquid for Shopify, and Karpathy's auto research package for LLM tuning. Caveats: the speaker admits blur between species (e.g., project harnesses vs. dark factories), notes that enterprises often add human review at the end for accountability (citing Amazon's recent AI incidents), and warns against using auto research for software building or coding harnesses for novel writing. The speaker also emphasizes that orchestration is heavy and only worth it for large-scale problems (e.g., 10,000+ tickets).

## Concepts surfaced

[[ai-agents]] · [[coding-harness]] · [[dark-factory]] · [[auto-research]] · [[orchestration-framework]] · [[llm-tools-loop]]
