---
title: "I Gave Claude Full Access To My App"
video_id: N2Ogvx_U8uM
date: 2026-08-13
url: https://www.youtube.com/watch?v=N2Ogvx_U8uM
channel: Leon van Zyl
tags:
  - ai-agents
  - coding
  - ai-tools
  - tutorials
transcript: ../transcripts/2026-08-13-i-gave-claude-full-access-to-my-app.md
relevant: true
---

# I Gave Claude Full Access To My App

## Executive Summary

This video demonstrates how to build a custom MCP server that allows Claude to interact with a third-party application on behalf of the user. The presenter creates a Trello-like Kanban app, deploys it to Vercel, and then exposes its functionality via an MCP server secured by OAuth authentication. By connecting this custom connector to Claude, the AI agent can perform actions like creating tasks and assigning users directly within the app. The tutorial emphasizes using specific coding skills and context engineering to ensure the agent builds a robust, production-ready integration.

## Key Points

- The presenter uses a 'start-and-app' skill and detailed planning prompts to generate a full-stack Kanban application with Next.js, ensuring the agent creates a scalable architecture with Postgres and proper role-based access control [00:03:17](https://www.youtube.com/watch?v=N2Ogvx_U8uM&t=197).
- After deploying the app to Vercel, the presenter installs 'better-auth' and 'MCP builder' skills to generate a remote MCP server that exposes the app's tools to AI agents while handling secure OAuth authentication [00:18:08](https://www.youtube.com/watch?v=N2Ogvx_U8uM&t=1088).
- The final integration allows Claude to act as a connector, enabling the AI to create, assign, and update tasks in the deployed app by authenticating via the user's existing account through the OAuth flow [00:23:44](https://www.youtube.com/watch?v=N2Ogvx_U8uM&t=1424). [MM:SS](https://www.youtube.com/watch?v=N2Ogvx_U8uM&t=SECONDS)
