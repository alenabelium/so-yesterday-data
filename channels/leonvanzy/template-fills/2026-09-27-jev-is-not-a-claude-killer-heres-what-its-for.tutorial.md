---
video_id: iyIAdmeKeMM
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-09-27-jev-is-not-a-claude-killer-heres-what-its-for.md
source_transcript: ../transcripts/2026-09-27-jev-is-not-a-claude-killer-heres-what-its-for.md
source_summary_hash: sha256:be9131c6a3d3473d99b2c3d18098b95a0d3603547e12a88862f64287815a165b
source_transcript_hash: sha256:3e37f6733280849fb62d12ae3eadff992c912652b2adc44edb3fc54672782492
fill_id: 0bdb3e5c-ee92-4a1b-9250-6a172156f6f0
published_at: '2026-09-30T06:17:35.046445'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Use TypeSafe AI's Jeff model for instant, low-cost classification and routing tasks instead of expensive reasoning models.

## Prerequisites

### TypeSafe AI Account
- **Kind**: account
- **Note**: Sign up for an account to access the Jeff API and playground.

### OpenRouter Account
- **Kind**: account
- **Note**: Alternative access method if TypeSafe waitlist is active; provides API key.

### GitHub Repository
- **Kind**: tool
- **Note**: A repository to connect the workflow and test issue classification.

### Claude Code Agent
- **Kind**: tool
- **Note**: Used in the demo to clone repos, create issues, and push GitHub Actions.

## Steps

### Understand Jeff's Use Case
- **Timestamp**: [02:38](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=158)
- **Action**: Recognize that Jeff is a 'System 1' model designed for instant, low-cost classification (choice, score, or zero) rather than complex reasoning.

### Access the API
- **Timestamp**: [08:02](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=482)
- **Action**: Sign up for TypeSafe AI or OpenRouter to get an API key. Create a new API key in the dashboard and save it securely.

### Clone Demo Repository
- **Timestamp**: [10:01](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=601)
- **Action**: Open your coding agent (e.g., Claude Code) and clone the provided GitHub repository to start the setup.
- **Command Or Clicks**: git clone <repository-url>

### Create GitHub Repo & Labels
- **Timestamp**: [11:02](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=662)
- **Action**: Instruct the agent to create a new private GitHub repository and add specific labels (e.g., bug, documentation, enhancement) and agent tags.
- **Command Or Clicks**: Create a new private GitHub repository... Please add these tags...

### Install Agent Skill
- **Timestamp**: [12:48](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=768)
- **Action**: Copy the URL for the TypeSafe agent skill from the community and install it in your project folder to teach the agent how to use Jeff.
- **Command Or Clicks**: Install the Type Safe agent skill...

### Configure GitHub Action
- **Timestamp**: [13:36](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=816)
- **Action**: Ask the coding agent to create a GitHub Action that calls Jeff via API on new issues, classifies them, assigns agents, and adds comments with confidence scores.
- **Command Or Clicks**: Every time we add a new task... Jive needs to be called via a GitHub Action...

### Test the Workflow
- **Timestamp**: [14:30](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=870)
- **Action**: Create a new issue in the repository. Observe Jeff's response, which should include the category, assigned agent, and confidence scores.
- **Command Or Clicks**: add a new emotion— frightened... Let's create this .

## Gotchas

### Jeff cannot reason or write complete sentences; it is strictly for classification tasks like choice, score, or zero.
- **Severity**: blocking
- **Timestamp**: [02:38](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=158)

### If confidence scores are below 0.75, you should add logic to pass the task to a human for review rather than auto-routing.
- **Severity**: serious
- **Timestamp**: [05:35](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=335)

### TypeSafe may have a waitlist; use OpenRouter as an alternative if you cannot access the TypeSafe API immediately.
- **Severity**: heads_up
- **Timestamp**: [08:02](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=482)

## Where to go next

Join Agentyc Labs for the coding masterclass and live sessions on building software factories with AI agents. See description for links.

## Concepts surfaced

[[system-1-vs-system-2]] · [[ai-classification]] · [[github-actions]] · [[software-factory]] · [[cost-optimization]]
