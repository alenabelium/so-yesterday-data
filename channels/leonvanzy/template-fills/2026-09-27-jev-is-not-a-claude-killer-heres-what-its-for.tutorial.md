---
video_id: iyIAdmeKeMM
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-09-27-jev-is-not-a-claude-killer-heres-what-its-for.md
source_transcript: ../transcripts/2026-09-27-jev-is-not-a-claude-killer-heres-what-its-for.md
source_summary_hash: sha256:be9131c6a3d3473d99b2c3d18098b95a0d3603547e12a88862f64287815a165b
source_transcript_hash: sha256:3e37f6733280849fb62d12ae3eadff992c912652b2adc44edb3fc54672782492
fill_id: e0cf57de-c05a-4b0f-812b-2eee9e318b3e
published_at: '2026-09-30T00:17:26.853596'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Use TypeSafe AI's Jeff model for low-cost, high-speed classification and routing tasks instead of expensive reasoning models.

## Prerequisites

### OpenRouter Account
- **Kind**: account
- **Note**: Sign up to bypass the TypeSafe waitlist and access Jeff via OpenRouter API.

### GitHub Repository
- **Kind**: tool
- **Note**: A repository with issues to classify, or create a new test repo for this tutorial.

### Claude Code Agent
- **Kind**: tool
- **Note**: Used to clone the repo and generate the GitHub Actions workflow code.

## Steps

### Understand Jeff's Use Case
- **Timestamp**: [00:54](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=54)
- **Action**: Recognize that Jeff is a 'System 1' model for instant classification (choice, score, or zero), not complex reasoning. It outputs deterministic structures with confidence scores.

### Access Jeff via OpenRouter
- **Timestamp**: [08:02](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=482)
- **Action**: Log in to typesafe.ai. If on the waitlist, register an account on OpenRouter instead to access the latest version of Jeff immediately.

### Generate API Key
- **Timestamp**: [09:01](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=541)
- **Action**: In the TypeSafe dashboard, navigate to 'API keys', create a new key named 'tutorial', copy it, and save it securely. Add credits if necessary.

### Clone Repository
- **Timestamp**: [10:01](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=601)
- **Action**: Open your coding agent (e.g., Claude Code). Paste the command to clone the demo repository into your project root folder.
- **Command Or Clicks**: git clone <repository-url>

### Create GitHub Repo & Labels
- **Timestamp**: [11:02](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=662)
- **Action**: Ask the agent to create a new private GitHub repository and add specific labels (e.g., improvement, error, documentation) for classification.

### Install Agent Skill
- **Timestamp**: [12:48](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=768)
- **Action**: Copy the URL for the TypeSafe agent skill repository. Return to your coding agent and install this skill in the project folder to teach it how to use Jeff.

### Generate GitHub Action
- **Timestamp**: [13:36](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=816)
- **Action**: Instruct the agent to create a GitHub Action that calls Jeff on new issues. It should classify the issue (bug/docs/enhancement), assign an agent (Fable/Astra/Haiku), and add a comment with the response and confidence score.

### Test the Workflow
- **Timestamp**: [14:30](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=870)
- **Action**: Create a new issue in the GitHub repository. Observe Jeff's response, which should include the classification, assigned agent, and confidence scores.

## Gotchas

### Jeff cannot write complete sentences or perform complex reasoning. It is strictly for classification tasks like choice, score, or zero.
- **Severity**: serious
- **Timestamp**: [02:38](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=158)

### Jeff has a tiny context window of about 32,000 tokens. Do not use it for long-context tasks requiring deep analysis.
- **Severity**: blocking
- **Timestamp**: [02:38](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=158)

### Check the confidence score in Jeff's output. If it is below 0.75, implement logic to route the task to a human for review.
- **Severity**: heads_up
- **Timestamp**: [05:35](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=335)

## Where to go next

Join Agentyc Labs for the coding masterclass and live sessions. Next Thursday features a deep dive into JFAI. Links are in the video description.

## Concepts surfaced

[[system-1-vs-system-2]] · [[ai-classification]] · [[github-actions]] · [[cost-optimization]] · [[software-factory]]
