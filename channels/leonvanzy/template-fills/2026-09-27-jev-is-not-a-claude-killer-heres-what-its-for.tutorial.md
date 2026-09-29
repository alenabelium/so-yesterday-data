---
video_id: iyIAdmeKeMM
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-09-27-jev-is-not-a-claude-killer-heres-what-its-for.md
source_transcript: ../transcripts/2026-09-27-jev-is-not-a-claude-killer-heres-what-its-for.md
source_summary_hash: sha256:be9131c6a3d3473d99b2c3d18098b95a0d3603547e12a88862f64287815a165b
source_transcript_hash: sha256:3e37f6733280849fb62d12ae3eadff992c912652b2adc44edb3fc54672782492
fill_id: 67d08fd8-46be-4c3c-8b42-79f05a45d1ea
published_at: '2026-09-29T15:11:40.758430'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Use Jeff for instant, low-cost classification and routing instead of expensive reasoning models.

## Prerequisites

### OpenRouter Account
- **Kind**: account
- **Note**: Bypasses TypeSafe waitlist to access Jeff via API.

### GitHub Repository
- **Kind**: tool
- **Note**: Required for the software factory workflow and issue tagging.

### Claude Code Agent
- **Kind**: tool
- **Note**: Used to clone repo, create labels, and push GitHub Actions.

## Steps

### Access Jeff via OpenRouter
- **Timestamp**: [08:02](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=482)
- **Action**: Sign up for an OpenRouter account to bypass the TypeSafe AI waitlist and gain access to the latest version of Jeff.
- **Command Or Clicks**: Navigate to OpenRouter, register, and select Jeff as your model provider.

### Generate API Key
- **Timestamp**: [09:01](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=541)
- **Action**: Create a new API key in the TypeSafe dashboard and add credits to your account to enable usage.
- **Command Or Clicks**: Go to API keys > Create New Key > Copy key > Add credits.

### Setup Repository Environment
- **Timestamp**: [10:01](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=601)
- **Action**: Clone a test repository and create a new private GitHub repo for the project using your coding agent.
- **Command Or Clicks**: git clone <URL> && Create a new private GitHub repository for this project.

### Define Agent Labels
- **Timestamp**: [11:20](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=680)
- **Action**: Add specific labels to the repo (e.g., claude-opus, codex-astra, claude-haiku) to categorize different types of work.
- **Command Or Clicks**: Please add these tags to the GitHub repository: claude-opus, codex-astra, claude-haiku.

### Install TypeSafe Skill
- **Timestamp**: [12:48](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=768)
- **Action**: Clone the official TypeSafe agent skill repository into your project folder to teach the agent how to use Jeff's APIs.
- **Command Or Clicks**: git clone <TypeSafeSkillURL> ./skills/typesafe

### Configure GitHub Action
- **Timestamp**: [13:36](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=816)
- **Action**: Instruct the agent to create a GitHub Action that calls Jeff on new issues to classify them and assign agents.
- **Command Or Clicks**: Create GitHub Action workflow file calling Jeff API with choice/score types.

### Test Classification Workflow
- **Timestamp**: [14:30](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=870)
- **Action**: Create a new issue to verify that Jeff correctly tags it, assigns an agent, and posts a comment with the confidence score.
- **Command Or Clicks**: Create new issue: 'add a new emotion frightened'.

## Gotchas

### Jeff cannot reason or write complex sentences; it is strictly for classification, scoring, and boolean decisions.
- **Severity**: blocking
- **Timestamp**: [02:38](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=158)

### Do not use Jeff for tasks requiring mathematical accuracy or scientific reasoning; use Claude instead.
- **Severity**: serious
- **Timestamp**: [05:35](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=335)

### Check the confidence score; if it is below 0.75, route the task to a human for review rather than auto-processing.
- **Severity**: heads_up
- **Timestamp**: [05:35](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=335)

## Where to go next

Join Agentyc Labs for the coding masterclass and next Thursday's deep dive into JFAI. See how to build a full software factory with agent swarms.

## Concepts surfaced

[[system-1-vs-system-2]] · [[cost-efficient-classification]] · [[github-actions-automation]] · [[agent-routing]] · [[confidence-scoring]]
