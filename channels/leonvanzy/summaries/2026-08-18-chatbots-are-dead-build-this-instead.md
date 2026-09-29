---
title: "Chatbots Are Dead. Build This Instead"
video_id: epGDGyTZs5Y
date: 2026-08-18
url: https://www.youtube.com/watch?v=epGDGyTZs5Y
channel: Leon van Zyl
tags:
  - ai-agents
  - coding
  - productivity
  - tutorials
transcript: ../transcripts/2026-08-18-chatbots-are-dead-build-this-instead.md
relevant: true
---

# Chatbots Are Dead. Build This Instead

## Executive Summary

The video argues that simple chatbots are obsolete and advocates for building autonomous AI agents capable of executing complex, multi-step workflows. Using a practical example of an enterprise agreement management system, the presenter demonstrates how to construct an agent that creates, sends, and tracks Non-Disclosure Agreements (NDAs) without manual intervention. The tutorial details the technical architecture involving Claude models, DocuSign's MCP server for tool access, and specific prompting strategies to ensure secure and accurate automation.

## Key Points

- The core philosophy shifts from passive chatbots to active agents defined by three components: the model (brain), the harness (SDK), and tools/permissions layer, demonstrated through an NDA workflow where the agent autonomously drafts, sends, and tracks signatures [00:01:11](https://www.youtube.com/watch?v=epGDGyTZs5Y&t=71).
- Building the application involves using Claude Code with specific skills like 'start an app' to enforce tech stack guardrails and Playwright MCP for automated end-to-end UI testing during development [00:07:30](https://www.youtube.com/watch?v=epGDGyTZs5Y&t=450).
- Integration with DocuSign is achieved via its beta MCP server, requiring setup of developer credentials, redirect URIs, and the creation of digital templates to allow the agent to execute real-world document workflows [00:12:42](https://www.youtube.com/watch?v=epGDGyTZs5Y&t=762).
- The final implementation allows users to interact via natural language prompts, where the agent confirms details with the user before acting, ensuring human-in-the-loop safety while automating the entire agreement lifecycle [00:21:26](https://www.youtube.com/watch?v=epGDGyTZs5Y&t=1286). [MM:SS](https://www.youtube.com/watch?v=epGDGyTZs5Y&t=SECONDS)
