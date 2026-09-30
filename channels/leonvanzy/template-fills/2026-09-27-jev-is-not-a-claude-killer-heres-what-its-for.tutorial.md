---
video_id: iyIAdmeKeMM
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-09-27-jev-is-not-a-claude-killer-heres-what-its-for.md
source_transcript: ../transcripts/2026-09-27-jev-is-not-a-claude-killer-heres-what-its-for.md
source_summary_hash: sha256:be9131c6a3d3473d99b2c3d18098b95a0d3603547e12a88862f64287815a165b
source_transcript_hash: sha256:3e37f6733280849fb62d12ae3eadff992c912652b2adc44edb3fc54672782492
fill_id: 28d75c05-95e8-40f7-ab25-3319cdc39a1c
published_at: '2026-09-30T01:17:39.714950'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Use Jeff for instant, low-cost classification and routing in GitHub workflows instead of expensive reasoning models.

## Prerequisites

### OpenRouter Account
- **Kind**: account
- **Note**: Sign up to bypass TypeSafe's waiting list and access Jeff via their API.

### GitHub Repository
- **Kind**: tool
- **Note**: A repo with issues to classify, such as a test project or existing codebase.

### Claude Code Agent
- **Kind**: tool
- **Note**: Used to clone repos, create tags, and generate GitHub Actions via CLI.

## Steps

### Access Jeff via OpenRouter
- **Timestamp**: [08:02](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=482)
- **Action**: Bypass the TypeSafe waiting list by registering on OpenRouter, which provides access to the latest version of Jeff.
- **Command Or Clicks**: Register at OpenRouter and select Jeff as the model provider.

### Generate API Key
- **Timestamp**: [09:01](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=541)
- **Action**: Navigate to the TypeSafe dashboard, go to API keys, create a new key named 'tutorial', and save it securely.
- **Command Or Clicks**: Dashboard > API Keys > Create New Key > Copy Key

### Clone Project Repository
- **Timestamp**: [10:01](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=601)
- **Action**: Use Claude Code to clone the demonstration repository into your local project root.
- **Command Or Clicks**: Claude Code: 'Clone [GitHub URL] into the root folder'

### Create GitHub Repository
- **Timestamp**: [10:45](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=645)
- **Action**: Instruct Claude Code to create a new private GitHub repository for the project.
- **Command Or Clicks**: Claude Code: 'Create a new private GitHub repository'

### Add Custom Tags
- **Timestamp**: [11:20](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=680)
- **Action**: Ask the agent to add specific tags like 'Claude Opus', 'Codex Astra', and 'Claude Haiku' to the repository.
- **Command Or Clicks**: Claude Code: 'Add these tags: Claude Opus, Codex Astra, Claude Haiku'

### Install TypeSafe Skill
- **Timestamp**: [12:48](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=768)
- **Action**: Copy the URL for the official TypeSafe agent skill and install it in the project folder to teach the agent how to use Jeff.
- **Command Or Clicks**: Clone TypeSafe skill repo into project folder

### Configure GitHub Action
- **Timestamp**: [13:36](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=816)
- **Action**: Instruct Claude Code to push changes that call Jeff via GitHub Action on new issues, assigning labels and agents based on classification.
- **Command Or Clicks**: Claude Code: 'Push changes to GitHub with Jeff integration logic'

### Test Workflow
- **Timestamp**: [14:30](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=870)
- **Action**: Create a new issue in the repository and verify that Jeff classifies it, assigns an agent, and posts a comment with confidence scores.
- **Command Or Clicks**: Create Issue: 'Add new emotion frightened'

## Gotchas

### Jeff cannot write complete sentences or reason; it is strictly for classification, scoring, or boolean decisions.
- **Severity**: blocking
- **Timestamp**: [02:38](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=158)

### Use confidence scores to route low-confidence results (<0.75) to human review rather than automated agents.
- **Severity**: serious
- **Timestamp**: [05:35](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=335)

## Where to go next

Join Agentyc Labs for the coding masterclass and live sessions on building software factories with AI agents.

## Concepts surfaced

[[system-1-vs-system-2]] · [[github-actions]] · [[ai-classification]] · [[cost-optimization]]
