---
video_id: iyIAdmeKeMM
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-09-27-jev-is-not-a-claude-killer-heres-what-its-for.md
source_transcript: ../transcripts/2026-09-27-jev-is-not-a-claude-killer-heres-what-its-for.md
source_summary_hash: sha256:be9131c6a3d3473d99b2c3d18098b95a0d3603547e12a88862f64287815a165b
source_transcript_hash: sha256:3e37f6733280849fb62d12ae3eadff992c912652b2adc44edb3fc54672782492
fill_id: f6c0a2b9-afe7-4840-a51f-65371da5398f
published_at: '2026-09-30T08:16:16.209046'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Use Jeff for instant, low-cost classification and routing in automated software factory workflows.

## Prerequisites

### OpenRouter Account
- **Kind**: account
- **Note**: Bypasses the TypeSafe waitlist to access Jeff via API.

### GitHub Repository
- **Kind**: tool
- **Note**: Required for the automated issue classification workflow.

### Claude Code Agent
- **Kind**: tool
- **Note**: Used to generate code and manage repository changes.

## Steps

### Understand Jeff's Role
- **Timestamp**: [00:54](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=54)
- **Action**: Recognize that Jeff is a 'System 1' model for instant classification, not a reasoning model like Claude. It excels at choice, score, or zero tasks with deterministic output.

### Access Jeff via OpenRouter
- **Timestamp**: [08:02](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=482)
- **Action**: Sign up for an OpenRouter account to bypass the TypeSafe waitlist and gain access to the latest version of Jeff.

### Generate API Key in Playground
- **Timestamp**: [09:01](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=541)
- **Action**: Navigate to the TypeSafe AI dashboard playground, view the JSON structure of a response, and create a new API key named 'tutorial'.

### Clone Repository for Setup
- **Timestamp**: [10:01](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=601)
- **Action**: Open your coding agent, install Opus 5.5, and clone the demonstration repository into your project root folder.

### Configure GitHub Labels
- **Timestamp**: [11:20](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=680)
- **Action**: Ask the agent to add specific tags (e.g., Claude Fable, Codex Astra, Claude Haiku) to the repository for routing purposes.

### Install TypeSafe Agent Skill
- **Timestamp**: [12:48](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=768)
- **Action**: Copy the URL for the official TypeSafe agent skill from the community link and install it in your project folder.

### Deploy GitHub Action Logic
- **Timestamp**: [13:36](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=816)
- **Action**: Instruct the agent to push changes that call Jeff via a GitHub Action on new issues, assigning labels and adding comments with confidence scores.

### Test Workflow with New Issue
- **Timestamp**: [14:30](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=870)
- **Action**: Create a new issue in the repository to verify that Jeff classifies it, assigns an agent, and posts a comment with the input/response.

## Gotchas

### Jeff cannot write complete sentences or reason; it is strictly for classification tasks like choice, score, or zero.
- **Severity**: serious
- **Timestamp**: [03:35](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=215)

### Use a confidence threshold (e.g., 0.75) to route low-confidence results to human review instead of automated agents.
- **Severity**: heads_up
- **Timestamp**: [05:35](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=335)

### Jeff has a tiny context window of about 32,000 tokens and is not suitable for complex science or math tasks.
- **Severity**: serious
- **Timestamp**: [02:38](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=158)

## Where to go next

Join Agentyc Labs for the coding masterclass and live sessions on building software factories with AI agents. Next Thursday covers JFA I in depth.

## Concepts surfaced

[[system-1-classification]] · [[software-factory-workflow]] · [[github-actions-automation]] · [[deterministic-output]] · [[cost-efficient-ai]]
