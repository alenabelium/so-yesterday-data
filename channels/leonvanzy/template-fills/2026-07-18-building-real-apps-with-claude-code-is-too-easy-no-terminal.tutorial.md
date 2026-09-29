---
video_id: ZW6d_2rwcdk
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-07-18-building-real-apps-with-claude-code-is-too-easy-no-terminal.md
source_transcript: ../transcripts/2026-07-18-building-real-apps-with-claude-code-is-too-easy-no-terminal.md
source_summary_hash: sha256:00340ef3a64779c903553278bde20abc37d1d19be9e62ad51fef77dc04268832
source_transcript_hash: sha256:ea19a94247e3f0b7746bfe2859f18d26086febf6bb722c039e4198a212522049
fill_id: 288f281d-a67e-445d-94b2-4bbb3031b4d8
published_at: '2026-09-29T11:20:39.898268'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Build and test real web apps with Claude Code's desktop app using planning mode, integrated browser testing, and automated Git workflows.

## Prerequisites

### Claude Pro/Max Subscription
- **Kind**: account
- **Note**: Free tier insufficient; paid plan required for Claude Code access.

### GitHub Account
- **Kind**: account
- **Note**: Free account needed for remote code backup and version control.

### Git Installation
- **Kind**: tool
- **Note**: Can be installed by Claude Code or manually before starting.

## Steps

