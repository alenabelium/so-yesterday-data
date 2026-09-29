---
video_id: iyIAdmeKeMM
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-09-27-jev-is-not-a-claude-killer-heres-what-its-for.md
source_transcript: ../transcripts/2026-09-27-jev-is-not-a-claude-killer-heres-what-its-for.md
source_summary_hash: sha256:be9131c6a3d3473d99b2c3d18098b95a0d3603547e12a88862f64287815a165b
source_transcript_hash: sha256:3e37f6733280849fb62d12ae3eadff992c912652b2adc44edb3fc54672782492
fill_id: 87668b50-8960-48bb-a2ca-aa43456ff807
published_at: '2026-09-29T16:11:38.661636'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Use Jeff from TypeSafe AI for instant, low-cost classification tasks like routing GitHub issues to specific coding agents.

## Prerequisites

### TypeSafe AI or OpenRouter Account
- **Kind**: account
- **Note**: Sign up for TypeSafe AI (waiting list may apply) or use OpenRouter to access the Jeff API.

### GitHub Repository
- **Kind**: tool
- **Note**: A GitHub repo is needed to connect the workflow and test the automated issue classification.

### API Key
- **Kind**: tool
- **Note**: Generate a new API key in the TypeSafe dashboard playground to authenticate requests.

## Steps

### Understand Jeff's Role and Cost Benefits
- **Timestamp**: [00:54](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=54)
- **Action**: Recognize that Jeff is a 'System 1' model designed for instant, deterministic classification (choice, score, zero) rather than complex reasoning. It costs significantly less than models like Claude or Sonnet for high-volume tasks.

### Access Jeff via OpenRouter
- **Timestamp**: [08:02](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=482)
- **Action**: Bypass the TypeSafe AI waiting list by registering on OpenRouter. Use the OpenRouter API endpoint to access the latest version of Jeff for this tutorial.

### Generate an API Key
- **Timestamp**: [09:01](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=541)
- **Action**: Navigate to the TypeSafe AI dashboard, go to 'API keys', create a new key named 'tutorial', and save it securely. Add credits if necessary.

### Clone Project Repository
- **Timestamp**: [10:01](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=601)
- **Action**: Open your coding agent (e.g., Claude Code), install the necessary model, and clone the provided GitHub repository into your project root folder.

### Create GitHub Repository and Labels
- **Timestamp**: [11:02](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=662)
- **Action**: Create a new private GitHub repository. Use your coding agent to add specific labels (e.g., error, documentation, enhancement) and custom agent tags (Claude Opus, Codex Astra, Claude Haiku).

### Install TypeSafe Agent Skill
- **Timestamp**: [12:48](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=768)
- **Action**: Copy the URL for the official TypeSafe agent skill from GitHub and install it in your project folder to teach your agent how to use Jeff's API.

### Configure GitHub Action via Agent
- **Timestamp**: [13:36](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=816)
- **Action**: Instruct your coding agent to create a GitHub Action that calls Jeff on new issues. Specify the logic: classify as bug/docs/enhancement, assign agent (Opus/Astra/Haiku), and add a comment with input/response/confidence.

### Test the Workflow
- **Timestamp**: [14:30](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=870)
- **Action**: Create a new issue in the repository. Observe Jeff's response, which should automatically label the issue and assign an agent based on the content, including a confidence score.

## Gotchas

### Jeff cannot write complete sentences or reason like Claude. It is strictly for classification tasks (choice, score, zero) with deterministic output structures.
- **Severity**: serious
- **Timestamp**: [02:38](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=158)

### Do not use Jeff for complex scientific/mathematical reasoning or tasks requiring high intelligence; it has a tiny context window (~32k tokens) and is bad at those areas.
- **Severity**: serious
- **Timestamp**: [03:35](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=215)

### Check the confidence score in Jeff's response. If it is below 0.75, implement logic to pass the task to a human for review rather than auto-routing.
- **Severity**: heads_up
- **Timestamp**: [05:35](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=335)

## Where to go next

Explore building a full 'software factory' workflow using these classifications. Join Agentyc Labs for masterclasses on effectively using agents for coding and real-world project creation.

## Concepts surfaced

[[system-1-vs-system-2-ai]] · [[automated-issue-routing]] · [[cost-efficient-llm-workflows]] · [[deterministic-ai-output]] · [[github-action-automation]]
