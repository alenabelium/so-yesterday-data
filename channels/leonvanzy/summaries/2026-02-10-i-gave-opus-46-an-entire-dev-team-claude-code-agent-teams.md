---
title: "I Gave Opus 4.6 an Entire Dev Team - Claude Code Agent Teams"
video_id: KCJsdQpcfic
date: 2026-02-10
url: https://www.youtube.com/watch?v=KCJsdQpcfic
channel: Leon van Zyl
tags:
  - ai-agents
  - coding
  - ai-tools
  - prompting
transcript: ../transcripts/2026-02-10-i-gave-opus-46-an-entire-dev-team-claude-code-agent-teams.md
---

# I Gave Opus 4.6 an Entire Dev Team - Claude Code Agent Teams

## Executive Summary

Opus 4.6 introduced an experimental "agent teams" feature that is fundamentally different from sub-agents. While sub-agents run isolated tasks and report back one-way to the parent, agent team members share a task list, communicate peer-to-peer, and coordinate their work automatically. The video demonstrates building a fitness tracker app with a five-member team (UX designer, backend dev, architect, database expert, devil's advocate), where each member has its own Claude Code instance, can be interrupted and given individual instructions, and has access to skills and MCP servers.

## Key Points

- Agent teams differ from sub-agents because team members share a task list and can communicate directly with each other -- for example, the database agent and API agent coordinate on schema design, preventing the incompatible implementations that isolated sub-agents can produce. [02:21](https://www.youtube.com/watch?v=KCJsdQpcfic&t=141)
- To enable agent teams, add the experimental setting to your project's settings.json, then prompt Claude to "create an agent team to explore this from different angles" with described team members; adding a devil's advocate team member improves output quality. [04:23](https://www.youtube.com/watch?v=KCJsdQpcfic&t=263)
- Human-in-the-loop control works by cycling between team members with shift+arrow keys, pressing escape to interrupt any individual member, and sending targeted instructions -- all without affecting other team members' progress. [00:00](https://www.youtube.com/watch?v=KCJsdQpcfic&t=0)
