---
video_id: iyIAdmeKeMM
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-09-27-jev-is-not-a-claude-killer-heres-what-its-for.md
source_transcript: ../transcripts/2026-09-27-jev-is-not-a-claude-killer-heres-what-its-for.md
source_summary_hash: sha256:be9131c6a3d3473d99b2c3d18098b95a0d3603547e12a88862f64287815a165b
source_transcript_hash: sha256:3e37f6733280849fb62d12ae3eadff992c912652b2adc44edb3fc54672782492
fill_id: 568acc15-ba44-47ab-bda4-4946bc10641f
published_at: '2026-09-29T22:18:17.926972'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Use Jeff for instant, low-cost classification tasks like routing GitHub issues to coding agents.

## Prerequisites

### TypeSafe AI or OpenRouter Account
- **Kind**: account
- **Note**: Sign up for TypeSafe AI (may have waitlist) or use OpenRouter to access Jeff.

### GitHub Repository
- **Kind**: tool
- **Note**: A repository to connect to the software factory workflow for issue classification.

### API Key
- **Kind**: tool
- **Note**: Generate a new API key in the TypeSafe dashboard and save it securely.

## Steps

### Understand Jeff's Role
- **Timestamp**: [00:54](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=54)
- **Action**: Recognize Jeff as a System 1 model for instant classification, not complex reasoning.

### Access Jeff via OpenRouter
- **Timestamp**: [08:02](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=482)
- **Action**: Bypass TypeSafe waitlist by registering on OpenRouter to access the latest Jeff version.

### Generate API Key
- **Timestamp**: [09:01](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=541)
- **Action**: Create a new API key in the TypeSafe dashboard and save it safely.

### Clone Repository
- **Timestamp**: [10:01](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=601)
- **Action**: Clone a test repository to use for the software factory demo.
- **Command Or Clicks**: git clone <repository-url>

### Add Custom Tags
- **Timestamp**: [11:20](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=680)
- **Action**: Ask your coding agent to add specific tags like Claude Opus, Codex Astra, and Claude Haiku.

### Install TypeSafe Skill
- **Timestamp**: [12:48](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=768)
- **Action**: Install the official TypeSafe agent skill to teach the agent how to use Jeff APIs.

### Configure GitHub Action
- **Timestamp**: [13:36](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=816)
- **Action**: Set up a GitHub Action to call Jeff on new issues for classification and agent assignment.

### Test Workflow
- **Timestamp**: [14:30](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=870)
- **Action**: Create a new issue to verify Jeff classifies it and assigns the correct agent.

## Gotchas

### Jeff cannot reason or write complete sentences; it is only for classification, scoring, or boolean decisions.
- **Severity**: blocking
- **Timestamp**: [02:38](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=158)

### Use confidence scores to route uncertain classifications to humans if the score is below 0.75.
- **Severity**: serious
- **Timestamp**: [05:35](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=335)

### Jeff has a tiny context window of about 32,000 tokens and cannot handle complex tasks.
- **Severity**: blocking
- **Timestamp**: [02:38](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=158)

## Where to go next

Join Agentyc Labs for the coding masterclass and live sessions on building software factories with AI agents.

## Concepts surfaced

[[system-1-vs-system-2]] · [[github-actions]] · [[software-factory]] · [[api-classification]]
