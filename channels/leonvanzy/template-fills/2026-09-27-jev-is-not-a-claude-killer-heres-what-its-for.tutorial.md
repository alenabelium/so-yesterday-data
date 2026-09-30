---
video_id: iyIAdmeKeMM
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-09-27-jev-is-not-a-claude-killer-heres-what-its-for.md
source_transcript: ../transcripts/2026-09-27-jev-is-not-a-claude-killer-heres-what-its-for.md
source_summary_hash: sha256:be9131c6a3d3473d99b2c3d18098b95a0d3603547e12a88862f64287815a165b
source_transcript_hash: sha256:3e37f6733280849fb62d12ae3eadff992c912652b2adc44edb3fc54672782492
fill_id: e02b96a7-94d9-4ae9-be1f-dc3a6f847cad
published_at: '2026-09-29T23:17:14.132546'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Use TypeSafe AI's Jeff model for low-cost, high-speed classification and routing in automated software factory workflows.

## Prerequisites

### OpenRouter Account
- **Kind**: account
- **Note**: Sign up to bypass TypeSafe's waiting list and access the Jeff API.

### GitHub Repository
- **Kind**: tool
- **Note**: A repo with issues to classify, such as a test project or existing codebase.

### Claude Code Agent
- **Kind**: tool
- **Note**: Installed locally to clone repos and generate GitHub Actions via CLI.

## Steps

### Access Jeff via OpenRouter
- **Timestamp**: [08:02](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=482)
- **Action**: Bypass the TypeSafe waiting list by registering on OpenRouter, which provides access to the latest version of Jeff.
- **Command Or Clicks**: Navigate to openrouter.ai and register an account.
- **Choice Branch**: Use TypeSafe directly if you have early access, otherwise use OpenRouter.

### Generate API Key
- **Timestamp**: [09:01](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=541)
- **Action**: Create a new API key in the TypeSafe dashboard playground and add credits to your account.
- **Command Or Clicks**: Go to API keys > Create New Key > Copy key > Add credits.
- **Choice Branch**: Use the free $5 credit if available, otherwise purchase more.

### Clone Project Repository
- **Timestamp**: [10:01](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=601)
- **Action**: Open your coding agent and clone a GitHub repository to serve as the base for the automation.
- **Command Or Clicks**: In Claude Code: 'clone this repository into the root folder of the project' [paste URL]
- **Choice Branch**: Use an existing repo or create a new test repository.

### Define Custom Labels
- **Timestamp**: [11:20](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=680)
- **Action**: Instruct your coding agent to add specific labels to the GitHub repository for routing purposes.
- **Command Or Clicks**: In Claude Code: 'Please add these tags to the GitHub repository: Claude Fable, Codex Astra, Claude Haiku'
- **Choice Branch**: Customize labels based on your team's needs.

### Install TypeSafe Agent Skill
- **Timestamp**: [12:48](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=768)
- **Action**: Clone the official TypeSafe agent skill repository into your project folder to teach the agent how to use Jeff.
- **Command Or Clicks**: In Claude Code: 'install this skill in the project folder' [paste GitHub URL]
- **Choice Branch**: Ensure the skill is installed in the root of your project.

### Configure GitHub Action
- **Timestamp**: [13:36](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=816)
- **Action**: Ask the coding agent to create a GitHub Action that calls Jeff on new issues to classify them and assign agents.
- **Command Or Clicks**: In Claude Code: 'push all these changes to GitHub' [after defining prompt logic]
- **Choice Branch**: Define confidence thresholds (e.g., <0.75 for human review).

### Test Automation
- **Timestamp**: [14:30](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=870)
- **Action**: Create a new issue in the repository to verify that Jeff classifies it correctly and adds the appropriate comment.
- **Command Or Clicks**: Create Issue: 'add a new emotion frightened'
- **Choice Branch**: Check the issue comments for Jeff's input, response, and confidence scores.

## Gotchas

### Jeff cannot write complete sentences or reason; it is strictly for classification, scoring, or boolean decisions.
- **Severity**: blocking
- **Timestamp**: [03:35](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=215)

### The API key is paid service; ensure you have credits added to your account before running workflows.
- **Severity**: serious
- **Timestamp**: [10:01](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=601)

### Jeff has a tiny context window of about 32,000 tokens, limiting complex input handling.
- **Severity**: serious
- **Timestamp**: [02:38](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=158)

## Where to go next

Join Agentyc Labs for the coding masterclass and live sessions on building software factories with AI agents. Check the description for links to the TypeSafe skill repo and Decodr sponsor.

## Concepts surfaced

[[system-1-vs-system-2-ai]] · [[automated-issue-routing]] · [[low-cost-llm-classification]] · [[github-actions-automation]] · [[software-factory-workflow]]
