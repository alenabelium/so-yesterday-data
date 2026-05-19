---
video_id: -W8uYEX4gLQ
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-04-22-claude-design-claude-code-no-designer-needed.md
source_transcript: ../transcripts/2026-04-22-claude-design-claude-code-no-designer-needed.md
source_summary_hash: sha256:0a27810ad1ff7e85d6a292f9f0355687c8c2bfc918e5f0a9b40f220d5d63f954
source_transcript_hash: sha256:b1dc0041292c4ec7d7c5038f404ddda4b5015beba7360366c0ab59bd9cd11274
fill_id: 00c8c16e-e67c-41e8-b4bc-958e30e70081
published_at: '2026-05-19T04:44:33.798629'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Redesign a functional app from wireframe to production-ready UI using only Claude Design and Claude Code.

## Prerequisites

### Claude Design Account
- **Kind**: account
- **Note**: Access to Claude Design for creating wireframes and high-fidelity interactive prototypes.

### Claude Code Terminal
- **Kind**: tool
- **Note**: Installed Claude Code CLI to receive design handoff and implement UI changes.

### Existing Project Codebase
- **Kind**: tool
- **Note**: A functional but visually plain application (e.g., Local Forge) to serve as the base for redesign.

## Steps

### Create project and select skills
- **Timestamp**: [02:30](https://www.youtube.com/watch?v=-W8uYEX4gLQ&t=150)
- **Action**: Name the project in Claude Design, select 'wireframe', and add the 'front-end design' and 'interactive prototype' skills.
- **Command Or Clicks**: Select 'wireframe' -> click 'create' -> add 'front-end design' skill -> add 'interactive prototype' skill
- **Choice Branch**: You can also upload existing codebases or Figma files, or start with a sketch.

### Dictate design requirements
- **Timestamp**: [03:26](https://www.youtube.com/watch?v=-W8uYEX4gLQ&t=206)
- **Action**: Use voice dictation to describe the UI layout, including sidebar workspaces, kanban board columns, and agent status indicators.
- **Command Or Clicks**: Press voice dictation button -> dictate requirements -> send
- **Choice Branch**: Specify fidelity (sketchy/lowfi), layout variations, and target platform during the Q&A phase.

### Review and select wireframe version
- **Timestamp**: [06:41](https://www.youtube.com/watch?v=-W8uYEX4gLQ&t=401)
- **Action**: Navigate the generated wireframes, zoom in/out, and select a preferred layout direction (e.g., Version 2).
- **Command Or Clicks**: Click/drag to navigate -> hold control + mouse wheel to zoom -> select 'version two'
- **Choice Branch**: You can tweak accent colors or request specific edits via comments on elements.

### Generate high-fidelity design
- **Timestamp**: [10:00](https://www.youtube.com/watch?v=-W8uYEX4gLQ&t=600)
- **Action**: Request the high-fidelity version, specifying light/dark mode, interactions, and visual details like agent avatars.
- **Command Or Clicks**: Chat: 'Please go for version two' -> 'I want both light and dark mode' -> 'Keep the handdrawn robots' -> continue
- **Choice Branch**: You can ask for mid-fidelity first, but the host skipped directly to hi-fi.

### Handoff to Claude Code
- **Timestamp**: [13:10](https://www.youtube.com/watch?v=-W8uYEX4gLQ&t=790)
- **Action**: Share the design, copy the handoff command, open Claude Code in the project folder, and paste the command to implement the UI.
- **Command Or Clicks**: Click 'share' -> 'hand off to cla code' -> copy command -> open terminal in project folder -> paste command -> run
- **Choice Branch**: Ensure the output file name is correct (e.g., 'local forge' instead of 'paulsbooks.html').

### Fix responsive layout issues
- **Timestamp**: [14:04](https://www.youtube.com/watch?v=-W8uYEX4gLQ&t=844)
- **Action**: Test the implemented UI, identify visual bugs (e.g., agent cards taking too much space), and prompt Claude Code to fix them.
- **Command Or Clicks**: Paste screenshot into Claude Code -> 'These need to be responsive and not take up the entire screen'
- **Choice Branch**: Use screenshots for precise visual feedback on layout issues.

## Gotchas

### Claude Design may name the output file incorrectly (e.g., 'paulsbooks.html' instead of 'local forge').
- **Severity**: serious
- **Timestamp**: [13:10](https://www.youtube.com/watch?v=-W8uYEX4gLQ&t=790)

### Agent cards may take up too much space initially, requiring horizontal scrolling; prompt for responsiveness.
- **Severity**: heads_up
- **Timestamp**: [14:04](https://www.youtube.com/watch?v=-W8uYEX4gLQ&t=844)

## Where to go next

Explore the agent coding master class for building real-world solutions with coding agents like Claude Code and Cursor.

## Concepts surfaced

[[claude-design]] · [[claude-code]] · [[ai-ui-generation]] · [[design-to-code]] · [[voice-dictation-design]] · [[responsive-ui-fix]]
