---
video_id: 3B-c34_Fa3Y
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-07-21-kimi-k3-is-claude-level-coding-for-19month.md
source_transcript: ../transcripts/2026-07-21-kimi-k3-is-claude-level-coding-for-19month.md
source_summary_hash: sha256:ef0388cbbb102e915629e13df76ec883bd33d7a3455d2412a146aa45e52235c0
source_transcript_hash: sha256:4b225e046c7630b903064b4cd846845a7350106e0e2e0c5847f92368b8c62e2e
fill_id: 7899309e-4d08-4b05-9fec-6e74a8ca19a7
published_at: '2026-09-29T11:20:52.650869'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Build and deploy a complex 3D web app using Kimi K3's CLI, RAMP framework, and MCP servers for under $20/month.

## Prerequisites

### Kimi Subscription
- **Kind**: account
- **Note**: Monthly plan (~$20) is cheaper than pay-as-you-go API keys.

### Kimi Code CLI
- **Kind**: tool
- **Note**: Native CLI tool installed via official command for best agentic performance.

### VS Code or Cursor
- **Kind**: tool
- **Note**: Recommended IDE to view file changes and manage the terminal.

### Hostinger Account
- **Kind**: account
- **Note**: Required for the MCP server to deploy the app to a live domain.

## Steps

### Install Kimi Code CLI
- **Timestamp**: [01:31](https://www.youtube.com/watch?v=3B-c34_Fa3Y&t=91)
- **Action**: Download and install the Kimi Code CLI tool using the command provided on their website.
- **Command Or Clicks**: Run the installation command for your OS from kimmy.com, then restart your terminal.
- **Choice Branch**: Use the native CLI for best results, or install the VS Code/Cursor extension.

### Authenticate and Select Model
- **Timestamp**: [03:43](https://www.youtube.com/watch?v=3B-c34_Fa3Y&t=223)
- **Action**: Sign in to your Kimi account and switch the active model to Kimi K3 with max reasoning.
- **Command Or Clicks**: Run `/login` to authenticate, then `/model` to select Kimi K3 and set effort to max.
- **Choice Branch**: Choose subscription login over API key for better value.

### Configure Agent Rules
- **Timestamp**: [07:43](https://www.youtube.com/watch?v=3B-c34_Fa3Y&t=463)
- **Action**: Create an `agents.md` file to enforce strict rules like concise responses and testing requirements.
- **Command Or Clicks**: Create `agents.md` and add rules for planning, testing, and UI design.
- **Choice Branch**: Add specific design system rules if building a web app.

### Install MCP Servers
- **Timestamp**: [10:42](https://www.youtube.com/watch?v=3B-c34_Fa3Y&t=642)
- **Action**: Install MCP servers for browser testing (Playwright) and deployment (Hostinger).
- **Command Or Clicks**: Ask the agent to install Playwright MCP, then paste Hostinger API config.
- **Choice Branch**: Use official provider skills for tech stack guidelines.

### Plan the Project
- **Timestamp**: [14:14](https://www.youtube.com/watch?v=3B-c34_Fa3Y&t=854)
- **Action**: Enter planning mode to discuss the project scope and generate a detailed implementation plan.
- **Command Or Clicks**: Press `Shift+Tab` to enter planning mode, then paste the detailed prompt.
- **Choice Branch**: Store the plan in a `plans` folder to save context window space.

### Implement with Swarm
- **Timestamp**: [19:57](https://www.youtube.com/watch?v=3B-c34_Fa3Y&t=1197)
- **Action**: Enable agent swarm to run sub-agents in parallel for complex implementation.
- **Command Or Clicks**: Enable swarm, pull in the plan, and ask the agent to implement the project.
- **Choice Branch**: Avoid swarm for simple projects due to high token usage.

### Deploy to Production
- **Timestamp**: [24:30](https://www.youtube.com/watch?v=3B-c34_Fa3Y&t=1470)
- **Action**: Commit the code and ask the agent to deploy the app to your Hostinger account.
- **Command Or Clicks**: Create a commit, then ask the agent to deploy to Hostinger via the MCP server.
- **Choice Branch**: Authenticate Hostinger account if it's your first deployment.

## Gotchas

### Swarm mode consumes tokens extremely fast and may exceed subscription limits quickly.
- **Severity**: serious
- **Timestamp**: [22:11](https://www.youtube.com/watch?v=3B-c34_Fa3Y&t=1331)

### Kimi K3 has a smaller context window (256k tokens) compared to competitors like GPT-5.
- **Severity**: serious
- **Timestamp**: [18:33](https://www.youtube.com/watch?v=3B-c34_Fa3Y&t=1113)

### Do not use max reasoning effort with swarm for standard projects to avoid excessive costs.
- **Severity**: blocking
- **Timestamp**: [22:11](https://www.youtube.com/watch?v=3B-c34_Fa3Y&t=1331)

## Where to go next

Check the linked GitHub repository for the full prompt and code. Explore the free RAMP framework course for more agentic coding strategies.

## Concepts surfaced

[[agentic-coding]] · [[mcp-servers]] · [[ramp-framework]] · [[context-window-management]] · [[ai-deployment]]
