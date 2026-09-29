---
video_id: 7-evWQJ1Vlw
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-07-09-zcode-glm-52-tutorial-stop-paying-200-for-claude-code.md
source_transcript: ../transcripts/2026-07-09-zcode-glm-52-tutorial-stop-paying-200-for-claude-code.md
source_summary_hash: sha256:24886768030b8507a86eea21b4d5233d5e40c34d71609d595bc33f033922011a
source_transcript_hash: sha256:b868c2d405d7144bc3381e6d11a01baeb286d86e6ec6d1cd271d2ea8731b8e6e
fill_id: 9081b63a-ce0e-4b02-af75-f0fa454be7bd
published_at: '2026-09-29T11:19:50.924574'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Build and deploy web apps with ZCode and GLM 5.2 for a fraction of the cost of Claude Code.

## Prerequisites

### ZCode Desktop App
- **Kind**: tool
- **Note**: Free download from z.ai for Windows, Mac, or Linux.

### Z.AI Account
- **Kind**: account
- **Note**: Required for subscription or API key authentication.

### GitHub Account
- **Kind**: account
- **Note**: Free account for version control and repository hosting.

### Git
- **Kind**: tool
- **Note**: Installed via ZCode agent or manually for local version control.

## Steps

### Download and install ZCode
- **Timestamp**: [02:14](https://www.youtube.com/watch?v=7-evWQJ1Vlw&t=134)
- **Action**: Visit the ZCode website, download the installer for your operating system, and run the installation.
- **Command Or Clicks**: Download installer from z.ai and run setup.

### Connect ZCode account
- **Timestamp**: [03:27](https://www.youtube.com/watch?v=7-evWQJ1Vlw&t=207)
- **Action**: Launch ZCode, click 'Connect', and sign in to your Z.AI account. Upgrade to a paid plan or prepare an API key.
- **Command Or Clicks**: Click Connect -> Sign in to Z.AI.
- **Choice Branch**: Choose subscription or API key payment method.

### Configure API key provider
- **Timestamp**: [04:23](https://www.youtube.com/watch?v=7-evWQJ1Vlw&t=263)
- **Action**: If using API keys, add a custom provider with the GLM base URL and your API key to bypass endpoint issues.
- **Command Or Clicks**: Settings -> Providers -> Add Custom Provider -> Paste API key.
- **Choice Branch**: Use subscription directly or custom API provider.

### Set up Git and GitHub
- **Timestamp**: [05:52](https://www.youtube.com/watch?v=7-evWQJ1Vlw&t=352)
- **Action**: Ask the ZCode agent to install Git and connect to your GitHub account for version control.
- **Command Or Clicks**: Chat: 'Please set up Git and GitHub on this machine and connect to my GitHub account.'

### Create first project
- **Timestamp**: [06:54](https://www.youtube.com/watch?v=7-evWQJ1Vlw&t=414)
- **Action**: Create a new folder and prompt ZCode to build a fireworks web app with specific visual requirements.
- **Command Or Clicks**: New Folder -> Chat: 'Make a fireworks web app...'
- **Choice Branch**: Select 'Edit Automatically' mode and GLM 5.2 model.

### Run parallel sessions
- **Timestamp**: [08:09](https://www.youtube.com/watch?v=7-evWQJ1Vlw&t=489)
- **Action**: Click 'New Task' next to the project to run a second session in parallel for multitasking.
- **Command Or Clicks**: Click 'New Task' in project sidebar.

### Commit to GitHub
- **Timestamp**: [10:54](https://www.youtube.com/watch?v=7-evWQJ1Vlw&t=654)
- **Action**: Ask the agent to create a repository and push the code to GitHub, choosing public or private visibility.
- **Command Or Clicks**: Chat: 'Please create a repository and push these changes.'
- **Choice Branch**: Select Public or Private repository.

### Plan complex project
- **Timestamp**: [13:47](https://www.youtube.com/watch?v=7-evWQJ1Vlw&t=827)
- **Action**: Switch to Planning Mode to flesh out a game idea before implementation, answering agent clarifications.
- **Command Or Clicks**: Mode: Planning -> Chat: 'I want a brick break a game...'
- **Choice Branch**: Approve plan to switch to implementation mode.

### Deploy to Vercel
- **Timestamp**: [16:41](https://www.youtube.com/watch?v=7-evWQJ1Vlw&t=1001)
- **Action**: Connect your GitHub account to Vercel, select the repository, and deploy the app for free.
- **Command Or Clicks**: Vercel Dashboard -> Add New -> Project -> Connect GitHub -> Deploy.

## Gotchas

### Default API key provider may fail due to incorrect endpoint; use custom provider with GLM base URL.
- **Severity**: blocking
- **Timestamp**: [04:23](https://www.youtube.com/watch?v=7-evWQJ1Vlw&t=263)

### Public repositories allow anyone to see and copy your code; choose private if sensitive.
- **Severity**: serious
- **Timestamp**: [10:54](https://www.youtube.com/watch?v=7-evWQJ1Vlw&t=654)

### GLM 5.2 lacks vision capabilities; it reviews HTML, not visual browser interactions.
- **Severity**: heads_up
- **Timestamp**: [00:00](https://www.youtube.com/watch?v=7-evWQJ1Vlw&t=0)

## Where to go next

Explore ZCode's sub-agents and MCP server configuration for advanced automation. Check out the linked Agent Coding Masterclass for deeper skills integration.

## Concepts surfaced

[[zcode-tutorial]] · [[glm-5-2]] · [[ai-coding-agents]] · [[github-integration]] · [[vercel-deployment]] · [[cost-effective-ai]]
