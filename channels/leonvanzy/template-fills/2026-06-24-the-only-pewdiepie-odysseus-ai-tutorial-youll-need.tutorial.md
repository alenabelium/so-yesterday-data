---
video_id: 7lfyY5ZiHgg
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-06-24-the-only-pewdiepie-odysseus-ai-tutorial-youll-need.md
source_transcript: ../transcripts/2026-06-24-the-only-pewdiepie-odysseus-ai-tutorial-youll-need.md
source_summary_hash: sha256:235ce3f44d9831f5f9e273f5821d62a9b4a3fd92af40cb556d9d1fc94aa141c5
source_transcript_hash: sha256:357bcc2578449f45e6dac615a92307616902d2b303dd1e08a64324ff1b049f24
fill_id: 6c6aea04-1673-48be-9054-39879887fbbb
published_at: '2026-09-29T11:05:59.744594'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Set up Odysseus AI locally or on a VPS for a private, self-hosted workspace with deep research and agent skills.

## Prerequisites

### Docker Desktop
- **Kind**: tool
- **Note**: Required to run the Odysseus containers locally.

### Git
- **Kind**: tool
- **Note**: Needed to clone the Odysseus repository.

### GitHub Account
- **Kind**: account
- **Note**: Required to access the Odysseus source code repository.

### Ollama or LM Studio
- **Kind**: tool
- **Note**: Local inference engines for running models offline.

## Steps

### Install Docker and Git
- **Timestamp**: [02:25](https://www.youtube.com/watch?v=7lfyY5ZiHgg&t=145)
- **Action**: Download and install Docker Desktop and Git for your operating system.
- **Command Or Clicks**: Download Docker Desktop and Git from their official websites.

### Clone and Configure Odysseus
- **Timestamp**: [03:43](https://www.youtube.com/watch?v=7lfyY5ZiHgg&t=223)
- **Action**: Create a folder, clone the repo, rename env.example to .env, and start containers.
- **Command Or Clicks**: git clone <repo-url> && cd odysseus && mv .env.example .env && docker compose up -d
- **Choice Branch**: Use cp command on Mac/Linux instead of manual rename.

### Access and Sign In
- **Timestamp**: [04:45](https://www.youtube.com/watch?v=7lfyY5ZiHgg&t=285)
- **Action**: Find the admin password in Docker logs and sign in at localhost:7000.
- **Command Or Clicks**: docker logs odysseus_main | grep 'initial admin'

### Configure Local Models
- **Timestamp**: [07:29](https://www.youtube.com/watch?v=7lfyY5ZiHgg&t=449)
- **Action**: Install Ollama/LM Studio, download a model, and connect via /setup local.
- **Command Or Clicks**: ollama pull <model-name> && /setup local http://localhost:11434/v1
- **Choice Branch**: Use LM Studio IP instead of Ollama URL.

### Explore Features
- **Timestamp**: [11:50](https://www.youtube.com/watch?v=7lfyY5ZiHgg&t=710)
- **Action**: Test agent mode, email integration, and the second brain memory system.
- **Command Or Clicks**: Use /skills command and email integration settings.

### Deploy to VPS
- **Timestamp**: [17:02](https://www.youtube.com/watch?v=7lfyY5ZiHgg&t=1022)
- **Action**: Install Odysseus on Hostinger VPS and configure OpenRouter API.
- **Command Or Clicks**: /setup openrouter <api-key>

## Gotchas

### AGPL3 license restricts rebranding; check terms before forking.
- **Severity**: serious
- **Timestamp**: [01:00](https://www.youtube.com/watch?v=7lfyY5ZiHgg&t=60)

### Hugging Face downloads may be rate-limited without a token.
- **Severity**: heads_up
- **Timestamp**: [05:30](https://www.youtube.com/watch?v=7lfyY5ZiHgg&t=330)

### Local model downloads may crash if hardware is insufficient.
- **Severity**: blocking
- **Timestamp**: [06:45](https://www.youtube.com/watch?v=7lfyY5ZiHgg&t=405)

## Where to go next

Join Agentic Labs for masterclasses on coding agents and SaaS builds.

## Concepts surfaced

[[self-hosted-ai]] · [[local-inference]] · [[docker-setup]] · [[agent-skills]] · [[deep-research]] · [[vps-deployment]]
