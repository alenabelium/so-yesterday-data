---
video_id: iyIAdmeKeMM
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-09-27-jev-is-not-a-claude-killer-heres-what-its-for.md
source_transcript: ../transcripts/2026-09-27-jev-is-not-a-claude-killer-heres-what-its-for.md
source_summary_hash: sha256:be9131c6a3d3473d99b2c3d18098b95a0d3603547e12a88862f64287815a165b
source_transcript_hash: sha256:3e37f6733280849fb62d12ae3eadff992c912652b2adc44edb3fc54672782492
fill_id: fca32c05-c083-4e29-a2da-5cffa61b2049
published_at: '2026-09-29T21:11:54.851595'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Use Jeff from TypeSafe AI for instant, low-cost classification tasks like routing GitHub issues to coding agents.

## Prerequisites

### OpenRouter Account
- **Kind**: account
- **Note**: Sign up to bypass TypeSafe's waiting list and access the Jeff API.

### GitHub Repository
- **Kind**: tool
- **Note**: A repo with issues to classify, such as a web app or test project.

### Claude Code Agent
- **Kind**: tool
- **Note**: Used to clone repos and generate GitHub Actions workflows for automation.

## Steps

### Understand Jeff's Use Case
- **Timestamp**: [00:54](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=54)
- **Action**: Recognize that Jeff is a 'System 1' model designed for instant, deterministic classification (choice, score, or zero) rather than complex reasoning.
- **Command Or Clicks**: N/A

### Access Jeff via OpenRouter
- **Timestamp**: [08:02](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=482)
- **Action**: Register on OpenRouter to bypass the TypeSafe waiting list and obtain API access.
- **Command Or Clicks**: N/A

### Generate API Key
- **Timestamp**: [09:01](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=541)
- **Action**: Navigate to the TypeSafe dashboard, go to API keys, create a new key named 'tutorial', and save it securely.
- **Command Or Clicks**: N/A

### Clone Project Repository
- **Timestamp**: [10:01](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=601)
- **Action**: Use Claude Code to clone a GitHub repository into the project root folder.
- **Command Or Clicks**: I will install Opus 5.5 and a high level of logical reasoning. Please clone this repository into the root folder of the project and I will just paste this GitHub URL there.

### Create Private Repo
- **Timestamp**: [10:45](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=645)
- **Action**: Instruct Claude Code to create a new private GitHub repository for the project.
- **Command Or Clicks**: "Create a new private GitHub repository for this project."

### Define Custom Tags
- **Timestamp**: [11:20](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=680)
- **Action**: Ask the agent to add specific tags to the repo, such as agent names (Fable, Codex, Haiku).
- **Command Or Clicks**: "Please add these tags to the GitHub repository. And let it be Claude from Fable, Codex from Astra, and maybe Claude from Haiku for very simple tasks."

### Install TypeSafe Skill
- **Timestamp**: [12:48](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=768)
- **Action**: Copy the URL for the official TypeSafe agent skill and install it in the project folder.
- **Command Or Clicks**: N/A

### Configure GitHub Action
- **Timestamp**: [13:36](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=816)
- **Action**: Instruct Claude Code to push a GitHub Action that calls Jeff on new issues for classification and agent assignment.
- **Command Or Clicks**: "Every time we add a new task... Jive needs to be called via a GitHub Action... Add a comment showing Jev's input and response, as well as the confidence score... And then we can just settle on a type-safe API key."

### Test Classification
- **Timestamp**: [14:30](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=870)
- **Action**: Create a new issue to verify Jeff's classification and agent routing logic.
- **Command Or Clicks**: "add a new emotion— frightened."

## Gotchas

### Jeff cannot reason or write complete sentences; it is strictly for fast, deterministic classification tasks like choice, score, or zero.
- **Severity**: blocking
- **Timestamp**: [02:38](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=158)

### TypeSafe currently has a waiting list; use OpenRouter as an alternative access point if you cannot join immediately.
- **Severity**: heads_up
- **Timestamp**: [08:02](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=482)

### If the confidence score is below 0.75, implement logic to pass the task to a human for review rather than auto-routing.
- **Severity**: serious
- **Timestamp**: [05:35](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=335)

## Where to go next

Join Agentyc Labs for the coding masterclass and live sessions. Next Thursday features a deep dive into JFA I. Links are in the description.

## Concepts surfaced

[[system-1-vs-system-2]] · [[deterministic-output]] · [[github-actions-automation]] · [[cost-efficient-ai]]
