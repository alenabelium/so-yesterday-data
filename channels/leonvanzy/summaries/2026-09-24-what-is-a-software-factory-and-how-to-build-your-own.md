---
title: "What Is a Software Factory? (And How to Build Your Own)"
video_id: AsvzMlLyQ38
date: 2026-09-24
url: https://www.youtube.com/watch?v=AsvzMlLyQ38
channel: Leon van Zyl
tags:
  - ai-agents
  - coding
  - productivity
  - tutorials
transcript: ../transcripts/2026-09-24-what-is-a-software-factory-and-how-to-build-your-own.md
relevant: true
---

# What Is a Software Factory? (And How to Build Your Own)

## Executive Summary

The video explains the concept of a software factory, which orchestrates a swarm of coding agents to process tasks via GitHub issues rather than requiring manual session management. It demonstrates how to build and deploy this system using Upstash for isolated agent sandboxes and GitHub Actions for workflow triggers. The tutorial provides a step-by-step guide on configuring agents like Claude and Codex, setting up secure API keys, and scaling the infrastructure through reusable snapshots.

## Key Points

- A software factory acts as an orchestration layer that receives signals (like GitHub issues), triages them, and assigns tasks to a swarm of available coding agents in sandboxed environments for safety and resource isolation [00:01:55](https://www.youtube.com/watch?v=AsvzMlLyQ38&t=115).
- The setup process involves using an AI agent to install a specific 'software factory skill' that programmatically creates Upstash boxes (virtual machines) and configures GitHub Actions to handle the workflow [00:09:13](https://www.youtube.com/watch?v=AsvzMlLyQ38&t=553).
- Security is maintained by running each agent in its own isolated VPS with limited permissions, using fine-grained GitHub tokens, and leveraging reusable snapshots to standardize agent environments across the swarm [00:05:06](https://www.youtube.com/watch?v=AsvzMlLyQ38&t=306).
- Scaling and maintenance are simplified by creating reusable snapshots for agent configurations and using GitHub merge requests to add or remove project repositories from the factory's scope [00:22:31](https://www.youtube.com/watch?v=AsvzMlLyQ38&t=1351). [MM:SS](https://www.youtube.com/watch?v=AsvzMlLyQ38&t=SECONDS)
