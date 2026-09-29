---
title: "Google Spent a Year Stitching MCP, A2A, AG-UI Together. I/O Today."
video_id: zP6TnEiueEc
date: 2026-05-19
url: https://www.youtube.com/watch?v=zP6TnEiueEc
channel: NateBJones
tags:
  - ai-strategy
  - ai-agents
  - productivity
  - ethics-safety
transcript: ../transcripts/2026-05-19-google-spent-a-year-stitching-mcp-a2a-ag-ui-together-io-toda.md
relevant: true
---

# Google Spent a Year Stitching MCP, A2A, AG-UI Together. I/O Today.

## Executive Summary

The video analyzes six emerging agent protocols launched in the last year, categorizing them into a core standard stack and contested layers to help developers build effective agentic systems. It argues that while MCP, A2A, and AGUI form the foundational substrate for tool access, agent coordination, and human control, other protocols like A2UI, AP2, and X42 address specific, narrower use cases such as structured UI rendering and payments. The central thesis is that developers must move beyond model selection to understand how these protocol substrates directly shape the customer experience, security, and workflow reliability of their AI agents.

## Key Points

- MCP, A2A, and AGUI constitute the core agent stack by solving tool discovery, cross-agent delegation, and human-in-the-loop control respectively, while A2UI, AP2, and X42 remain contested or domain-specific layers for UI rendering and payments [00:01:54](https://www.youtube.com/watch?v=zP6TnEiueEc&t=114).
- MCP standardizes tool integration but introduces significant security risks like tool poisoning, requiring developers to implement strict scopes and approval flows rather than treating it as a simple feature toggle [00:03:11](https://www.youtube.com/watch?v=zP6TnEiueEc&t=191).
- A2A enables agents to delegate tasks to specialized agents across boundaries using 'agent cards' as operating contracts, though it adds complexity regarding latency, failure modes, and observability [00:06:26](https://www.youtube.com/watch?v=zP6TnEiueEc&t=386).
- AGUI addresses the 'supervision debt' of long-running agents by providing a control layer for streaming state, approvals, and interruptions, which traditional chat interfaces cannot support [00:08:57](https://www.youtube.com/watch?v=zP6TnEiueEc&t=537).
- Payment protocols like AP2 and X42 are highly contested and opinionated, meaning developers must carefully evaluate how their specific customer geographies and trust requirements align with these substrates [00:13:22](https://www.youtube.com/watch?v=zP6TnEiueEc&t=802).
- Developers should evaluate their agent workflows against six specific questions regarding tool needs, delegation, control, UI, and payments to ensure the chosen protocol stack aligns with the actual customer experience [00:16:40](https://www.youtube.com/watch?v=zP6TnEiueEc&t=1000).
