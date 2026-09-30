---
video_id: iyIAdmeKeMM
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-09-27-jev-is-not-a-claude-killer-heres-what-its-for.md
source_transcript: ../transcripts/2026-09-27-jev-is-not-a-claude-killer-heres-what-its-for.md
source_summary_hash: sha256:be9131c6a3d3473d99b2c3d18098b95a0d3603547e12a88862f64287815a165b
source_transcript_hash: sha256:3e37f6733280849fb62d12ae3eadff992c912652b2adc44edb3fc54672782492
fill_id: ec04a858-a55a-4854-8640-bddac8dada65
published_at: '2026-09-30T04:16:59.590373'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Use Jeff for instant, low-cost classification tasks like GitHub issue routing instead of expensive reasoning models.

## Prerequisites

### OpenRouter Account
- **Kind**: account
- **Note**: Required to access Jeff without waiting in line on the TypeSafe waitlist.

### GitHub Repository
- **Kind**: tool
- **Note**: A repo to connect to the workflow for automated issue classification and agent routing.

### Claude Code Agent
- **Kind**: tool
- **Note**: Used in the demo to clone repos, create issues, and push GitHub Actions workflows.

## Steps

### Access Jeff via OpenRouter
- **Timestamp**: [08:02](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=482)
- **Action**: Bypass the TypeSafe waitlist by registering on OpenRouter, which provides access to the latest version of Jeff.
- **Command Or Clicks**: Register account at OpenRouter. Use 'Jeff' in API calls instead of 'TypeSafe API'.
- **Choice Branch**: Use TypeSafe dashboard directly if you have access, or use OpenRouter as an alternative.

### Generate API Key
- **Timestamp**: [09:01](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=541)
- **Action**: Navigate to the API keys section in the TypeSafe dashboard and create a new key named 'tutorial'.
- **Command Or Clicks**: Go to API keys -> Create new key -> Name it 'tutorial' -> Copy and save securely.
- **Choice Branch**: Ensure you have credits added; new accounts often receive $5 free credits.

### Clone Repository
- **Timestamp**: [10:01](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=601)
- **Action**: Use an agent to clone a test GitHub repository into your local project root.
- **Command Or Clicks**: Copy the command from the code section. Open Claude Code -> Paste GitHub URL -> Clone to root folder.
- **Choice Branch**: You can use any existing repo or create a new test repository.

### Define Agent Labels
- **Timestamp**: [11:20](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=680)
- **Action**: Create specific GitHub labels for routing tasks to different AI agents based on complexity.
- **Command Or Clicks**: Ask agent: 'Please add these tags to the GitHub repository.' -> Add labels: Claude Fable, Codex Astra, Claude Haiku.
- **Choice Branch**: Labels help route bugs to Fable, spatial tasks to Astra, and docs to Haiku.

### Install TypeSafe Skill
- **Timestamp**: [12:48](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=768)
- **Action**: Install the official TypeSafe agent skill to teach your coding agent how to use Jeff's API.
- **Command Or Clicks**: Copy GitHub URL for the skill. Return to agent -> Install skill in project folder.
- **Choice Branch**: This skill provides the necessary instructions for the agent to interact with Jeff.

### Configure GitHub Action
- **Timestamp**: [13:36](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=816)
- **Action**: Instruct the agent to create a GitHub Action that calls Jeff on every new issue.
- **Command Or Clicks**: Ask Claude: 'Push changes to GitHub.' -> Agent creates workflow to classify issue and assign agent label.
- **Choice Branch**: The workflow must include confidence scores and input/response comments.

### Test the Workflow
- **Timestamp**: [14:30](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=870)
- **Action**: Create a new GitHub issue to verify that Jeff classifies it correctly and assigns an agent.
- **Command Or Clicks**: Create new issue -> Write description (e.g., 'add a new emotion'). -> Check comments for classification result.
- **Choice Branch**: Verify the confidence score; if low, consider human review or re-prompting.

## Gotchas

### Jeff is not a general-purpose LLM. It cannot write complete sentences or reason like Claude.
- **Severity**: serious
- **Timestamp**: [00:00](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=0)

### Jeff has a tiny context window of about 32,000 tokens and is bad at science/math.
- **Severity**: serious
- **Timestamp**: [02:38](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=158)

### If confidence score is below 0.75, the system should pass the task to a human for review.
- **Severity**: blocking
- **Timestamp**: [05:35](https://www.youtube.com/watch?v=iyIAdmeKeMM&t=335)

## Where to go next

Join Agentyc Labs for the coding masterclass and live sessions on building software factories with AI agents. Next Thursday features a deep dive into JFA I.

## Concepts surfaced

[[system-1-vs-system-2]] · [[github-actions-workflow]] · [[ai-agent-routing]] · [[cost-optimization-in-ai]]
