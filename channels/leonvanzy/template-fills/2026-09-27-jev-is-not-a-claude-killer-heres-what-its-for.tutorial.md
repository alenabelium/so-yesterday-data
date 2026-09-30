---
video_id: iyIAdmeKeMM
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-09-27-jev-is-not-a-claude-killer-heres-what-its-for.md
source_transcript: ../transcripts/2026-09-27-jev-is-not-a-claude-killer-heres-what-its-for.md
source_summary_hash: sha256:be9131c6a3d3473d99b2c3d18098b95a0d3603547e12a88862f64287815a165b
source_transcript_hash: sha256:3e37f6733280849fb62d12ae3eadff992c912652b2adc44edb3fc54672782492
fill_id: b048028e-ac6a-4626-9948-10cf3452cbeb
published_at: '2026-09-30T07:16:05.428736'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Use Jeff from TypeSafe AI for instant, low-cost classification tasks like routing GitHub issues to coding agents.

## Prerequisites

### OpenRouter Account
- **Kind**: account
- **Note**: Required to bypass the TypeSafe waitlist and access Jeff via API.

### GitHub Repository
- **Kind**: tool
- **Note**: A repo to connect to the software factory workflow for automated issue tagging.

## Steps

### Access Jeff via OpenRouter
- **Timestamp**: [08:02](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=482)
- **Action**: Bypass the TypeSafe waitlist by registering on OpenRouter, which provides access to the latest version of Jeff.
- **Command Or Clicks**: Register account at OpenRouter and select Jeff as the model provider.
- **Choice Branch**: Use TypeSafe directly if you have an account; otherwise use OpenRouter.

### Generate API Key
- **Timestamp**: [09:01](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=541)
- **Action**: Navigate to the API keys section in the dashboard, create a new key named 'tutorial', and save it securely.
- **Command Or Clicks**: Dashboard > API Keys > Create New Key (name: tutorial) > Copy Key.
- **Choice Branch**: Ensure you have credits added; free $5 credit is often available upon signup.

### Clone and Setup Repo
- **Timestamp**: [10:01](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=601)
- **Action**: Clone the provided code repository into your project root folder using Claude Code to prepare for integration.
- **Command Or Clicks**: Claude Code: 'Install Opus 5.5... Clone [GitHub URL] to root folder.'
- **Choice Branch**: You can use an existing repo or create a new test repository.

### Define Agent Labels
- **Timestamp**: [11:20](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=680)
- **Action**: Instruct the coding agent to add specific tags to the GitHub repository for routing, such as labels for different AI agents.
- **Command Or Clicks**: Claude Code: 'Create a new private GitHub repository... Please add these tags: Claude Fable, Codex Astra, Claude Haiku.'
- **Choice Branch**: Customize tags based on your specific agent swarm needs.

### Install TypeSafe Skill
- **Timestamp**: [12:48](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=768)
- **Action**: Copy the URL for the official TypeSafe agent skill and install it in the project folder to teach the agent how to use Jeff.
- **Command Or Clicks**: Copy GitHub repo URL > Return to agent > Install skill in project folder.
- **Choice Branch**: Link to community repo provided in video description.

### Configure GitHub Action
- **Timestamp**: [13:36](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=816)
- **Action**: Instruct the agent to create a GitHub Action that calls Jeff on new issues to classify them and assign agents.
- **Command Or Clicks**: Claude Code: 'Every time we add a new task... Jive needs to be called via a GitHub Action... Add comment showing input/response.'
- **Choice Branch**: Define confidence thresholds (e.g., <0.75 for human review) in the logic.

### Test Workflow
- **Timestamp**: [14:30](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=870)
- **Action**: Create a new issue to verify that Jeff classifies the task, assigns an agent, and posts a comment with confidence scores.
- **Command Or Clicks**: GitHub UI: Create Issue 'add a new emotion - frightened' > Check comments for Jeff's response.
- **Choice Branch**: Review confidence scores; low scores may indicate ambiguity requiring human review.

## Gotchas

### Jeff cannot write complete sentences or reason like Claude; it is strictly for classification, scoring, or zero/one decisions.
- **Severity**: serious
- **Timestamp**: [02:38](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=158)

### The context window is tiny (~32k tokens), so do not send large amounts of data to Jeff.
- **Severity**: serious
- **Timestamp**: [03:35](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=215)

### Do not use Jeff for tasks requiring mathematical or scientific accuracy; it is not designed for complex reasoning.
- **Severity**: blocking
- **Timestamp**: [06:49](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=409)

## Where to go next

Join Agentyc Labs for the coding masterclass and live sessions on building software factories with AI agents. Check the description for links to the TypeSafe skill repo and community.

## Concepts surfaced

[[system-1-vs-system-2]] · [[github-actions-automation]] · [[ai-agent-routing]] · [[cost-efficient-llm]]
