---
title: "Stop Babysitting Claude Code - Run It in a Sandbox Instead"
video_id: iUDuN9dyuTY
date: 2026-07-29
url: https://www.youtube.com/watch?v=iUDuN9dyuTY
channel: Leon van Zyl
tags:
  - ai-agents
  - ai-safety
  - productivity
  - tutorials
transcript: ../transcripts/2026-07-29-stop-babysitting-claude-code-run-it-in-a-sandbox-instead.md
relevant: true
---

# Stop Babysitting Claude Code - Run It in a Sandbox Instead

## Executive Summary

The video argues that running AI coding agents like Claude Code in 'YOLO' mode without safeguards is risky due to potential prompt injections and credential leaks. It introduces Docker Sandboxes as a secure, isolated microVM environment that allows agents to operate freely without accessing the host machine's sensitive data. The presenter demonstrates how to install Docker Sandboxes, configure network policies, and securely inject secrets for GitHub integration. Finally, the video showcases a practical workflow where the agent autonomously triages issues and creates pull requests within the disposable sandbox environment.

## Key Points

- Running AI agents in standard mode exposes sensitive host files and credentials to prompt injection risks, whereas Docker Sandboxes isolate the agent in a microVM with its own kernel and file system [00:02:08](https://www.youtube.com/watch?v=iUDuN9dyuTY&t=128).
- Setting up Docker Sandboxes involves installing the 'spx' tool, configuring network policies (open, balanced, or lockdown), and securely piping secrets like GitHub tokens from the host to the sandbox environment [00:06:23](https://www.youtube.com/watch?v=iUDuN9dyuTY&t=383).
- The agent successfully triaged 81 issues and implemented five changes to create a pull request within the sandbox, demonstrating that the disposable environment ensures safety while maintaining high productivity [00:14:27](https://www.youtube.com/watch?v=iUDuN9dyuTY&t=867).
