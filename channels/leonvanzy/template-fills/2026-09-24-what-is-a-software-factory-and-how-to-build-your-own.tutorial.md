---
video_id: AsvzMlLyQ38
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-09-24-what-is-a-software-factory-and-how-to-build-your-own.md
source_transcript: ../transcripts/2026-09-24-what-is-a-software-factory-and-how-to-build-your-own.md
source_summary_hash: sha256:7b8dfaffe62362ea50989890032188b69325e2f4dd88a2d2b27832560f2e6d0c
source_transcript_hash: sha256:c7dc9a28382beba51eabb35bbb45494d363fda768aebbbc7933b8905b5bd63c2
fill_id: b89efa9f-8a75-4ee6-8bae-bc060a65eafa
published_at: '2026-09-29T12:20:17.825213'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Build a GitHub-based software factory that orchestrates Claude and Codex agents via issues and Upstash sandboxes.

## Prerequisites

### GitHub Account
- **Kind**: account
- **Note**: Required for repository management, issue tracking, and GitHub Actions triggers.

### Upstash Account
- **Kind**: account
- **Note**: Provides the Box API key and VPS infrastructure for isolated agent sandboxes.

### Claude Code Subscription
- **Kind**: tool
- **Note**: Needed to generate the OAuth token for running agents under your subscription.

## Steps

### Install the factory skill via agent
- **Timestamp**: [09:13](https://www.youtube.com/watch?v=AsvzMlLyQ38&t=553)
- **Action**: Copy the GitHub repository link containing the software factory skill. In your coding agent, create a new folder and ask it to install the skill by pasting the URL.
- **Command Or Clicks**: Ask agent: "Please install the software factory skill." Paste URL.

### Activate the creation skill
- **Timestamp**: [10:51](https://www.youtube.com/watch?v=AsvzMlLyQ38&t=651)
- **Action**: Trigger the factory setup process using the specific slash command provided by the installed skill.
- **Command Or Clicks**: from draw slash "create up slash software factory"

### Configure repositories and agents
- **Timestamp**: [11:53](https://www.youtube.com/watch?v=AsvzMlLyQ38&t=713)
- **Action**: Select the GitHub repositories to bind, choose coding agents (Claude Code/Codex), name the new factory repo, set worker limits based on your Upstash plan, and configure task distribution logic.
- **Command Or Clicks**: Select repos -> Next. Choose Claude Code/Codex -> Next. Name repo 'Software Factory' -> Private. Set worker limit (e.g., 4) -> Next.

### Generate Upstash Box API Key
- **Timestamp**: [13:43](https://www.youtube.com/watch?v=AsvzMlLyQ38&t=823)
- **Action**: Create an API key in Upstash to allow the factory to interact with agent boxes. Paste this into the .env file.
- **Command Or Clicks**: Upstash -> Box Overview -> API Keys -> Create Key 'Software Factory'. Copy and paste into .env. Ctrl+S to save.

### Generate GitHub Fine-Grained Token
- **Timestamp**: [15:05](https://www.youtube.com/watch?v=AsvzMlLyQ38&t=905)
- **Action**: Create a fine-grained personal access token in GitHub settings. Grant read/write permissions for Content, Issues, and Pull Requests on specific repositories.
- **Command Or Clicks**: GitHub Profile -> Settings -> Developer Settings -> Personal Access Tokens -> Fine-grained tokens -> Generate Token. Set permissions: Content (RW), Issues (RW), Pull Requests (RW).

### Get Claude Code OAuth Token
- **Timestamp**: [16:03](https://www.youtube.com/watch?v=AsvzMlLyQ38&t=963)
- **Action**: Run the command in Claude Code to retrieve your OAuth token, which allows agents to run under your subscription.
- **Command Or Clicks**: In Claude Code, press the play button to insert the key. Paste into .env.

### Configure Agent Models and Test
- **Timestamp**: [17:00](https://www.youtube.com/watch?v=AsvzMlLyQ38&t=1020)
- **Action**: Select models (e.g., Opus for Claude, high effort for Codex). The agent will create smoke test boxes in Upstash to verify connectivity.
- **Command Or Clicks**: Select 'Opus with high effort' for Claude. Confirm smoke tests pass.

### Merge Factory Pull Requests
- **Timestamp**: [18:21](https://www.youtube.com/watch?v=AsvzMlLyQ38&t=1101)
- **Action**: Review and merge the pull requests created by the agent in both the project repositories and the software factory repo to enable bidirectional triggers.
- **Command Or Clicks**: Click 'Merge' on the pull requests in both repositories.

### Test the Factory Workflow
- **Timestamp**: [20:11](https://www.youtube.com/watch?v=AsvzMlLyQ38&t=1211)
- **Action**: Create a GitHub issue with a 'ready' label to trigger the factory. Monitor the actions tab and issue labels as the agent processes the task.
- **Command Or Clicks**: Create Issue -> Add 'ready' label. Check Actions tab. Change label to 'done' to trigger agent.

### Scale with Snapshots
- **Timestamp**: [22:31](https://www.youtube.com/watch?v=AsvzMlLyQ38&t=1351)
- **Action**: Create reusable snapshots in Upstash to pre-load skills and configurations for new agent boxes, ensuring consistent environments.
- **Command Or Clicks**: Ask agent: "Please create new snapshots for the Claude and Codex blocks that have the following skills preloaded."

## Gotchas

### Public repositories allow anyone to assign tasks and activate your factory. Keep it private or restrict triage logic.
- **Severity**: serious
- **Timestamp**: [06:04](https://www.youtube.com/watch?v=AsvzMlLyQ38&t=364)

### Agents may be blocked by permission systems during execution. You must manually click 'disable' in Cloud Code to allow command execution.
- **Severity**: blocking
- **Timestamp**: [21:40](https://www.youtube.com/watch?v=AsvzMlLyQ38&t=1300)

### Upstash does not allow agents to delete boxes or snapshots. You must perform deletions manually yourself.
- **Severity**: serious
- **Timestamp**: [23:53](https://www.youtube.com/watch?v=AsvzMlLyQ38&t=1433)

## Where to go next

Explore Agentic Labs for advanced coding agent courses and live sessions. Check Upstash documentation for deeper Box configuration details.

## Concepts surfaced

[[software-factory]] · [[github-actions]] · [[upstash-boxes]] · [[claude-code]] · [[codex-agent]] · [[agent-sandboxing]]
