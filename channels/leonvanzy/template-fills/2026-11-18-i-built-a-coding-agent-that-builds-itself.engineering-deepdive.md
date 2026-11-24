---
video_id: etrC9bplAbA
template_id: engineering-deepdive
template_version: 1
source_summary: ../summaries/2026-11-18-i-built-a-coding-agent-that-builds-itself.md
source_transcript: ../transcripts/2026-11-18-i-built-a-coding-agent-that-builds-itself.md
source_summary_hash: sha256:349dc9f85893664763b156e9beaffdfdc67d69c55e86f6fa377e894a890d703e
source_transcript_hash: sha256:d63ceb3b61545cb6df5059659a398d00466f8d7d9eb93abc611d040b0d8656cd
fill_id: 23e43bfd-8c5e-42f8-b118-d0922b7d7e76
published_at: '2026-11-24T07:17:41.122643'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

Code Den is an open-source, MIT-licensed tool that implements four levels of AI coding systems, from individual agent sessions to a fully autonomous 'dark factory' that detects issues, assigns tasks to a swarm of agents, and merges changes without human intervention. The non-obvious choice: the orchestrator and project managers handle multi-project management, while the dark factory uses a scout agent to identify improvements and automatically implement them after passing tests, verification, and security audits.

## Components

### Orchestrator Agent
- **Role**: Sees all projects and all sessions running in them. Provides reports on all agents' work and can launch new sessions on request. Acts as the central command for multi-project management.
- **Timestamp**: [01:26](https://www.youtube.com/watch?v=etrC9bplAbA&t=86)

### Project Manager
- **Role**: Per-project agent that sees all sessions running in that project. Provides updates, can create sessions on behalf of the user, and asks clarifying questions. Sends notifications to the inbox when changes are ready to merge.
- **Timestamp**: [10:43](https://www.youtube.com/watch?v=etrC9bplAbA&t=643)

### Software Factory
- **Role**: Level 3 mode that processes GitHub issues as tasks. Classifies tasks (bug, feature, documentation) and assigns them to a swarm of worker agents. Follows workflows: low-risk changes create PRs directly; new features require verification by another agent; bug fixes must be reproduced and proven fixed.
- **Timestamp**: [17:53](https://www.youtube.com/watch?v=etrC9bplAbA&t=1073)

### Dark Factory
- **Role**: Level 4 mode with no human intervention. A scout agent analyzes the codebase to identify problems, gaps, and feature opportunities, then automatically creates tasks. The factory runs the same loop as the software factory but merges changes automatically after checks.
- **Timestamp**: [23:07](https://www.youtube.com/watch?v=etrC9bplAbA&t=1387)

### Automation
- **Role**: Scheduled or event-triggered agent runs, e.g., security scans every hour. Can send requests to new agent sessions or to the project manager. Supports templates, custom prompts, and variable placeholders.
- **Timestamp**: [07:38](https://www.youtube.com/watch?v=etrC9bplAbA&t=458)

### Scout Agent
- **Role**: In dark factory mode, analyzes code to find issues and opportunities. For larger projects, creates subagents to analyze code from different perspectives. Automatically creates tasks for the factory.
- **Timestamp**: [23:07](https://www.youtube.com/watch?v=etrC9bplAbA&t=1387)

## Trade-offs

- Automation can run on a schedule or event, but requires careful configuration to avoid redundant sessions.
- Dark factory merges automatically, but only after passing tests, verification, and security audits.
- Software factory requires GitHub and a vision file, adding setup overhead but enabling autonomous workflows.
- Scaling agents increases resource consumption on your machine.
- Trusted authors setting prevents junk tasks in public repos but limits contributions.
- Daily budget and merge limits act as safety valves but may halt progress if misconfigured.

## Concepts surfaced

[[ai-agents]] · [[orchestrator]] · [[software-factory]] · [[dark-factory]] · [[automation]] · [[github-issues]]
