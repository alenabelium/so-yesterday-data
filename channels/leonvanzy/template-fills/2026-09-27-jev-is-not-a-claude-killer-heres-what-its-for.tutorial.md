---
video_id: iyIAdmeKeMM
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-09-27-jev-is-not-a-claude-killer-heres-what-its-for.md
source_transcript: ../transcripts/2026-09-27-jev-is-not-a-claude-killer-heres-what-its-for.md
source_summary_hash: sha256:be9131c6a3d3473d99b2c3d18098b95a0d3603547e12a88862f64287815a165b
source_transcript_hash: sha256:3e37f6733280849fb62d12ae3eadff992c912652b2adc44edb3fc54672782492
fill_id: 817228ce-8121-4c51-bcf0-a5def87b4d5e
published_at: '2026-09-29T17:11:36.358849'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Use Jeff from TypeSafe AI for instant, low-cost classification tasks like routing GitHub issues to coding agents.

## Prerequisites

### OpenRouter Account
- **Kind**: account
- **Note**: Sign up at OpenRouter to bypass TypeSafe's waiting list and access Jeff via API.

### GitHub Repository
- **Kind**: tool
- **Note**: A repo to connect to the software factory workflow for automated issue tagging.

### Claude Code Agent
- **Kind**: tool
- **Note**: Used in the demo to clone repos and generate GitHub Actions workflows.

## Steps

### Access Jeff via OpenRouter
- **Timestamp**: [08:02](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=482)
- **Action**: Bypass the TypeSafe waiting list by registering at OpenRouter, which provides access to the latest version of Jeff.
- **Command Or Clicks**: Go to OpenRouter and register an account.

### Create API Key in TypeSafe
- **Timestamp**: [09:01](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=541)
- **Action**: Navigate to the API keys section in the TypeSafe dashboard, create a new key named 'tutorial', and save it securely.
- **Command Or Clicks**: Go to API keys -> Create new key -> Copy and save.

### Clone Repository
- **Timestamp**: [10:01](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=601)
- **Action**: Use Claude Code to clone a test GitHub repository into the project root folder for the demo.
- **Command Or Clicks**: Open agent (Claude Code) -> Paste GitHub URL -> Clone to root folder.

### Define Agent Labels
- **Timestamp**: [11:20](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=680)
- **Action**: Ask the coding agent to add specific tags to the repository for routing, such as 'Claude Opus', 'Codex Astra', and 'Claude Haiku'.
- **Command Or Clicks**: Prompt agent: 'Please add these tags: Claude Opus, Codex Astra, Claude Haiku.'

### Install TypeSafe Skill
- **Timestamp**: [12:48](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=768)
- **Action**: Copy the URL for the official TypeSafe agent skill from GitHub and install it in the project folder to teach the agent how to use Jeff.
- **Command Or Clicks**: Copy URL -> Return to agent -> Install skill in project folder.

### Configure GitHub Action
- **Timestamp**: [13:36](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=816)
- **Action**: Instruct the agent to create a GitHub Action that calls Jeff on new issues to classify them and assign agents based on confidence scores.
- **Command Or Clicks**: Prompt agent: 'Create GitHub Action to call Jeff, tag issues, assign agents, and add comments with confidence scores.'

### Test the Workflow
- **Timestamp**: [14:30](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=870)
- **Action**: Create a new GitHub issue to verify that Jeff correctly classifies the task, assigns an agent, and posts a comment with the response.
- **Command Or Clicks**: Create new issue -> Check comments for Jeff's classification and confidence score.

## Gotchas

### Jeff is a 'System 1' model; it cannot reason or write complete sentences, making it unsuitable for complex tasks like science or math.
- **Severity**: serious
- **Timestamp**: [02:38](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=158)

### Jeff has a tiny context window of about 32,000 tokens and is not a chatbot; use it only for choice, score, or zero tasks.
- **Severity**: serious
- **Timestamp**: [03:35](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=215)

### If the confidence score is below 0.75, add logic to pass the request to a human for review rather than automating it blindly.
- **Severity**: heads_up
- **Timestamp**: [05:35](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=335)

## Where to go next

Join Agentyc Labs for the coding masterclass and next Thursday's deep dive into JFA I. Check the description for links to the software factory tutorial and Decodr sponsor.

## Concepts surfaced

[[system-1-vs-system-2]] · [[github-actions-automation]] · [[llm-cost-optimization]] · [[software-factory-workflow]]
