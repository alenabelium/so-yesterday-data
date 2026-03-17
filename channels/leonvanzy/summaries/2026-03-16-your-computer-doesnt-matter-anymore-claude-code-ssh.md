---
title: "Your Computer Doesn't Matter Anymore - Claude Code SSH"
video_id: HIaRu-_Gmno
date: 2026-03-16
url: https://www.youtube.com/watch?v=HIaRu-_Gmno
channel: Leon van Zyl
tags:
  - tutorials
  - ai-tools
  - coding
  - productivity
transcript: ../transcripts/2026-03-16-your-computer-doesnt-matter-anymore-claude-code-ssh.md
---

# Your Computer Doesn't Matter Anymore - Claude Code SSH

## Executive Summary

Running Claude Code on a remote VPS via SSH frees you from local hardware limitations and lets you connect from any device. The setup involves spinning up a VPS (e.g., on Hostinger), installing Claude Code on the server, generating an SSH key pair locally, adding the public key to the server's authorized_keys, and configuring the connection in Claude Code Desktop. Once connected, all code and dependencies live on the always-available server, and Claude Code continues running even when your local machine is off.

## Key Points

- Moving Claude Code and project dependencies to a VPS means your local machine only runs Claude Code Desktop as a thin client -- the code is always available, agents keep running when you shut down your PC, and you can connect from any device (laptop, work PC, etc.). [01:42](https://www.youtube.com/watch?v=HIaRu-_Gmno&t=102)
- The SSH setup requires three commands on the server (create .ssh directory, add public key to authorized_keys, set permissions) and one local command (ssh-keygen) -- then you fill in the user, host IP, port 22, and identity file path in Claude Code Desktop. [06:20](https://www.youtube.com/watch?v=HIaRu-_Gmno&t=380)
- A VPS can be more powerful than local hardware, which is especially beneficial for resource-intensive tasks like game development or machine learning, and the Hostinger template also installs N8N as a bonus automation platform. [02:39](https://www.youtube.com/watch?v=HIaRu-_Gmno&t=159)
