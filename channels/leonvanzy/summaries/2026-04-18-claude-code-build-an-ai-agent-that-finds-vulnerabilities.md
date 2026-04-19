---
title: "Claude Code: Build an AI Agent That Finds Vulnerabilities"
video_id: VFLieg8JjLA
date: 2026-04-18
url: https://www.youtube.com/watch?v=VFLieg8JjLA
channel: Leon van Zyl
tags:
  - coding
  - ai-tools
  - tutorials
  - ai-agents
transcript: ../transcripts/2026-04-18-claude-code-build-an-ai-agent-that-finds-vulnerabilities.md
---

# Claude Code: Build an AI Agent That Finds Vulnerabilities

## Executive Summary

Leon van Zyl walks through building a security vulnerability scanner using Claude Code's skills and sub-agent system. Rather than creating a standalone Python application, he demonstrates a reusable approach: first creating a Claude Code skill that references the OWASP Top 10 vulnerability checklist with separate reference documents, then building a sub-agent that invokes the skill to audit any codebase. When tested against an intentionally vulnerable note-keeping app, the agent identified 37 security vulnerabilities including SQL injections, broken access control, and cryptographic failures, producing a structured audit report. The key insight is that skills are portable and shareable across projects, agents, and teams.

## Key Points

- The approach uses Claude Code's skill system to create a reusable security scanner with OWASP Top 10 references stored as separate markdown files, making it portable across projects and shareable with any assistant that supports skills -- including Codex and OpenClaw. [03:18](https://www.youtube.com/watch?v=VFLieg8JjLA&t=198)
- A dedicated sub-agent is created alongside the skill to handle autonomous security audits, demonstrating how skills and sub-agents work hand in hand -- the main agent can delegate security reviews to the sub-agent while coordinating other tasks. [09:16](https://www.youtube.com/watch?v=VFLieg8JjLA&t=556)
- The scanner successfully identified 37 vulnerabilities in a deliberately insecure test app, including 9 critical issues like SQL injection and broken authentication with MD5 passwords, producing a structured report with risk scores and remediation guidance. [11:06](https://www.youtube.com/watch?v=VFLieg8JjLA&t=666)
