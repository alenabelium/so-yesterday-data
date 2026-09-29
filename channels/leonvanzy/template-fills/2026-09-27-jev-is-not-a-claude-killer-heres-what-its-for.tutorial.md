---
video_id: iyIAdmeKeMM
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-09-27-jev-is-not-a-claude-killer-heres-what-its-for.md
source_transcript: ../transcripts/2026-09-27-jev-is-not-a-claude-killer-heres-what-its-for.md
source_summary_hash: sha256:be9131c6a3d3473d99b2c3d18098b95a0d3603547e12a88862f64287815a165b
source_transcript_hash: sha256:3e37f6733280849fb62d12ae3eadff992c912652b2adc44edb3fc54672782492
fill_id: 79fe7179-8e2e-4bdb-a83e-f75143276c1f
published_at: '2026-09-29T19:11:54.420298'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Use Jeff for instant, low-cost classification tasks like routing GitHub issues to specific coding agents.

## Prerequisites

### OpenRouter Account
- **Kind**: account
- **Note**: Sign up to bypass TypeSafe's waiting list and access the Jeff API.

### GitHub Repository
- **Kind**: tool
- **Note**: A repo to connect to the software factory workflow for issue classification.

### Claude Code Agent
- **Kind**: tool
- **Note**: Used to clone repos and generate GitHub Actions via natural language.

## Steps

### Access Jeff via OpenRouter
- **Timestamp**: [08:02](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=482)
- **Action**: Bypass the TypeSafe waiting list by registering on OpenRouter, which provides access to the latest version of Jeff.
- **Command Or Clicks**: Register at OpenRouter and select 'Jeff' as the model provider.
- **Choice Branch**: Use TypeSafe directly if you have an account, or OpenRouter to skip the waitlist.

### Generate API Key
- **Timestamp**: [09:01](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=541)
- **Action**: Navigate to the API keys section in the dashboard and create a new key for authentication.
- **Command Or Clicks**: Go to 'API keys' > Create New Key > Copy and save securely.
- **Choice Branch**: Ensure you add credits to your account as this is a paid service.

### Clone Repository
- **Timestamp**: [10:01](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=601)
- **Action**: Use an agent to clone the target GitHub repository into your local project root.
- **Command Or Clicks**: Copy repo URL > Paste into Claude Code: 'clone this repository into the root folder'
- **Choice Branch**: You can use any existing repo or create a new test repository.

### Define Classification Labels
- **Timestamp**: [11:02](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=662)
- **Action**: Instruct the agent to add specific tags to the GitHub repository for categorization.
- **Command Or Clicks**: Ask agent: 'Please add these tags: bug, documentation, enhancement, claude-opus, codex-astra, claude-haiku'
- **Choice Branch**: Customize labels based on your team's needs (e.g., billing vs technical support).

### Install TypeSafe Skill
- **Timestamp**: [12:48](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=768)
- **Action**: Download the official TypeSafe agent skill to teach the coding agent how to use Jeff's API.
- **Command Or Clicks**: Copy GitHub URL > Install skill in project folder via agent command.
- **Choice Branch**: This skill handles the technical integration of the API calls.

### Configure GitHub Action
- **Timestamp**: [13:36](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=816)
- **Action**: Set up a workflow to call Jeff on every new issue, classify it, and assign an agent.
- **Command Or Clicks**: Ask agent: 'Create GitHub Action to call Jeff on new issues, add labels, and post confidence scores.'
- **Choice Branch**: Route complex tasks to Opus, spatial tasks to Codex Astra, and docs to Haiku.

### Test the Workflow
- **Timestamp**: [14:30](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=870)
- **Action**: Create a new issue to verify Jeff classifies the type and assigns the correct agent.
- **Command Or Clicks**: Create GitHub Issue > Check comments for Jeff's classification and confidence score.
- **Choice Branch**: Review confidence scores; if low, consider human review or re-prompting.

## Gotchas

### Jeff cannot write complete sentences or reason like Claude; it is strictly for instant classification tasks.
- **Severity**: blocking
- **Timestamp**: [02:38](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=158)

### The output structure is deterministic, providing confidence scores that can trigger human review if below a threshold.
- **Severity**: heads_up
- **Timestamp**: [05:35](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=335)

### Jeff has a tiny context window of about 32,000 tokens and cannot handle complex math or science tasks.
- **Severity**: serious
- **Timestamp**: [02:38](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=158)

## Where to go next

Join Agentyc Labs for the 'Agentyc Coding masterclass' and live sessions on building software factories with AI agents. Next Thursday features a deep dive into JFAI.

## Concepts surfaced

[[system-1-vs-system-2-ai]] · [[github-issue-routing]] · [[deterministic-llm-output]] · [[cost-efficient-ai-workflows]] · [[software-factory-architecture]]
