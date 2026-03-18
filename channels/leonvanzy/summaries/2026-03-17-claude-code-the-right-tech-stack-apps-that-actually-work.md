---
title: "Claude Code + The Right Tech Stack = Apps That Actually Work"
video_id: e6fqES1ygAQ
date: 2026-03-17
url: https://www.youtube.com/watch?v=e6fqES1ygAQ
channel: Leon van Zyl
tags:
  - tutorials
  - coding
  - ai-tools
transcript: ../transcripts/2026-03-17-claude-code-the-right-tech-stack-apps-that-actually-work.md
---

# Claude Code + The Right Tech Stack = Apps That Actually Work

## Executive Summary

Leon van Zyl walks beginners through the full web application tech stack, explaining why vibe-coded apps break when they skip foundational architecture decisions. He builds a bookmark app step by step, progressing from browser local storage to SQLite to a production-ready Postgres database, showing how each upgrade solves real deployment problems. The key lesson is that AI coding agents default to convenient but non-production choices like SQLite, and developers must understand the front-end, back-end, and database layers to catch these pitfalls. He recommends a Next.js + React + Postgres + Drizzle ORM + BetterAuth stack and provides a free boilerplate template to get started immediately.

## Key Points

- Vibe-coded apps often fail in production because AI agents default to SQLite, which cannot persist data on platforms like Vercel or Netlify; migrating to a managed Postgres database with Drizzle ORM solves this and makes deployment straightforward. [17:04](https://www.youtube.com/watch?v=e6fqES1ygAQ&t=1024)
- Using Next.js as a meta-framework eliminates the complexity of managing separate front-end and back-end servers, consolidating everything into a single project that handles both UI and secure server-side logic out of the box. [15:11](https://www.youtube.com/watch?v=e6fqES1ygAQ&t=911)
- When starting a new project, explicitly telling your coding agent that the app must be production-ready and specifying the deployment target (e.g., Vercel) prevents it from choosing throwaway technologies and dramatically improves the resulting architecture. [23:45](https://www.youtube.com/watch?v=e6fqES1ygAQ&t=1425)
