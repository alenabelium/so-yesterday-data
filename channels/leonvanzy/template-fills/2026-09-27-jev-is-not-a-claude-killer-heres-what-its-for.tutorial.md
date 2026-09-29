---
video_id: iyIAdmeKeMM
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-09-27-jev-is-not-a-claude-killer-heres-what-its-for.md
source_transcript: ../transcripts/2026-09-27-jev-is-not-a-claude-killer-heres-what-its-for.md
source_summary_hash: sha256:be9131c6a3d3473d99b2c3d18098b95a0d3603547e12a88862f64287815a165b
source_transcript_hash: sha256:3e37f6733280849fb62d12ae3eadff992c912652b2adc44edb3fc54672782492
fill_id: 01ebadeb-a421-45a2-b44b-6fc8a2fbec24
published_at: '2026-09-29T14:12:13.520951'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Use Jeff for instant, low-cost classification tasks like routing GitHub issues to coding agents.

## Prerequisites

### TypeSafe AI or OpenRouter account
- **Kind**: account
- **Note**: Sign up for TypeSafe AI or use OpenRouter to access Jeff without the waitlist.

### GitHub Repository
- **Kind**: tool
- **Note**: A repository to connect to the software factory workflow and test issue classification.

### Claude Code Agent
- **Kind**: tool
- **Note**: Used in the demo to clone repos, create issues, and push GitHub Actions code.

## Steps

### Understand Jeff's capabilities
- **Timestamp**: [02:38](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=158)
- **Action**: Recognize that Jeff is a 'System 1' model for instant classification, not complex reasoning. It supports choice, score, or zero tasks with deterministic output and confidence scores.

### Access Jeff via OpenRouter
- **Timestamp**: [08:02](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=482)
- **Action**: Bypass the TypeSafe AI waitlist by registering on OpenRouter, which provides access to the latest version of Jeff for this tutorial.

### Generate API Key
- **Timestamp**: [09:01](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=541)
- **Action**: Navigate to the TypeSafe AI dashboard, go to API keys, create a new key named 'tutorial', copy it, and add credits if necessary.

### Setup GitHub Repository
- **Timestamp**: [10:01](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=601)
- **Action**: Clone a test repository using Claude Code, create a new private GitHub repository for the project, and add specific labels like 'error', 'documentation', and 'enhancement'.

### Install TypeSafe Agent Skill
- **Timestamp**: [12:48](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=768)
- **Action**: Copy the URL for the official TypeSafe AI agent skill repository and install it in your project folder to teach the agent how to use Jeff's APIs.

### Configure GitHub Action
- **Timestamp**: [13:36](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=816)
- **Action**: Instruct Claude Code to create a GitHub Action that calls Jeff on new issues to classify them (bug, doc, enhancement) and assign an agent (Fable, Astra, Haiku), then post the response.

### Test the Workflow
- **Timestamp**: [14:30](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=870)
- **Action**: Create a new GitHub issue to verify that Jeff classifies it correctly, assigns the agent, and posts a comment with the confidence score and input/output data.

## Gotchas

### Jeff cannot write complete sentences or reason; it is strictly for classification tasks like choice, score, or zero.
- **Severity**: blocking
- **Timestamp**: [02:38](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=158)

### Jeff has a tiny context window of about 32,000 tokens and is bad at science/math tasks requiring reasoning.
- **Severity**: serious
- **Timestamp**: [02:38](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=158)

### If confidence scores are below 0.75, you should add logic to pass the task to a human for review.
- **Severity**: heads_up
- **Timestamp**: [05:35](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=335)

## Where to go next

Join Agentyc Labs for the coding masterclass and live sessions on building software factories and using agents effectively. See the description for links.

## Concepts surfaced

[[system-1-models]] · [[github-actions]] · [[agent-routing]] · [[cost-optimization]]
