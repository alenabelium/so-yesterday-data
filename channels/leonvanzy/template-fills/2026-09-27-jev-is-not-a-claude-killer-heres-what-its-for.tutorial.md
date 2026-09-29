---
video_id: iyIAdmeKeMM
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-09-27-jev-is-not-a-claude-killer-heres-what-its-for.md
source_transcript: ../transcripts/2026-09-27-jev-is-not-a-claude-killer-heres-what-its-for.md
source_summary_hash: sha256:be9131c6a3d3473d99b2c3d18098b95a0d3603547e12a88862f64287815a165b
source_transcript_hash: sha256:3e37f6733280849fb62d12ae3eadff992c912652b2adc44edb3fc54672782492
fill_id: e2037c75-9d57-44a3-9da8-e4c7e0be5202
published_at: '2026-09-29T12:12:21.622736'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Use TypeSafe AI's Jeff model for instant, low-cost classification and routing tasks instead of expensive reasoning models.

## Prerequisites

### TypeSafe AI Account
- **Kind**: account
- **Note**: Sign up at typesafe.ai. A waiting list may exist; use OpenRouter as an alternative access method.

### OpenRouter Account
- **Kind**: account
- **Note**: Register to bypass TypeSafe's waitlist and access the latest Jeff version via their API.

### GitHub Repository
- **Kind**: tool
- **Note**: A repository is needed to test the workflow. Clone a sample repo or create a new private one for this tutorial.

### Claude Code Agent
- **Kind**: tool
- **Note**: Used in the demo to generate code and GitHub Actions. Install Opus 5.5 with high logical reasoning level.

## Steps

### Understand Jeff's Role
- **Timestamp**: [00:00](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=0)
- **Action**: Recognize that Jeff is a 'System 1' model for instant, low-cost classification (choice, score, zero), not a general-purpose reasoning LLM like Claude.

### Access Jeff via OpenRouter
- **Timestamp**: [08:02](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=482)
- **Action**: If the TypeSafe AI waiting list is active, register on OpenRouter to access Jeff. Use OpenRouter's API endpoint if not using the TypeSafe dashboard.

### Generate API Key
- **Timestamp**: [09:01](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=541)
- **Action**: In the TypeSafe AI dashboard, navigate to API keys, create a new key named 'tutorial', copy it, and save it securely. Add credits if necessary.

### Clone Sample Repository
- **Timestamp**: [10:01](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=601)
- **Action**: Open your coding agent (e.g., Claude Code with Opus 5.5). Paste the GitHub URL from the video to clone the sample web application repository.

### Create Private Repo & Add Labels
- **Timestamp**: [11:02](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=662)
- **Action**: Ask your agent to create a new private GitHub repository. Then, instruct it to add specific labels: improvement, error, documentation change, and agent tags (Claude Fable, Codex Astra, Claude Haiku).

### Install TypeSafe Agent Skill
- **Timestamp**: [12:48](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=768)
- **Action**: Copy the GitHub URL for the official TypeSafe agent skill. Instruct your coding agent to install this skill in the project folder to teach it how to use Jeff's API.

### Configure GitHub Action
- **Timestamp**: [13:36](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=816)
- **Action**: Instruct your agent to create a GitHub Action that calls Jeff on new issues. It must classify the issue (bug/docs/enhancement), assign an agent (Fable/Astra/Haiku), and add a comment with input, response, and confidence scores.

### Test the Workflow
- **Timestamp**: [14:30](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=870)
- **Action**: Create a new GitHub issue (e.g., 'add a new emotion'). Observe Jeff's response in the comments, verifying the classification category, assigned agent, and confidence scores.

## Gotchas

### Jeff cannot write complete sentences or reason. It is strictly for fast, deterministic classification tasks like choice, score, or zero.
- **Severity**: blocking
- **Timestamp**: [02:38](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=158)

### Jeff has a tiny context window of about 32,000 tokens. Do not use it for complex tasks requiring long context or scientific reasoning.
- **Severity**: serious
- **Timestamp**: [02:38](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=158)

### Check the confidence score in Jeff's response. If it is below 0.75, implement logic to route the task to a human for review.
- **Severity**: heads_up
- **Timestamp**: [05:35](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=335)

## Where to go next

Join Agentyc Labs for the coding masterclass and live sessions. Next Thursday features a deep dive into JFAI. Links are in the video description.

## Concepts surfaced

[[system-1-vs-system-2-ai]] · [[cost-efficient-classification]] · [[github-automation-workflows]] · [[deterministic-llm-output]] · [[software-factory-routing]]
