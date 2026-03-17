---
title: "Don't Build Another OpenClaw Agent Until You Watch This"
video_id: OASdadLGW4s
date: 2026-02-18
url: https://www.youtube.com/watch?v=OASdadLGW4s
channel: Leon van Zyl
tags:
  - ai-tools
  - ai-agents
  - tutorials
  - productivity
transcript: ../transcripts/2026-02-18-dont-build-another-openclaw-agent-until-you-watch-this.md
---

# Don't Build Another OpenClaw Agent Until You Watch This

## Executive Summary

OpenClaw's persistent memory makes it a powerful personal AI assistant that adapts to your preferences over time, but losing your server means losing all that trained knowledge. The video shows how to set up automated daily GitHub backups of the agent's entire workspace -- including memories, identity, skills, cron jobs, and generated assets -- using an SSH deploy key. It also walks through a fresh OpenClaw installation (now with OpenAI support), connecting Telegram, and demonstrates the agent's ability to create its own backup cron job through natural conversation.

## Key Points

- The agent's workspace files (agent.md, heartbeat, identity, memory, soul, tools, user) represent everything it has learned about you; automated daily backups to a private GitHub repo via SSH deploy key ensure you can fully recover your assistant if the server is lost. [09:04](https://www.youtube.com/watch?v=OASdadLGW4s&t=544)
- OpenClaw's persistent memory enables genuinely personalized interactions -- asking for a thumbnail automatically includes your face and preferred style because the agent has accumulated your preferences across hundreds of conversations without being explicitly told. [00:00](https://www.youtube.com/watch?v=OASdadLGW4s&t=0)
- The backup setup is remarkably simple: just tell the agent you want daily GitHub backups and it configures the SSH key, git remote, and midnight cron job itself through natural conversation -- no manual scripting required. [10:06](https://www.youtube.com/watch?v=OASdadLGW4s&t=606)
