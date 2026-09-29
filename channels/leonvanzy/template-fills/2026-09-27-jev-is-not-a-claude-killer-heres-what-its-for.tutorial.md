---
video_id: iyIAdmeKeMM
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-09-27-jev-is-not-a-claude-killer-heres-what-its-for.md
source_transcript: ../transcripts/2026-09-27-jev-is-not-a-claude-killer-heres-what-its-for.md
source_summary_hash: sha256:be9131c6a3d3473d99b2c3d18098b95a0d3603547e12a88862f64287815a165b
source_transcript_hash: sha256:3e37f6733280849fb62d12ae3eadff992c912652b2adc44edb3fc54672782492
fill_id: fe1f321e-fe15-4bb1-8fab-8a0fb94162b5
published_at: '2026-09-29T20:11:55.139043'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Use TypeSafe AI's Jeff model for low-cost, high-speed classification tasks like routing GitHub issues to specific coding agents.

## Prerequisites

### TypeSafe AI Account
- **Kind**: account
- **Note**: Sign up at typesafe.ai; may require waiting list or use OpenRouter as alternative access.

### OpenRouter Account
- **Kind**: account
- **Note**: Alternative provider to access Jeff if TypeSafe waitlist is active.

### GitHub Repository
- **Kind**: tool
- **Note**: A repository with issues to classify; clone existing or create new private repo.

### Claude Code Agent
- **Kind**: tool
- **Note**: Used in demo to generate code and GitHub Actions for the classification workflow.

## Steps

### Understand Jeff's Use Case
- **Timestamp**: [00:00](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=0)
- **Action**: Recognize that Jeff is a System 1 model for instant, low-cost classification (choice, score, zero), not a reasoning model like Claude.
- **Command Or Clicks**: None

### Access Jeff via OpenRouter
- **Timestamp**: [08:02](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=482)
- **Action**: Bypass TypeSafe's waiting list by registering on OpenRouter to get access to the latest version of Jeff.
- **Command Or Clicks**: Visit typesafe.ai or OpenRouter and register an account.

### Generate API Key
- **Timestamp**: [09:01](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=541)
- **Action**: Navigate to the API keys section in the TypeSafe dashboard, create a new key named 'tutorial', and save it securely.
- **Command Or Clicks**: Dashboard > API Keys > Create New Key > Copy Key

### Clone Repository
- **Timestamp**: [10:01](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=601)
- **Action**: Open your coding agent (e.g., Claude Code), install Opus 5.5, and clone the demo repository into the project root.
- **Command Or Clicks**: git clone <GitHub_URL>

### Create GitHub Repo & Labels
- **Timestamp**: [11:02](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=662)
- **Action**: Instruct the agent to create a new private GitHub repository and add specific labels like 'error', 'documentation', 'enhancement', 'Claude Opus', 'Codex Astra', and 'Claude Haiku'.
- **Command Or Clicks**: Agent Command: "Create a new private GitHub repository... Add tags: error, documentation, enhancement, Claude Opus, Codex Astra, Claude Haiku"

### Install TypeSafe Skill
- **Timestamp**: [12:48](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=768)
- **Action**: Copy the URL for the official TypeSafe agent skill repository and install it in your project folder to teach the agent how to use Jeff's API.
- **Command Or Clicks**: Clone TypeSafe skill repo into project folder

### Configure GitHub Action
- **Timestamp**: [13:36](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=816)
- **Action**: Instruct the agent to create a GitHub Action that calls Jeff on new issues to classify them as bug/docs/enhancement and assign an agent (Opus/Astra/Haiku) based on confidence scores.
- **Command Or Clicks**: Agent Command: "Create GitHub Action to call TypeSafe API... Add comment with input/response/confidence"

### Test the Workflow
- **Timestamp**: [14:30](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=870)
- **Action**: Create a new issue in the repository to verify that Jeff classifies it correctly, assigns an agent, and posts a comment with the confidence score.
- **Command Or Clicks**: GitHub > New Issue > Write description > Create

## Gotchas

### Jeff cannot write complete sentences or reason; it is strictly for classification, scoring, or boolean decisions.
- **Severity**: blocking
- **Timestamp**: [02:38](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=158)

### Jeff has a tiny context window of about 32,000 tokens and cannot handle complex science/math tasks.
- **Severity**: serious
- **Timestamp**: [02:38](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=158)

### If confidence score is below 0.75, logic should pass the task to a human for review rather than auto-routing.
- **Severity**: heads_up
- **Timestamp**: [05:35](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=335)

## Where to go next

Join Agentyc Labs for the coding masterclass and live sessions on building software factories with AI agents. Next Thursday features a deep dive into JFAI.

## Concepts surfaced

[[system-1-vs-system-2-ai]] · [[github-actions-automation]] · [[llm-cost-optimization]] · [[agent-routing-workflows]]
