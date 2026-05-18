---
video_id: BV9Bnj3l8pk
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-04-17-how-good-is-opus-47-really-new-claude-code-desktop-test.md
source_transcript: ../transcripts/2026-04-17-how-good-is-opus-47-really-new-claude-code-desktop-test.md
source_summary_hash: sha256:25ca9bc4009b02de4910ddb0cc1a645a96346348f6f1242be42a764a46c22885
source_transcript_hash: sha256:40f17524f981a312f08caf17c0c468ec0fc4ff169d3b81d4c89a29a8d4f52de9
fill_id: d6216d14-b0b3-4622-8c0d-eeee4a45e1e3
published_at: '2026-05-18T05:47:07.759466'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Opus 4.7 builds a fully functional infinite canvas app in one shot using Claude Code Desktop.

## Prerequisites

### Claude Code Desktop App
- **Kind**: tool
- **Note**: Updated version with new UI and workspace management features.

### Opus 4.7 Model
- **Kind**: tool
- **Note**: Anthropic's new flagship coding model required for this test.

### Bypass Permissions Mode
- **Kind**: knowledge
- **Note**: Enable in settings to let the agent run without asking for permission.

## Steps

### Update and Open Claude Code Desktop
- **Timestamp**: [00:00](https://www.youtube.com/watch?v=BV9Bnj3l8pk&t=0)
- **Action**: Update the Claude Code Desktop app to access the new UI and toggle to Claude Code mode.
- **Command Or Clicks**: Toggle between normal chat, co-work, and cla code modes in the left sidebar.

### Create Project Folder and Session
- **Timestamp**: [00:45](https://www.youtube.com/watch?v=BV9Bnj3l8pk&t=45)
- **Action**: Create a local folder named 'infinite draw' and select it as the project workspace for a new session.
- **Command Or Clicks**: Start a new session -> select project folder -> create 'infinite draw' folder.

### Configure Agent Mode
- **Timestamp**: [01:12](https://www.youtube.com/watch?v=BV9Bnj3l8pk&t=72)
- **Action**: Switch to bypass permissions mode to allow the agent to make changes without asking.
- **Command Or Clicks**: Settings -> enable allow bypass permissions mode -> select bypass permissions mode.

### Submit One-Shot Prompt
- **Timestamp**: [02:16](https://www.youtube.com/watch?v=BV9Bnj3l8pk&t=136)
- **Action**: Provide a detailed prompt requesting an infinite canvas app with shapes, text, icons, and export features.
- **Command Or Clicks**: Type prompt in chat -> select Opus 4.7 model -> set reasoning effort to extra high -> send.

### Review Architecture Plan
- **Timestamp**: [05:14](https://www.youtube.com/watch?v=BV9Bnj3l8pk&t=314)
- **Action**: Allow the agent to ask clarifying questions and generate an architecture plan using recommended stacks.
- **Command Or Clicks**: Click 'recommended' on tech stack questions -> open plan pane -> click 'revise plan' if needed.

### Monitor Agent Execution
- **Timestamp**: [07:31](https://www.youtube.com/watch?v=BV9Bnj3l8pk&t=451)
- **Action**: Watch the agent scaffold the Next.js app and install dependencies via the task pane.
- **Command Or Clicks**: Open tasks dropdown -> view task status -> open terminal if needed.

### Preview and Test Application
- **Timestamp**: [12:18](https://www.youtube.com/watch?v=BV9Bnj3l8pk&t=738)
- **Action**: Use the embedded preview pane to watch the live app build and test functionality like drawing and exporting.
- **Command Or Clicks**: Click preview -> click setup -> observe agent testing in embedded browser.

## Gotchas

### You must enable 'allow bypass permissions mode' in settings to let the agent run autonomously.
- **Severity**: blocking
- **Timestamp**: [01:12](https://www.youtube.com/watch?v=BV9Bnj3l8pk&t=72)

### The agent may ask clarifying questions; answering with 'recommended' speeds up the process.
- **Severity**: heads_up
- **Timestamp**: [05:14](https://www.youtube.com/watch?v=BV9Bnj3l8pk&t=314)

### Ensure you select 'extra high' reasoning effort for the best results with Opus 4.7.
- **Severity**: heads_up
- **Timestamp**: [04:00](https://www.youtube.com/watch?v=BV9Bnj3l8pk&t=240)

## Where to go next

Check out the next video in this series to see how Opus 4.7 handles complex debugging tasks in existing codebases.

## Concepts surfaced

[[claude-code-desktop]] · [[opus-4-7]] · [[agentic-coding]] · [[one-shot-prompting]] · [[infinite-canvas-app]]
