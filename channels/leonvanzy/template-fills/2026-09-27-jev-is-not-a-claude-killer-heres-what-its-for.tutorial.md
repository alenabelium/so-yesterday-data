---
video_id: iyIAdmeKeMM
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-09-27-jev-is-not-a-claude-killer-heres-what-its-for.md
source_transcript: ../transcripts/2026-09-27-jev-is-not-a-claude-killer-heres-what-its-for.md
source_summary_hash: sha256:be9131c6a3d3473d99b2c3d18098b95a0d3603547e12a88862f64287815a165b
source_transcript_hash: sha256:3e37f6733280849fb62d12ae3eadff992c912652b2adc44edb3fc54672782492
fill_id: bfeba2fb-9cc6-4cb2-85fa-653ee66d7603
published_at: '2026-09-29T18:11:45.524420'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Use Jeff from TypeSafe AI for instant, low-cost classification and routing tasks instead of expensive reasoning models.

## Prerequisites

### OpenRouter Account
- **Kind**: account
- **Note**: Required to bypass TypeSafe's waiting list and access the Jeff API.

### GitHub Repository
- **Kind**: tool
- **Note**: A repo is needed to test the automated issue classification workflow.

### Claude Code Agent
- **Kind**: tool
- **Note**: Used in the demo to generate code and manage repository changes.

## Steps

### Understand Jeff's Use Case
- **Timestamp**: [00:54](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=54)
- **Action**: Recognize that Jeff is a 'System 1' model designed for instant, deterministic classification (choice, score, or zero) rather than complex reasoning.

### Access Jeff via OpenRouter
- **Timestamp**: [08:02](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=482)
- **Action**: Sign up for OpenRouter to bypass TypeSafe's waiting list and gain access to the latest version of Jeff.

### Generate API Key in Playground
- **Timestamp**: [09:01](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=541)
- **Action**: Navigate to the TypeSafe AI dashboard playground, test a query, switch to JSON view to see the deterministic structure, and create a new API key.

### Clone Project Repository
- **Timestamp**: [10:01](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=601)
- **Action**: Copy the command from the demo code and paste it into your coding agent to clone the repository.

### Define Custom Tags
- **Timestamp**: [11:20](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=680)
- **Action**: Ask your agent to add specific tags to the GitHub repository for routing, such as 'Claude Opus', 'Codex Astra', and 'Claude Haiku'.

### Install TypeSafe Agent Skill
- **Timestamp**: [12:48](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=768)
- **Action**: Copy the URL for the official TypeSafe agent skill and install it in your project folder to teach the agent how to use Jeff.

### Configure GitHub Action Logic
- **Timestamp**: [13:36](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=816)
- **Action**: Instruct your agent to create a GitHub Action that calls Jeff on new issues to classify them and assign agents based on confidence scores.

### Test the Workflow
- **Timestamp**: [14:30](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=870)
- **Action**: Create a new issue in the repository to verify that Jeff correctly classifies the task, assigns an agent, and posts a comment with the response.

## Gotchas

### Jeff cannot reason or write complete sentences; it is strictly for classification tasks like choice, score, or zero.
- **Severity**: blocking
- **Timestamp**: [02:38](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=158)

### TypeSafe currently has a waiting list; use OpenRouter as an alternative access method if you cannot join immediately.
- **Severity**: heads_up
- **Timestamp**: [08:02](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=482)

### If the confidence score is below 0.75, implement logic to pass the request to a human for review rather than auto-processing.
- **Severity**: serious
- **Timestamp**: [05:35](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=335)

## Where to go next

Connect this repository to a real 'software factory' workflow. Join Agentyc Labs for the masterclass on building agent swarms and automating coding pipelines.

## Concepts surfaced

[[system-1-vs-system-2]] · [[deterministic-output]] · [[github-actions-automation]] · [[cost-efficient-ai]]
