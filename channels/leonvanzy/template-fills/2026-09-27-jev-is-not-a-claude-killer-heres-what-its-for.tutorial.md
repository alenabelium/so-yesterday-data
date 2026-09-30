---
video_id: iyIAdmeKeMM
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-09-27-jev-is-not-a-claude-killer-heres-what-its-for.md
source_transcript: ../transcripts/2026-09-27-jev-is-not-a-claude-killer-heres-what-its-for.md
source_summary_hash: sha256:be9131c6a3d3473d99b2c3d18098b95a0d3603547e12a88862f64287815a165b
source_transcript_hash: sha256:3e37f6733280849fb62d12ae3eadff992c912652b2adc44edb3fc54672782492
fill_id: 2b56b640-0fb6-487c-95de-c58a2574e8b8
published_at: '2026-09-30T05:17:16.915732'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Use Jeff from TypeSafe AI for instant, low-cost classification tasks like routing GitHub issues to coding agents.

## Prerequisites

### OpenRouter Account
- **Kind**: account
- **Note**: Required to access Jeff via API without waiting for TypeSafe's waitlist.

### GitHub Repository
- **Kind**: tool
- **Note**: A repo with issues to classify and route using the automated workflow.

### Claude Code Agent
- **Kind**: tool
- **Note**: Used in the tutorial to generate code, labels, and GitHub Actions for the setup.

## Steps

### Understand Jeff's Role
- **Timestamp**: [02:38](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=158)
- **Action**: Recognize Jeff as a 'System 1' model for instant, low-cost classification (choice, score, zero) rather than complex reasoning.

### Access Jeff via OpenRouter
- **Timestamp**: [08:02](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=482)
- **Action**: Bypass the TypeSafe waitlist by registering on OpenRouter to get API access to the latest Jeff model.

### Generate API Key
- **Timestamp**: [09:01](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=541)
- **Action**: Navigate to the TypeSafe AI dashboard, go to API keys, create a new key named 'tutorial', and save it securely.

### Clone Project Repository
- **Timestamp**: [10:01](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=601)
- **Action**: Use Claude Code to clone a test GitHub repository into the root folder for setting up the automation.
- **Command Or Clicks**: clone [GitHub URL]

### Create Repo and Labels
- **Timestamp**: [11:02](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=662)
- **Action**: Ask Claude Code to create a new private GitHub repository and add specific labels like 'error', 'documentation', and 'enhancement'.
- **Command Or Clicks**: create a new private GitHub repository for this project

### Install TypeSafe Skill
- **Timestamp**: [12:48](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=768)
- **Action**: Copy the URL for the official TypeSafe agent skill and install it in the project folder to teach the agent how to use Jeff's APIs.
- **Command Or Clicks**: install [TypeSafe Skill GitHub URL]

### Configure GitHub Action
- **Timestamp**: [13:36](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=816)
- **Action**: Instruct Claude Code to push changes that call Jeff via a GitHub Action on new issues, assigning labels and agents based on classification.

### Test the Workflow
- **Timestamp**: [14:30](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=870)
- **Action**: Create a new GitHub issue to verify that Jeff classifies the task, assigns an agent, and posts a comment with the confidence score.

## Gotchas

### Jeff cannot write complete sentences or reason; it is strictly for classification tasks like choice, score, or zero.
- **Severity**: serious
- **Timestamp**: [02:38](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=158)

### If the confidence score is below 0.75, you should add logic to pass the request to a human for review instead of auto-processing.
- **Severity**: serious
- **Timestamp**: [05:35](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=335)

### Jeff has a tiny context window of about 32,000 tokens, so it cannot handle complex or long-context tasks.
- **Severity**: blocking
- **Timestamp**: [02:38](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=158)

## Where to go next

Join Agentyc Labs for the coding masterclass and live sessions on building software factories with AI agents. Next Thursday features a deep dive into JFAI.

## Concepts surfaced

[[system-1-vs-system-2]] · [[github-actions-automation]] · [[cost-efficient-ai-routing]] · [[deterministic-output-structures]] · [[agent-swarm-workflows]]
