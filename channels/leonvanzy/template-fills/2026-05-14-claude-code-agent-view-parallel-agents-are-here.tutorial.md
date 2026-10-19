---
video_id: tJVUAzLZUyI
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-05-14-claude-code-agent-view-parallel-agents-are-here.md
source_transcript: ../transcripts/2026-05-14-claude-code-agent-view-parallel-agents-are-here.md
source_summary_hash: sha256:2c0f8bf4f74437fdfb60520afcbab24a50f37d5b9235a5438e495c71a9f8027e
source_transcript_hash: sha256:116ed9038bd42d5d6fa0373d989da9d1730b77e43c92acf9d9c6c14086511a83
fill_id: d953e9ff-221d-40b7-9c67-fbba353c8c92
published_at: '2026-10-19T21:39:33.104830'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Dispatch, monitor, and control multiple parallel Claude Code agents from one dispatcher, including background tasks, skills, and work-tree experiments.

## Prerequisites

### Claude Code installed
- **Kind**: tool
- **Note**: Update to the latest version via the provided command for your OS.

### Operating system
- **Kind**: os
- **Note**: Works on macOS, Linux, or Windows with WSL.

## Steps

### Update Claude Code to the latest version
- **Timestamp**: [01:30](https://www.youtube.com/watch?v=tJVUAzLZUyI&t=90)
- **Action**: Run the update command for your operating system to ensure Agent View is available.
- **Command Or Clicks**: For macOS/Linux/WSL: <update command>; For Windows: <update command>

### Launch the dispatcher with claude agents
- **Timestamp**: [02:00](https://www.youtube.com/watch?v=tJVUAzLZUyI&t=120)
- **Action**: Instead of the usual claude command, run 'claude agents' to open the dispatcher window where you can create and manage background agents.
- **Command Or Clicks**: claude agents

### Dispatch a background agent from the dispatcher
- **Timestamp**: [02:30](https://www.youtube.com/watch?v=tJVUAzLZUyI&t=150)
- **Action**: Give the dispatcher any instruction; it will create a new Claude Code session in the background to perform the task. Use the mouse to click on a session to view it, and the back arrow to return to the dispatcher.
- **Command Or Clicks**: Type instruction in dispatcher; click session; press back arrow

### Create a background session from a terminal
- **Timestamp**: [03:20](https://www.youtube.com/watch?v=tJVUAzLZUyI&t=200)
- **Action**: Open a new terminal window and run 'claude -d' with a prompt. This creates a background session without occupying the terminal; you can close the terminal and view the session in the dispatcher.
- **Command Or Clicks**: claude -d "update the readme file"

### Run a background session in bypass permissions mode
- **Timestamp**: [04:30](https://www.youtube.com/watch?v=tJVUAzLZUyI&t=270)
- **Action**: Set permissions mode to bypass permissions and use the background flag to start a session that won't ask for permission.
- **Command Or Clicks**: claude --dangerously-skip-permissions -d "add the legal and privacy pages"

### Change permissions mode with Shift+Tab
- **Timestamp**: [05:40](https://www.youtube.com/watch?v=tJVUAzLZUyI&t=340)
- **Action**: In any session, press Shift+Tab to cycle through permission modes, e.g., switch to 'accept all edits' to avoid constant prompts.
- **Command Or Clicks**: Shift+Tab

### Run a skill in agent view
- **Timestamp**: [06:00](https://www.youtube.com/watch?v=tJVUAzLZUyI&t=360)
- **Action**: Use the dispatcher to run a specific skill, like a security scanner, in a background agent. Set the mode to auto-accept edits to avoid permission prompts.
- **Command Or Clicks**: Run skill 'security scanner' in dispatcher

### Set up a loop command for continuous improvement
- **Timestamp**: [06:41](https://www.youtube.com/watch?v=tJVUAzLZUyI&t=401)
- **Action**: Use the loop command to create a cron job that runs every 10 minutes, identifies a meaningful improvement, makes the change, and commits it.
- **Command Or Clicks**: loop "every 10 minutes, identify one meaningful improvement, make it, and create a commit"

### Use the goal command for long-running tasks
- **Timestamp**: [07:20](https://www.youtube.com/watch?v=tJVUAzLZUyI&t=440)
- **Action**: The goal command keeps running until a complex task is completed, even if it takes hours or days. Provide a detailed task description.
- **Command Or Clicks**: goal "add a built-in issue tracking feature..."

### Stop and resume sessions
- **Timestamp**: [08:05](https://www.youtube.com/watch?v=tJVUAzLZUyI&t=485)
- **Action**: To stop all running sessions, go to the agent view and press Ctrl+X. Sessions move to the completed tab with status 'stopped'. To resume, open a stopped session and tell the agent to resume.
- **Command Or Clicks**: Ctrl+X

### View sessions across projects
- **Timestamp**: [09:06](https://www.youtube.com/watch?v=tJVUAzLZUyI&t=546)
- **Action**: Agent view shows sessions from all your projects in one place. You can run 'claude agents' from anywhere on your machine and jump between sessions across workspaces.
- **Command Or Clicks**: claude agents (from any directory)

### Use agent view with work trees for parallel design experiments
- **Timestamp**: [10:30](https://www.youtube.com/watch?v=tJVUAzLZUyI&t=630)
- **Action**: Scaffold a base app, then dispatch multiple background agents, each instructed to create an isolated work tree with a different design variation. Add a command to run the dev server on a unique port for each.
- **Command Or Clicks**: claude --dangerously-skip-permissions -d "please scaffold a simple to-do app..." then dispatch three agents with work tree prompts

## Gotchas

### Sessions continue running in the background even if you close the terminal window; you must stop them explicitly with Ctrl+X in agent view.
- **Severity**: serious
- **Timestamp**: [08:05](https://www.youtube.com/watch?v=tJVUAzLZUyI&t=485)

### If you don't set a permissions mode, sessions will keep asking for permission; use Shift+Tab to switch to auto-accept edits.
- **Severity**: heads_up
- **Timestamp**: [05:40](https://www.youtube.com/watch?v=tJVUAzLZUyI&t=340)

## Where to go next

Now that you can manage parallel agents, explore combining agent views with work trees for rapid design iteration. Check out the coding masterclass for deeper workflows.

## Concepts surfaced

[[parallel-agents]] · [[background-agents]] · [[work-trees]] · [[loop-command]] · [[goal-command]] · [[permissions-modes]]
