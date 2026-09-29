---
video_id: WjOcStPCbgk
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-09-02-fable-51-just-built-a-better-claude-code-for-local-models.md
source_transcript: ../transcripts/2026-09-02-fable-51-just-built-a-better-claude-code-for-local-models.md
source_summary_hash: sha256:a2140cb4bd760ecaa56bd4f8a5d96b91b7c7646c76d2ad8724b2b542fd327c52
source_transcript_hash: sha256:0c1c03e283de9a30fb8e2f9460819e4e3237b1252873b906c775c697d967ac1c
fill_id: 58dda086-dc67-430b-9d17-1381e66b2fb5
published_at: '2026-09-29T11:23:36.211316'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Build a specialized coding harness for local models using Fable 5.1.

## Prerequisites

### Ollama or LM Studio
- **Kind**: tool
- **Note**: Local model runners with API endpoints for Small Coder to connect.

### npm
- **Kind**: tool
- **Note**: Required to install and run the Small Coder package globally.

## Steps

### Define requirements for local model harness
- **Timestamp**: [02:00](https://www.youtube.com/watch?v=WjOcStPCbgk&t=120)
- **Action**: Provide Fable 5.1 with a brain dump of constraints: optimize for free local models, respect context windows, support Ollama/LM Studio, and avoid heavy setup.
- **Command Or Clicks**: None (prompting)
- **Choice Branch**: Specify that the agent should test itself by building a Minecraft clone.

### Request terminal and web interfaces
- **Timestamp**: [03:08](https://www.youtube.com/watch?v=WjOcStPCbgk&t=188)
- **Action**: Ask Fable to build both a terminal interface and a web-based version of the harness, including memory file support and a planning phase for small context windows.
- **Command Or Clicks**: None (prompting)
- **Choice Branch**: Request an integrated browser in the web UI later.

### Audit and fix the application
- **Timestamp**: [05:46](https://www.youtube.com/watch?v=WjOcStPCbgk&t=346)
- **Action**: Create a new session to have Fable audit the app for bugs and optimize it for local models, then manually test and report remaining issues.
- **Command Or Clicks**: None (prompting)
- **Choice Branch**: Rename 'YOLO mode' to 'bypass permissions'.

### Publish to npm
- **Timestamp**: [08:49](https://www.youtube.com/watch?v=WjOcStPCbgk&t=529)
- **Action**: Ask Fable to guide the creation of an npm access token and publish the package, enabling installation via a single command.
- **Command Or Clicks**: npm login / npm publish (guided by agent)
- **Choice Branch**: Choose npx for immediate execution.

### Deploy website to Vercel
- **Timestamp**: [11:00](https://www.youtube.com/watch?v=WjOcStPCbgk&t=660)
- **Action**: Have Fable generate a single-page website from the GitHub repo and deploy it to Vercel with a custom domain.
- **Command Or Clicks**: None (prompting)
- **Choice Branch**: Assign smallcoder.dev as the custom domain.

## Gotchas

### Standard harnesses like Claude Code consume too many tokens for local models with limited context windows.
- **Severity**: serious
- **Timestamp**: [02:00](https://www.youtube.com/watch?v=WjOcStPCbgk&t=120)

### Run Small Coder in the actual workspace directory to allow file modifications.
- **Severity**: blocking
- **Timestamp**: [09:48](https://www.youtube.com/watch?v=WjOcStPCbgk&t=588)

## Where to go next

Check out Aentic Labs for more coding agent workflows. Star the Small Coder repo on GitHub.

## Concepts surfaced

[[local-llm]] · [[ai-agents]] · [[prompt-engineering]] · [[npm-publishing]]
