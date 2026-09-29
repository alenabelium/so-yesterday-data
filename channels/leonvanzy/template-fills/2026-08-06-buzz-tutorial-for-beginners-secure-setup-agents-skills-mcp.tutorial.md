---
video_id: xJEFjE88wdw
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-08-06-buzz-tutorial-for-beginners-secure-setup-agents-skills-mcp.md
source_transcript: ../transcripts/2026-08-06-buzz-tutorial-for-beginners-secure-setup-agents-skills-mcp.md
source_summary_hash: sha256:ff9bcf76cb15cf6671d225fcefc56f77ddb82d15e23b3b47f8eae916f4ab01ef
source_transcript_hash: sha256:95701ce1888405b80bd78713c1c374c63e5d38a5e96d900d7112ce4ac2994a7e
fill_id: 1f8f6a37-973a-4eb4-87f2-32899887ff8d
published_at: '2026-09-29T11:22:03.309730'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Securely self-host Buzz on a VPS to create a private, multi-agent team with specialized skills and MCP integrations.

## Prerequisites

### VPS
- **Kind**: hardware
- **Note**: Hostinger VPS (e.g., KVM2) for self-hosting Buzz to ensure data privacy.

### Claude Code
- **Kind**: tool
- **Note**: Required CLI agent. Buzz piggybacks on existing coding agents like Claude Code or CodeEx.

### CodeEx
- **Kind**: tool
- **Note**: Alternative to Claude Code. You only need one of these installed to run Buzz.

## Steps

### Install Buzz locally
- **Timestamp**: [01:15](https://www.youtube.com/watch?v=xJEFjE88wdw&t=75)
- **Action**: Download the latest release from the GitHub repository for your OS and run the installer.
- **Command Or Clicks**: Download .exe (Windows) or equivalent from GitHub releases. Run installer: Next > Next > Finish.
- **Choice Branch**: Select your operating system file from the GitHub latest releases page.

### Generate identity key
- **Timestamp**: [01:44](https://www.youtube.com/watch?v=xJEFjE88wdw&t=104)
- **Action**: Create a unique identity key for your user and save it securely.
- **Command Or Clicks**: Copy the generated identity key and save it in a secure place. Click Next.
- **Choice Branch**: Ensure the key is saved; it is unique to your user.

### Configure default harness
- **Timestamp**: [02:33](https://www.youtube.com/watch?v=xJEFjE88wdw&t=153)
- **Action**: Select your default coding agent (harness) and model. Buzz detects installed agents like Claude Code.
- **Command Or Clicks**: Select 'claude code' as harness and 'opus' as model. Click Next.
- **Choice Branch**: If you use OpenAI, select a GPT model instead.

### Self-host community on VPS
- **Timestamp**: [03:24](https://www.youtube.com/watch?v=xJEFjE88wdw&t=204)
- **Action**: Avoid cloud infrastructure to prevent monitoring. Deploy Buzz on a VPS like Hostinger.
- **Command Or Clicks**: Purchase VPS (e.g., KVM2). Use coupon code 'Leon Buzz' for 10% off. Copy the 'origin' value from the dashboard.
- **Choice Branch**: Use the VPS origin URL to join the community securely.

### Join community via VPS
- **Timestamp**: [04:34](https://www.youtube.com/watch?v=xJEFjE88wdw&t=274)
- **Action**: Paste the VPS origin URL into Buzz to join the self-hosted community.
- **Command Or Clicks**: In Buzz: Join a community > Paste origin URL > Next. Set username and avatar.
- **Choice Branch**: None.

### Create specialized agents
- **Timestamp**: [06:32](https://www.youtube.com/watch?v=xJEFjE88wdw&t=392)
- **Action**: Add new agents with specific roles, personas, and harnesses (e.g., Kimmy Code, Open Code).
- **Command Or Clicks**: Agents > Create Agent. Set name, system prompt, harness, and model. Save changes.
- **Choice Branch**: Restart Buzz for harness changes to take effect.

### Pair mobile device
- **Timestamp**: [10:19](https://www.youtube.com/watch?v=xJEFjE88wdw&t=619)
- **Action**: Install the Buzz app on your phone and pair it to control your team remotely.
- **Command Or Clicks**: Buzz: Mobile > Start Pairing. Scan QR code on device. Confirm numbers.
- **Choice Branch**: None.

### Install skills and MCP servers
- **Timestamp**: [11:31](https://www.youtube.com/watch?v=xJEFjE88wdw&t=691)
- **Action**: Install skills/MCPs via your underlying CLI tool (Claude Code or CodeEx) at user/global level.
- **Command Or Clicks**: Run skills/MCP install commands in Claude Code or CodeEx CLI. Ask agent to install via URL if needed.
- **Choice Branch**: Install globally so all agents in Buzz can access them.

### Orchestrate multi-agent task
- **Timestamp**: [14:37](https://www.youtube.com/watch?v=xJEFjE88wdw&t=877)
- **Action**: Tag a project management agent to delegate tasks to other specialized agents.
- **Command Or Clicks**: Tag @Fizz: 'Create a new channel for my software development team.'
- **Choice Branch**: Ensure the PM agent delegates rather than doing all work itself.

## Gotchas

### Using the cloud community infrastructure may allow them to monitor your messages and data. Self-hosting is recommended for security.
- **Severity**: serious
- **Timestamp**: [02:33](https://www.youtube.com/watch?v=xJEFjE88wdw&t=153)

### You must have either Claude Code or CodeEx installed. Buzz relies on these as its underlying harness.
- **Severity**: blocking
- **Timestamp**: [04:34](https://www.youtube.com/watch?v=xJEFjE88wdw&t=274)

### Skills/MCPs installed for CodeEx only affect CodeEx agents, not Claude agents. Install separately if needed.
- **Severity**: serious
- **Timestamp**: [14:37](https://www.youtube.com/watch?v=xJEFjE88wdw&t=877)

## Where to go next

Explore the linked videos for setting up Claude Code, CodeEx, and using Open Code with open-source models. Join the free community for support.

## Concepts surfaced

[[self-hosted-ai]] · [[multi-agent-orchestration]] · [[mcp-integration]] · [[slack-alternative]] · [[open-source-ai]]
