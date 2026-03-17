---
title: "Stop Building Websites the Hard Way (Use Claude Code)"
video_id: R65qnDnSFWY
date: 2026-01-27
url: https://www.youtube.com/watch?v=R65qnDnSFWY
channel: Leon van Zyl
tags:
  - ai-tools
  - coding
  - tutorials
  - prompting
transcript: ../transcripts/2026-01-27-stop-building-websites-the-hard-way-use-claude-code.md
---

# Stop Building Websites the Hard Way (Use Claude Code)

## Executive Summary

This comprehensive tutorial demonstrates building a professional restaurant website with Claude Code, including a design system enforced by a custom sub-agent, stock image optimization via a custom skill, an N8N-powered AI chatbot with menu knowledge and reservation capabilities, and free deployment on Vercel. The workflow combines design reference images from Dribbble, the front-end design skill from Anthropic's marketplace, a custom image-to-WebP skill for performance optimization, and N8N data tables for backend functionality -- all without writing any code manually.

## Key Points

- Installing the front-end design skill from Anthropic's marketplace and creating a custom front-end designer sub-agent that references a design system eliminates AI slop, producing unique, professional-looking designs consistent across all pages. [05:46](https://www.youtube.com/watch?v=R65qnDnSFWY&t=346)
- Creating a custom Claude Code skill to download stock images, resize them, and convert to WebP reduced image sizes dramatically (e.g., 96KB vs 718KB) and ensured consistent optimization that can be reused across projects. [17:56](https://www.youtube.com/watch?v=R65qnDnSFWY&t=1076)
- Embedding an N8N chatbot with data table tools gives the website an AI assistant that can answer menu questions and create reservations in a real database, while the reservation form connects to N8N via a webhook API endpoint for non-chat bookings. [28:54](https://www.youtube.com/watch?v=R65qnDnSFWY&t=1734)
