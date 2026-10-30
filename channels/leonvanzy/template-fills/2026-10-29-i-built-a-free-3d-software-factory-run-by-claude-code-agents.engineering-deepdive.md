---
video_id: NAQyKMdxRT4
template_id: engineering-deepdive
template_version: 1
source_summary: ../summaries/2026-10-29-i-built-a-free-3d-software-factory-run-by-claude-code-agents.md
source_transcript: ../transcripts/2026-10-29-i-built-a-free-3d-software-factory-run-by-claude-code-agents.md
source_summary_hash: sha256:5607adf17a4a7627158605428a2928a4e8cbb5acf2a6dbc4ad857cd5c62c60b1
source_transcript_hash: sha256:745409d933c01663e979d37c43f9329327d6bd2c1b401ebd0911ccc3503abca6
fill_id: 35017bfa-9c34-4992-a09c-db028dc51255
published_at: '2026-10-30T20:51:41.036709'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

Cube Forge is an open-source 3D software factory where Claude Code and Codex agents autonomously manage GitHub issues and pull requests. The defining architectural choice is running each agent in an isolated Upstash Box VM, enabling cloud execution, resource isolation, and continuous operation even when the user's PC is off.

## Components

### 3D World / Office
- **Role**: Interactive 3D environment representing projects as floors. Agents walk, play games, make coffee, and interact with objects. Provides visual status and gamified engagement.
- **Timestamp**: [00:00](https://www.youtube.com/watch?v=NAQyKMdxRT4&t=0)

### Kanban Board
- **Role**: Task management interface where users create tasks with descriptions. Tasks are automatically assigned to agents, who work on them and create pull requests.
- **Timestamp**: [00:54](https://www.youtube.com/watch?v=NAQyKMdxRT4&t=54)

### CEO Agent (Luna)
- **Role**: Autonomous agent that monitors project workload, hires/fires agents based on demand, and communicates via chat and voice. Can walk between floors and manage tasks.
- **Timestamp**: [03:07](https://www.youtube.com/watch?v=NAQyKMdxRT4&t=187)

### Manager Console
- **Role**: Central dashboard for adding projects (local folder, GitHub repo, or new), viewing management info, customizing CEO model, and managing team agents.
- **Timestamp**: [05:59](https://www.youtube.com/watch?v=NAQyKMdxRT4&t=359)

### Upstash Boxes Integration
- **Role**: Cloud VM service where each agent runs in an isolated box with ~2 CPU cores, 4GB RAM, and a built-in browser. Enables cloud execution and resource isolation.
- **Timestamp**: [10:10](https://www.youtube.com/watch?v=NAQyKMdxRT4&t=610)

### Agent Authentication
- **Role**: Process to authenticate agents in boxes using Claude Code subscription or API keys. Provides a URL for authorization, then copies credentials into the box.
- **Timestamp**: [12:15](https://www.youtube.com/watch?v=NAQyKMdxRT4&t=735)

## Trade-offs

- Running agents on local hardware is resource-intensive and they compete for resources.
- Local agents share the same codebase, risking interference.
- Cloud boxes isolate agents, limiting damage from prompt injection.
- Free Upstash plan limits to 10 boxes, capping concurrent agents.
- Cloud execution requires trusting third-party infrastructure with code and credentials.

## Concepts surfaced

[[ai-agents]] · [[agent-orchestration]] · [[cloud-execution]] · [[github-issues]] · [[pull-requests]] · [[gamification]]
