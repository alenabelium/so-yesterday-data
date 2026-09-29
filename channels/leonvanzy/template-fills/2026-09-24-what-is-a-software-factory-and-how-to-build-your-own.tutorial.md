---
video_id: AsvzMlLyQ38
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-09-24-what-is-a-software-factory-and-how-to-build-your-own.md
source_transcript: ../transcripts/2026-09-24-what-is-a-software-factory-and-how-to-build-your-own.md
source_summary_hash: sha256:7b8dfaffe62362ea50989890032188b69325e2f4dd88a2d2b27832560f2e6d0c
source_transcript_hash: sha256:c7dc9a28382beba51eabb35bbb45494d363fda768aebbbc7933b8905b5bd63c2
fill_id: 0fe8ae89-e732-4ac0-a22b-b1a7153079fe
published_at: '2026-09-29T11:25:11.513340'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Build a swarm of coding agents using GitHub issues as triggers, Upstash boxes for isolated sandboxes, and reusable snapshots for scalable agent deployment.

## Prerequisites

### GitHub Account
- **Kind**: account
- **Note**: Required to manage repositories, issues, and personal access tokens for the factory workflow.

### Upstash Account
- **Kind**: account
- **Note**: Provides the 'Box' infrastructure (Linux VMs) where coding agents run in isolated sandboxes.

### Claude Code or Codex
- **Kind**: tool
- **Note**: The specific coding agents that will process tasks and generate pull requests within the factory.

## Steps

### Install the Factory Skill
- **Timestamp**: [09:13](https://www.youtube.com/watch?v=AsvzMlLyQ38&t=553)
- **Action**: Copy the GitHub repository link containing the software factory skill, create a new folder in your coding agent, and instruct the agent to install the skill using the provided URL.
- **Command Or Clicks**: Paste URL into agent chat and say: "Please install the software factory skill."

### Activate the Factory Creation
- **Timestamp**: [10:51](https://www.youtube.com/watch?v=AsvzMlLyQ38&t=651)
- **Action**: Trigger the factory creation process by invoking the specific slash command in your coding agent interface.
- **Command Or Clicks**: Type: /create/up/software-factory

### Configure Repositories and Agents
- **Timestamp**: [11:53](https://www.youtube.com/watch?v=AsvzMlLyQ38&t=713)
- **Action**: Select the GitHub repositories to bind to the factory, choose which coding agents (e.g., Claude Code, Codex) will act as workers, and set the worker limit based on your Upstash plan.
- **Command Or Clicks**: Select repos in UI; specify agent types and box count (e.g., 4 boxes).

### Generate API Keys and Secrets
- **Timestamp**: [13:43](https://www.youtube.com/watch?v=AsvzMlLyQ38&t=823)
- **Action**: Create an Upstash Box API key and a GitHub Fine-Grained Personal Access Token with read/write permissions for issues, pull requests, and contents. Paste these into the .env file.
- **Command Or Clicks**: Upstash: Create API Key; GitHub: Settings > Developer settings > Personal access tokens > Generate token.

### Merge Pull Requests to Enable Triggers
- **Timestamp**: [18:21](https://www.youtube.com/watch?v=AsvzMlLyQ38&t=1101)
- **Action**: Accept the pull requests created by the agent in your project repositories. This step allows the projects to send signals (issues) to the software factory.
- **Command Or Clicks**: Click 'Merge pull request' on the generated PRs in GitHub.

### Test the Factory Workflow
- **Timestamp**: [20:11](https://www.youtube.com/watch?v=AsvzMlLyQ38&t=1211)
- **Action**: Create a new GitHub issue with a 'ready' label to trigger the factory. The system will assign an agent, who will work in a sandbox and create a pull request upon completion.
- **Command Or Clicks**: Create Issue > Add label 'ready' > Observe Actions tab for execution.

### Scale with Reusable Snapshots
- **Timestamp**: [22:31](https://www.youtube.com/watch?v=AsvzMlLyQ38&t=1351)
- **Action**: Create snapshots in Upstash to define a standard environment (skills, configs) for agents. Use these snapshots when creating new boxes to ensure consistent agent behavior without manual setup.
- **Command Or Clicks**: Ask agent: "Please create new snapshots for the Claude and Codex blocks that have the following skills preloaded."

## Gotchas

### Public repositories allow anyone to assign tasks and activate your factory. Keep the factory repo private and restrict issue assignment if needed.
- **Severity**: serious
- **Timestamp**: [06:04](https://www.youtube.com/watch?v=AsvzMlLyQ38&t=364)

### Agents run in isolated sandboxes (VPS) to prevent access to your local secrets or files. Do not expect them to interact with your local machine directly.
- **Severity**: serious
- **Timestamp**: [05:06](https://www.youtube.com/watch?v=AsvzMlLyQ38&t=306)

### Upstash does not allow agents to delete boxes or snapshots. You must manually delete old resources to avoid clutter or billing issues.
- **Severity**: blocking
- **Timestamp**: [23:53](https://www.youtube.com/watch?v=AsvzMlLyQ38&t=1433)

## Where to go next

Explore Agentic Labs for advanced coding agent courses and live sessions. Check Upstash documentation for deeper insights into Box configurations and snapshot management.

## Concepts surfaced

[[software-factory]] · [[coding-agents]] · [[github-actions]] · [[upstash-boxes]] · [[agent-sandboxes]] · [[reusable-snapshots]]
