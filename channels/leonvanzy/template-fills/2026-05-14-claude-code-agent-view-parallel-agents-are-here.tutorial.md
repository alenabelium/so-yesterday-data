---
video_id: tJVUAzLZUyI
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-05-14-claude-code-agent-view-parallel-agents-are-here.md
source_transcript: ../transcripts/2026-05-14-claude-code-agent-view-parallel-agents-are-here.md
source_summary_hash: sha256:20d8cef5efe65b14db441b10ab2d96c784454392f7d848ff676f1c7574da7759
source_transcript_hash: sha256:116ed9038bd42d5d6fa0373d989da9d1730b77e43c92acf9d9c6c14086511a83
fill_id: b7a257f8-eebd-4cf9-9c6d-142a28876286
published_at: '2026-05-19T08:13:42.968621'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Learn to dispatch and manage multiple parallel AI agent sessions in Claude Code using the new Agent View dispatcher.

## Prerequisites

### Claude Code
- **Kind**: tool
- **Note**: Must be updated to the latest version to access Agent Views.

### Terminal
- **Kind**: tool
- **Note**: Required to run claude agents and background commands.

## Steps

### Update Claude Code
- **Timestamp**: [01:15](https://www.youtube.com/watch?v=tJVUAzLZUyI&t=75)
- **Action**: Ensure you have the latest version of Claude Code installed to enable Agent Views.
- **Command Or Clicks**: Run the update command provided for your OS (Mac OS, Linux, or WSL).

### Open Dispatcher
- **Timestamp**: [02:00](https://www.youtube.com/watch?v=tJVUAzLZUyI&t=120)
- **Action**: Launch the Agent View dispatcher interface to manage parallel sessions.
- **Command Or Clicks**: claude agents

### Dispatch via Prompt
- **Timestamp**: [02:30](https://www.youtube.com/watch?v=tJVUAzLZUyI&t=150)
- **Action**: Create a new background agent session by giving an instruction in the dispatcher.
- **Command Or Clicks**: Type instruction (e.g., 'update the logo') and send.

### Dispatch via CLI Flag
- **Timestamp**: [03:15](https://www.youtube.com/watch?v=tJVUAzLZUyI&t=195)
- **Action**: Create a background session directly from a terminal window using the background flag.
- **Command Or Clicks**: claude -d -b 'update the readme file'

### Manage Permissions
- **Timestamp**: [04:30](https://www.youtube.com/watch?v=tJVUAzLZUyI&t=270)
- **Action**: Run a session with bypassed permissions or change mode interactively.
- **Command Or Clicks**: claude -p dangerous-is-key -b 'add legal pages' OR press Shift+Tab in session.

### Run Loop Command
- **Timestamp**: [06:00](https://www.youtube.com/watch?v=tJVUAzLZUyI&t=360)
- **Action**: Create a cron job that periodically identifies and commits improvements.
- **Command Or Clicks**: loop: 'every 10 minutes identify one meaningful improvement...'

### Stop Sessions
- **Timestamp**: [07:45](https://www.youtube.com/watch?v=tJVUAzLZUyI&t=465)
- **Action**: Stop all running background agents from the Agent View interface.
- **Command Or Clicks**: Hold Control and press X

### Resume Session
- **Timestamp**: [08:15](https://www.youtube.com/watch?v=tJVUAzLZUyI&t=495)
- **Action**: Resume a stopped session by instructing the agent to continue.
- **Command Or Clicks**: Open stopped session and say 'resume'

### Cross-Project View
- **Timestamp**: [08:45](https://www.youtube.com/watch?v=tJVUAzLZUyI&t=525)
- **Action**: View and jump between sessions across different projects from a single dispatcher.
- **Command Or Clicks**: Run claude agents from any directory.

### Parallel Work Trees
- **Timestamp**: [10:30](https://www.youtube.com/watch?v=tJVUAzLZUyI&t=630)
- **Action**: Scaffold multiple design variations using isolated work trees in parallel.
- **Command Or Clicks**: claude -d -b 'scaffold to-do app' then dispatch work tree prompts.

## Gotchas

### Killing the terminal window does not stop the background agent; it continues running.
- **Severity**: serious
- **Timestamp**: [07:30](https://www.youtube.com/watch?v=tJVUAzLZUyI&t=450)

### Sessions created without explicit permission flags will ask for permission for every change.
- **Severity**: heads_up
- **Timestamp**: [04:45](https://www.youtube.com/watch?v=tJVUAzLZUyI&t=285)

## Where to go next

Explore using different design skills or frameworks in parallel work trees to test UI variations efficiently.

## Concepts surfaced

[[claude-code-agent-view]] · [[parallel-ai-agents]] · [[background-tasks]] · [[work-trees]] · [[claude-loop-command]] · [[claude-goal-command]]