### Install and Subscribe
- **Timestamp**: [01:38](https://www.youtube.com/watch?v=ZW6d_2rwcdk&t=98)
- **Action**: Download the Claude desktop app, install it, and upgrade to a Pro or Max subscription to access the Code tab.
- **Command Or Clicks**: Go to the linked page, download installer, double-click to install, sign in, go to 'View all plans', upgrade to Pro.
- **Choice Branch**: Select Pro plan for starters; Max for heavy usage.

### Configure Workspace and Mode
- **Timestamp**: [04:02](https://www.youtube.com/watch?v=ZW6d_2rwcdk&t=242)
- **Action**: Select a project folder to trust, then choose a mode: Planning (discussion only), Ask Permissions, Accept Edits, or Auto (default).
- **Command Or Clicks**: Click folder name, select directory, click 'Trust'. Click mode button to switch between Planning, Ask Permissions, Accept Edits, or Auto.
- **Choice Branch**: Use Planning mode for architecture; Auto for building.

### Select Model and Effort
- **Timestamp**: [05:59](https://www.youtube.com/watch?v=ZW6d_2rwcdk&t=359)
- **Action**: Choose Opus 4.8 for coding tasks and set effort to High. Avoid Ultra Code to prevent unnecessary costs.
- **Command Or Clicks**: Select 'Opus' from model selector. Select 'High' from effort selector.
- **Choice Branch**: Use Sonnet for documentation; Opus for coding.

### Set Up Git and GitHub
- **Timestamp**: [07:03](https://www.youtube.com/watch?v=ZW6d_2rwcdk&t=423)
- **Action**: Ask Claude to install Git and connect to GitHub for version control and backup.
- **Command Or Clicks**: Prompt: 'please install and set up git on my machine'. Then: 'please set up and connect to github from my machine'.
- **Choice Branch**: Follow authentication link if prompted.

### Build First Project
- **Timestamp**: [09:46](https://www.youtube.com/watch?v=ZW6d_2rwcdk&t=586)
- **Action**: Prompt Claude to build a tip calculator. It creates a folder and runs the app in the integrated browser.
- **Command Or Clicks**: Prompt: 'make a tip calculator I can use in the browser. Let me type in the bill amount, choose a tip percentage, and split it across a number of people.'
- **Choice Branch**: Test the app in the preview window.

### Commit to GitHub
- **Timestamp**: [10:59](https://www.youtube.com/watch?v=ZW6d_2rwcdk&t=659)
- **Action**: Ask Claude to create a GitHub repository and push the project. Choose private or public visibility.
- **Command Or Clicks**: Prompt: 'please create a new GitHub repository and push our project'. Click 'Private' or 'Public' when prompted.
- **Choice Branch**: Select Private for personal projects.

### Integrated Browser Testing
- **Timestamp**: [10:59](https://www.youtube.com/watch?v=ZW6d_2rwcdk&t=659)
- **Action**: Use the integrated browser to test the app and improve the UI without leaving the app.
- **Command Or Clicks**: Prompt: 'please use your browser to test the app. Also see if you could improve the UI.'
- **Choice Branch**: Observe Claude navigating and taking screenshots.

### Plan New Project
- **Timestamp**: [10:59](https://www.youtube.com/watch?v=ZW6d_2rwcdk&t=659)
- **Action**: Switch to Planning mode to discuss architecture for a new project before building.
- **Command Or Clicks**: Click 'Modes' > 'Plan mode' or hold Shift+Tab. Prompt: 'I want to build a daily habit tracker...'
- **Choice Branch**: Revise the plan if needed before accepting.

### Multitask with Multiple Sessions
- **Timestamp**: [13:59](https://www.youtube.com/watch?v=ZW6d_2rwcdk&t=839)
- **Action**: Open a second session in the same project folder to work on multiple tasks simultaneously.
- **Command Or Clicks**: Click '+' button in sidebar, select same project folder. Prompt: 'please describe this project'.
- **Choice Branch**: Switch between sessions in the sidebar.

### Surgical Edits
- **Timestamp**: [15:39](https://www.youtube.com/watch?v=ZW6d_2rwcdk&t=939)
- **Action**: Use the 'Select Elements' button to highlight specific UI parts for precise changes.
- **Command Or Clicks**: Click 'Select Elements', highlight element. Prompt: 'please change the name to Abbott's Forge'.
- **Choice Branch**: Use for specific branding or text changes.

### Merge Pull Request
- **Timestamp**: [17:05](https://www.youtube.com/watch?v=ZW6d_2rwcdk&t=1025)
- **Action**: Click 'Create PR' to push changes to GitHub, then merge the pull request.
- **Command Or Clicks**: Click 'Create PR' button. Click 'Merge PR' in GitHub or ask Claude to merge.
- **Choice Branch**: Review changes in GitHub if technical.

### Connect Third-Party Apps
- **Timestamp**: [19:33](https://www.youtube.com/watch?v=ZW6d_2rwcdk&t=1173)
- **Action**: Browse and install connectors like Gmail to automate actions like sending emails on completion.
- **Command Or Clicks**: Click '+' > 'Connectors' > 'Browse'. Install Gmail. Prompt: 'Whenever you complete a change, send me an email...'
- **Choice Branch**: Update .claude.md for project-specific rules.

### Enable Remote Control
- **Timestamp**: [21:09](https://www.youtube.com/watch?v=ZW6d_2rwcdk&t=1269)
- **Action**: Enable remote control in settings to manage Claude Code sessions on mobile devices.
- **Command Or Clicks**: Go to Settings > Claude Code > Enable 'Remote Control by default'.
- **Choice Branch**: Access via mobile app.

## Gotchas

### Free tier does not include Claude Code; you must upgrade to Pro or Max.
- **Severity**: blocking
- **Timestamp**: [01:38](https://www.youtube.com/watch?v=ZW6d_2rwcdk&t=98)

### Ultra Code mode is very expensive and often overcomplicates tasks; avoid as default.
- **Severity**: serious
- **Timestamp**: [07:03](https://www.youtube.com/watch?v=ZW6d_2rwcdk&t=423)

### Public repositories are visible to everyone; choose Private for personal projects.
- **Severity**: serious
- **Timestamp**: [10:59](https://www.youtube.com/watch?v=ZW6d_2rwcdk&t=659)

## Where to go next

Explore the Agent Coding Master Class for advanced agent fundamentals, MCP servers, and SaaS application building. Check the description for links to the Claude Code course and Agentic Labs.

## Concepts surfaced

[[claude-code-desktop]] · [[planning-mode]] · [[integrated-browser-testing]] · [[git-github-integration]] · [[agent-connectors]] · [[remote-control]]
