---
video_id: iyIAdmeKeMM
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-09-27-jev-is-not-a-claude-killer-heres-what-its-for.md
source_transcript: ../transcripts/2026-09-27-jev-is-not-a-claude-killer-heres-what-its-for.md
source_summary_hash: sha256:be9131c6a3d3473d99b2c3d18098b95a0d3603547e12a88862f64287815a165b
source_transcript_hash: sha256:3e37f6733280849fb62d12ae3eadff992c912652b2adc44edb3fc54672782492
fill_id: 738c5a5d-0fc5-48f4-9740-843278fc56aa
published_at: '2026-09-29T13:12:03.160204'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Use Jeff for instant, low-cost classification tasks like routing GitHub issues to specialized coding agents.

## Prerequisites

### OpenRouter Account
- **Kind**: account
- **Note**: Sign up to bypass TypeSafe's waiting list and access Jeff via the OpenRouter API.

### GitHub Repository
- **Kind**: tool
- **Note**: A repository with issues to classify, such as a web app or test project.

### Claude Code Agent
- **Kind**: tool
- **Note**: Used to clone repos and generate the necessary GitHub Action workflow files.

## Steps

### Access Jeff via OpenRouter
- **Timestamp**: [08:02](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=482)
- **Action**: Bypass the TypeSafe waiting list by registering an account on OpenRouter, which provides access to the latest version of Jeff.
- **Command Or Clicks**: Register at OpenRouter and select Jeff as the model provider.
- **Choice Branch**: You can also use the TypeSafe dashboard directly if you have access.

### Generate API Key
- **Timestamp**: [09:01](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=541)
- **Action**: Navigate to the API keys section in your provider's dashboard and create a new key for authentication.
- **Command Or Clicks**: Go to API keys > Create New Key > Name it 'tutorial' > Copy and save securely.
- **Choice Branch**: Ensure you add credits if using a paid tier, though free tiers may be available.

### Clone Project Repository
- **Timestamp**: [10:01](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=601)
- **Action**: Use your coding agent to clone the example repository containing the 3D model web app.
- **Command Or Clicks**: Open Claude Code > Install Opus 5.5 > Paste GitHub URL to clone into root folder.
- **Choice Branch**: You can use any existing repo or create a new test repository.

### Define Agent Labels
- **Timestamp**: [11:02](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=662)
- **Action**: Instruct the agent to add specific labels to the GitHub repository for routing purposes.
- **Command Or Clicks**: Prompt agent: 'Please add these tags: Claude Fable, Codex Astra, Claude Haiku.'
- **Choice Branch**: Customize labels based on your team's needs (e.g., bug, docs, enhancement).

### Install TypeSafe Skill
- **Timestamp**: [12:48](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=768)
- **Action**: Add the official TypeSafe agent skill to teach the coding agent how to interact with Jeff's API.
- **Command Or Clicks**: Copy GitHub URL for the skill > Install in project folder via agent.
- **Choice Branch**: Link to the community repo is provided in the video description.

### Configure GitHub Action
- **Timestamp**: [13:36](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=816)
- **Action**: Create a workflow that calls Jeff on new issues to classify them and assign agents.
- **Command Or Clicks**: Prompt agent to create GitHub Action: call Jeff, add labels (improvement/error/docs), assign agent, post comment with confidence score.
- **Choice Branch**: Set confidence thresholds for human review if needed.

### Test the Workflow
- **Timestamp**: [14:30](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=870)
- **Action**: Create a new issue to verify that Jeff classifies it correctly and assigns the appropriate agent.
- **Command Or Clicks**: Create issue 'add new emotion - frightened' > Check comments for classification and confidence scores.
- **Choice Branch**: Review confidence scores; low scores may indicate ambiguity.

## Gotchas

### Jeff is a System 1 model, not a reasoning model. It cannot write complete sentences or handle complex logic/science tasks.
- **Severity**: serious
- **Timestamp**: [02:38](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=158)

### Jeff has a tiny context window of about 32,000 tokens. Do not exceed this limit in your queries.
- **Severity**: blocking
- **Timestamp**: [02:38](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=158)

### Do not use Jeff for tasks requiring mathematical accuracy or scientific reasoning; use Claude or OpenAI instead.
- **Severity**: serious
- **Timestamp**: [05:35](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=335)

## Where to go next

Join Agentyc Labs for the coding masterclass and live sessions on building software factories. Next Thursday features a deep dive into JFA I.

## Concepts surfaced

[[system-1-vs-system-2]] · [[github-actions]] · [[agent-routing]] · [[cost-optimization]]
