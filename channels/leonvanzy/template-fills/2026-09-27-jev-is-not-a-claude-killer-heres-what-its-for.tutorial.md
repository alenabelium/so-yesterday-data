---
video_id: iyIAdmeKeMM
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-09-27-jev-is-not-a-claude-killer-heres-what-its-for.md
source_transcript: ../transcripts/2026-09-27-jev-is-not-a-claude-killer-heres-what-its-for.md
source_summary_hash: sha256:be9131c6a3d3473d99b2c3d18098b95a0d3603547e12a88862f64287815a165b
source_transcript_hash: sha256:3e37f6733280849fb62d12ae3eadff992c912652b2adc44edb3fc54672782492
fill_id: 9ed0fe2c-ff24-4537-9d0b-e8ae7dea2aec
published_at: '2026-09-29T22:11:28.856170'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Use Jeff from TypeSafe AI for cheap, instant classification tasks like routing GitHub issues to coding agents.

## Prerequisites

### OpenRouter Account
- **Kind**: account
- **Note**: Required to access Jeff without the TypeSafe waitlist.

### GitHub Repository
- **Kind**: tool
- **Note**: A repo with issues to classify and route via agents.

### Claude Code Agent
- **Kind**: tool
- **Note**: Used to clone the repo and generate workflow code.

## Steps

### Access Jeff via OpenRouter
- **Timestamp**: [08:02](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=482)
- **Action**: Bypass the TypeSafe waitlist by registering on OpenRouter to get API access to Jeff.
- **Command Or Clicks**: Register at OpenRouter and select Jeff as the model provider.
- **Choice Branch**: Use TypeSafe directly if you have an account; otherwise use OpenRouter.

### Generate API Key
- **Timestamp**: [09:01](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=541)
- **Action**: Create a new API key in the dashboard to authenticate requests.
- **Command Or Clicks**: Navigate to 'API keys' > 'Create new key' > Copy and save securely.
- **Choice Branch**: Ensure you have credits added; TypeSafe offers $5 free.

### Clone Project Repository
- **Timestamp**: [10:01](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=601)
- **Action**: Use the coding agent to clone the starter repository into your local environment.
- **Command Or Clicks**: In Claude Code: 'clone this repository into the root folder of the project' [paste GitHub URL]
- **Choice Branch**: You can use any existing repo or create a new test one.

### Define Agent Labels
- **Timestamp**: [11:20](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=680)
- **Action**: Instruct the agent to add specific labels for routing (e.g., Codex, Fable, Haiku).
- **Command Or Clicks**: In Claude Code: 'Please add these tags to the GitHub repository' [list agents]
- **Choice Branch**: Labels determine which specialized agent handles the task.

### Install TypeSafe Skill
- **Timestamp**: [12:48](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=768)
- **Action**: Add the official TypeSafe agent skill to teach your coding agent how to call Jeff.
- **Command Or Clicks**: Copy URL from community > In Claude Code: install skill in project folder
- **Choice Branch**: This skill provides the necessary API integration logic.

### Configure GitHub Action Logic
- **Timestamp**: [13:36](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=816)
- **Action**: Ask the agent to write code that triggers Jeff on new issues to classify and route.
- **Command Or Clicks**: In Claude Code: 'Every time we add a new task... Jive needs to be called via a GitHub Action' [paste prompt]
- **Choice Branch**: Prompt must include classification types, agent mapping, and confidence handling.

### Test Workflow with New Issue
- **Timestamp**: [14:30](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=870)
- **Action**: Create a new GitHub issue to verify Jeff classifies it correctly and adds comments.
- **Command Or Clicks**: Create GitHub Issue > Check for automated comment with classification and confidence score.
- **Choice Branch**: Review confidence scores; if <0.75, consider human review logic.

## Gotchas

### Jeff is a 'System 1' model: fast but cannot reason or write complete sentences. Do not use for complex tasks.
- **Severity**: serious
- **Timestamp**: [02:38](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=158)

### Context window is tiny (~32k tokens). Large inputs will fail or truncate.
- **Severity**: blocking
- **Timestamp**: [03:35](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=215)

### Confidence scores vary. If score < 0.75, the classification might be ambiguous and need human review.
- **Severity**: heads_up
- **Timestamp**: [05:35](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=335)

## Where to go next

Join Agentyc Labs for the 'Software Factory' masterclass to automate the full agent swarm workflow. Next video covers JFA I in depth.

## Concepts surfaced

[[system-1-vs-system-2]] · [[automated-issue-routing]] · [[cost-efficient-llm-classification]] · [[github-actions-workflow]] · [[agent-swarm]]
