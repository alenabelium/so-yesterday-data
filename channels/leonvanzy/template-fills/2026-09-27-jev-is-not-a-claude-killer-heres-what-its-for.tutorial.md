---
video_id: iyIAdmeKeMM
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-09-27-jev-is-not-a-claude-killer-heres-what-its-for.md
source_transcript: ../transcripts/2026-09-27-jev-is-not-a-claude-killer-heres-what-its-for.md
source_summary_hash: sha256:be9131c6a3d3473d99b2c3d18098b95a0d3603547e12a88862f64287815a165b
source_transcript_hash: sha256:3e37f6733280849fb62d12ae3eadff992c912652b2adc44edb3fc54672782492
fill_id: 7739efd7-ff81-41cf-85c1-e7c7eef27b33
published_at: '2026-09-30T03:16:35.325706'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Use TypeSafe AI's Jeff model for low-cost, high-speed classification tasks like routing GitHub issues to specific coding agents.

## Prerequisites

### OpenRouter Account
- **Kind**: account
- **Note**: Required to access Jeff without the TypeSafe waitlist.

### GitHub Repository
- **Kind**: tool
- **Note**: A repo with issues to classify and route via automation.

### Claude Code Agent
- **Kind**: tool
- **Note**: Used in the demo to generate the GitHub Actions workflow code.

## Steps

### Understand Jeff's Use Case
- **Timestamp**: [00:54](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=54)
- **Action**: Recognize that Jeff is a System 1 model for instant, low-cost classification (choice, score, zero) rather than complex reasoning.
- **Command Or Clicks**: N/A

### Access Jeff via OpenRouter
- **Timestamp**: [08:02](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=482)
- **Action**: Bypass the TypeSafe waitlist by registering on OpenRouter and selecting the latest version of Jeff.
- **Command Or Clicks**: N/A

### Generate API Key in Playground
- **Timestamp**: [09:01](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=541)
- **Action**: Navigate to the TypeSafe AI dashboard, go to API keys, create a new key named 'tutorial', and save it securely.
- **Command Or Clicks**: N/A

### Clone Demo Repository
- **Timestamp**: [10:01](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=601)
- **Action**: Use Claude Code to clone the provided GitHub repository into your project root folder.
- **Command Or Clicks**: clone <github-url>

### Create Private Repo and Add Tags
- **Timestamp**: [11:02](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=662)
- **Action**: Instruct the agent to create a new private GitHub repository and add specific tags for agents (e.g., Codex, Haiku).
- **Command Or Clicks**: "Create a new private GitHub repository..." "Please add these tags..."

### Install TypeSafe Agent Skill
- **Timestamp**: [12:48](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=768)
- **Action**: Copy the URL for the official TypeSafe agent skill and install it in your project folder to teach the agent how to use Jeff.
- **Command Or Clicks**: install <skill-url>

### Configure GitHub Action Logic
- **Timestamp**: [13:36](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=816)
- **Action**: Ask the agent to write a GitHub Action that classifies issues, assigns agents based on tags, and comments with Jeff's response and confidence scores.
- **Command Or Clicks**: "Every time we add a new task... Jive needs to be called via a GitHub Action..."

### Test the Workflow
- **Timestamp**: [14:30](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=870)
- **Action**: Create a new issue in the repository and verify that Jeff correctly classifies it (e.g., as 'improvement') and assigns an agent.
- **Command Or Clicks**: N/A

## Gotchas

### Jeff cannot write complete sentences or reason; it is strictly for classification tasks like choice, score, or zero.
- **Severity**: serious
- **Timestamp**: [02:38](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=158)

### Use confidence scores to route uncertain predictions (e.g., below 0.75) to human review rather than automated agents.
- **Severity**: heads_up
- **Timestamp**: [05:35](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=335)

## Where to go next

Join Agentyc Labs for the coding masterclass and live sessions on building software factories with AI agents. Check the description for links to the TypeSafe skill repo and Agentyc community.

## Concepts surfaced

[[system-1-ai]] · [[github-actions-automation]] · [[cost-efficient-llm-routing]] · [[deterministic-json-output]]
