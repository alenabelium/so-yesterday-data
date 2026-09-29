---
video_id: AsvzMlLyQ38
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-09-24-what-is-a-software-factory-and-how-to-build-your-own.md
source_transcript: ../transcripts/2026-09-24-what-is-a-software-factory-and-how-to-build-your-own.md
source_summary_hash: sha256:7b8dfaffe62362ea50989890032188b69325e2f4dd88a2d2b27832560f2e6d0c
source_transcript_hash: sha256:c7dc9a28382beba51eabb35bbb45494d363fda768aebbbc7933b8905b5bd63c2
fill_id: 69f206cc-29d6-4ea1-b9e0-dd0c0a1f21a8
published_at: '2026-09-29T13:19:27.518925'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Build a swarm of coding agents using GitHub issues and Upstash sandboxes.

## Prerequisites

### GitHub Account
- **Kind**: account
- **Note**: Required for managing repositories, issues, and personal access tokens.

### Upstash Account
- **Kind**: account
- **Note**: Provides the free tier for running isolated Linux boxes (VPS) for agents.

### Coding Agent
- **Kind**: tool
- **Note**: Claude Code or similar tool to generate and configure the factory skill.

## Steps

### Install the Software Factory Skill
- **Timestamp**: [09:13](https://www.youtube.com/watch?v=AsvzMlLyQ38&t=553)
- **Action**: Copy the GitHub repository link containing the software factory skill and ask your coding agent to install it.
- **Command Or Clicks**: Ask agent: "Please install the software factory skill." Paste URL. Activate with slash command: /create/up/software-factory
- **Choice Branch**: Allow the agent to use '7th context' for documentation if prompted.

### Configure Factory Parameters
- **Timestamp**: [10:51](https://www.youtube.com/watch?v=AsvzMlLyQ38&t=651)
- **Action**: Answer the agent's prompts to select repositories, agents (Claude/Codex), and worker limits.
- **Command Or Clicks**: Select repos. Set agent type (e.g., Claude Code). Set worker limit (e.g., 4 boxes). Enable agent browser.
- **Choice Branch**: Choose between even distribution or priority for specific agents if no label is present.

### Generate and Add Secrets
- **Timestamp**: [13:43](https://www.youtube.com/watch?v=AsvzMlLyQ38&t=823)
- **Action**: Create API keys for Upstash and GitHub, then add them to the .env file.
- **Command Or Clicks**: Upstash: Create Box API Key. GitHub: Generate Fine-grained PAT with repo/issue/pr permissions. Cloud Code: Run play button for OAuth token. Paste all into .env.
- **Choice Branch**: Keep tokens secret; do not share them publicly.

### Merge Repository Triggers
- **Timestamp**: [18:21](https://www.youtube.com/watch?v=AsvzMlLyQ38&t=1101)
- **Action**: Merge the pull requests created by the agent to allow project repositories to signal the factory.
- **Command Or Clicks**: Open PRs in target repos. Click 'Merge pull request' on each.
- **Choice Branch**: Ensure all connected repos have their respective PRs merged.

### Test the Factory Workflow
- **Timestamp**: [19:28](https://www.youtube.com/watch?v=AsvzMlLyQ38&t=1168)
- **Action**: Create a GitHub issue with specific labels to trigger the agent swarm.
- **Command Or Clicks**: Create Issue. Add label 'ready'. Assign tag for specific agent (e.g., Codex). Change label to 'done' to start processing.
- **Choice Branch**: Monitor labels changing from 'done' to 'running in the factory' to 'factory review'.

### Scale with Snapshots
- **Timestamp**: [22:31](https://www.youtube.com/watch?v=AsvzMlLyQ38&t=1351)
- **Action**: Create reusable snapshots for agent environments to ensure consistent skills and safeguards.
- **Command Or Clicks**: Ask agent: "Please create new snapshots for the Claude and Codex blocks that have the following skills preloaded." Update Upstash boxes.
- **Choice Branch**: Upstash prevents agents from deleting snapshots; manual deletion is required.

## Gotchas

### Public repositories allow anyone to trigger your factory. Keep it private or restrict issue assignment.
- **Severity**: serious
- **Timestamp**: [06:04](https://www.youtube.com/watch?v=AsvzMlLyQ38&t=364)

### Agents may be blocked by permission systems; click 'disable' in Cloud Code to allow command execution.
- **Severity**: blocking
- **Timestamp**: [21:40](https://www.youtube.com/watch?v=AsvzMlLyQ38&t=1300)

### Upstash does not allow agents to delete boxes or snapshots. You must manage deletion manually.
- **Severity**: heads_up
- **Timestamp**: [23:53](https://www.youtube.com/watch?v=AsvzMlLyQ38&t=1433)

## Where to go next

Explore Agentic Labs for advanced coding agent courses and live sessions. Check Upstash docs for deeper sandbox configuration.

## Concepts surfaced

[[software-factory]] · [[agent-swarm]] · [[upstash-boxes]] · [[github-actions]] · [[sandbox-isolation]] · [[automated-triage]]
