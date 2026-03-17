---
title: "OpenClaw Is Incredible — Here's How to Actually Use It"
video_id: XH0pVKjnmww
date: 2026-01-28
url: https://www.youtube.com/watch?v=XH0pVKjnmww
channel: Leon van Zyl
tags:
  - ai-tools
  - tutorials
  - ai-agents
  - ethics-safety
transcript: ../transcripts/2026-01-28-openclaw-is-incredible-heres-how-to-actually-use-it.md
---

# OpenClaw Is Incredible — Here's How to Actually Use It

## Executive Summary

OpenClaw (formerly Moldbot/Claudebot) is an open-source project that lets you create a persistent AI assistant accessible via Telegram, WhatsApp, Discord, and other chat platforms. Its standout feature is persistent memory that learns your preferences over time and adapts responses accordingly. However, the agent has full root access to your server by default, creating significant security risks. The video walks through setup on a VPS, connecting Telegram, installing skills for thumbnail generation, and recommends running the agent in a sandboxed Docker environment with limited privileges for production use.

## Key Points

- OpenClaw's persistent memory is its killer feature -- it remembers your preferences across conversations, so when asked to generate thumbnails it automatically includes your face and preferred style based on past interactions, without being explicitly told. [00:00](https://www.youtube.com/watch?v=XH0pVKjnmww&t=0)
- The agent runs with full root access by default, meaning a compromised chat channel could let attackers execute arbitrary commands on your server; running it in a sandboxed Docker container with a dedicated limited-privilege user is strongly recommended. [03:04](https://www.youtube.com/watch?v=XH0pVKjnmww&t=184)
- For users who only need an AI assistant without file system access and command execution, N8N is presented as a safer alternative that can replicate most of OpenClaw's capabilities (memory, thumbnails, research) through drag-and-drop workflows. [16:23](https://www.youtube.com/watch?v=XH0pVKjnmww&t=983)
