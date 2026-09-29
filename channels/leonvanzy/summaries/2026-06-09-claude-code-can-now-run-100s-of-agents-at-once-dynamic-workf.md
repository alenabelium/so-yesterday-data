---
title: "Claude Code Can Now Run 100s of Agents at Once (Dynamic Workflows)"
video_id: Aa_6bmzDc80
date: 2026-06-09
url: https://www.youtube.com/watch?v=Aa_6bmzDc80
channel: Leon van Zyl
tags:
  - ai-tools
  - productivity
  - coding
transcript: ../transcripts/2026-06-09-claude-code-can-now-run-100s-of-agents-at-once-dynamic-workf.md
relevant: true
---

# Claude Code Can Now Run 100s of Agents at Once (Dynamic Workflows)

## Executive Summary

Claude Code now supports dynamic workflows, enabling the execution of hundreds of parallel agents to handle large-scale, repetitive tasks efficiently. The video demonstrates how to initiate these workflows using specific prompts, emphasizing their suitability for batch processing over simple, single-session tasks. Key best practices include starting with small test batches to verify logic, avoiding human-in-the-loop interactions, and managing file contention when multiple agents modify the same codebase. Users can save and reuse these workflows, making them a powerful tool for automating complex, multi-step operations like security audits.

## Key Points

- Dynamic workflows allow Claude Code to spin up tens or hundreds of parallel sub-agents, making them ideal for repetitive tasks like auditing hundreds of items, but they are expensive due to high token usage and should be avoided for simple tasks [00:02:10](https://www.youtube.com/watch?v=Aa_6bmzDc80&t=130).
- To implement a workflow, users must explicitly prompt Claude to use one, start with a small batch for verification, and ensure requirements are clear upfront since the process runs autonomously without human intervention [00:03:34](https://www.youtube.com/watch?v=Aa_6bmzDc80&t=214).
- Users can save, share, and reuse created workflows by pressing 'S' during the session, allowing teams to deploy standardized automation scripts like the demonstrated OWASP security audit in future sessions [00:06:48](https://www.youtube.com/watch?v=Aa_6bmzDc80&t=408).
