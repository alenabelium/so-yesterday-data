---
title: "Claude Code Can't See These Bugs. Fiddler MCP Can"
video_id: P4JSc8TYo4I
date: 2026-11-24
url: https://www.youtube.com/watch?v=P4JSc8TYo4I
channel: Leon van Zyl
tags:
  - ai-tools
  - ai-agents
  - tutorials
  - productivity
transcript: ../transcripts/2026-11-24-claude-code-cant-see-these-bugs-fiddler-mcp-can.md
relevant: true
---

# Claude Code Can't See These Bugs. Fiddler MCP Can

## Executive Summary

This video demonstrates how Fiddler Everywhere, an HTTP traffic inspection tool, can be integrated with Claude Code via MCP to debug issues that coding agents cannot see by analyzing code alone. The presenter shows how to configure Fiddler MCP, use it to identify a missing 'Bearer' prefix in an authorization header, and simulate rate limiting and slow responses to test application resilience. The video emphasizes the importance of proactive debugging and testing for responsible AI-assisted development.

## Key Points

- Fiddler Everywhere records all HTTP traffic between your app and external services, revealing hidden bugs like incorrect headers or expired API keys that code analysis misses. [00:02:12](https://www.youtube.com/watch?v=P4JSc8TYo4I&t=132)
- Fiddler MCP connects to Claude Code, allowing the agent to inspect live traffic, edit and resend requests to test fixes, and create rules to simulate failures like rate limits or slow responses. [00:03:31](https://www.youtube.com/watch?v=P4JSc8TYo4I&t=211)
- By default, Fiddler masks sensitive data (API keys, headers) before sending to the agent, but you can disable scrubbing to expose the root cause, as shown when the missing 'Bearer' prefix was identified. [00:07:04](https://www.youtube.com/watch?v=P4JSc8TYo4I&t=424)
- Fiddler rules let you intentionally break your app to test resilience—Claude created a rate-limit rule and a delay rule, and the agent successfully diagnosed and fixed the resulting issues. [00:09:06](https://www.youtube.com/watch?v=P4JSc8TYo4I&t=546)
