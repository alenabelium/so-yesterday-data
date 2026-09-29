---
video_id: iUDuN9dyuTY
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-07-29-stop-babysitting-claude-code-run-it-in-a-sandbox-instead.md
source_transcript: ../transcripts/2026-07-29-stop-babysitting-claude-code-run-it-in-a-sandbox-instead.md
source_summary_hash: sha256:6f8332fcb0079d58a805a0ffd48183e0fdbc8ecaec475d1085968a4e2e4b2bac
source_transcript_hash: sha256:f34475a0cfaa06ceba399d9f23fab210012a353c40f5b741da39d85f0079799e
fill_id: 4a9f3e7d-9bbf-4b68-8f44-4318b06131b2
published_at: '2026-09-29T11:21:27.549739'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Run Claude Code in Docker Sandboxes to isolate AI agents from your host machine, preventing credential leaks and prompt injection risks while enabling safe YOLO mode automation.

## Prerequisites

### Docker Desktop
- **Kind**: tool
- **Note**: Installed on your host machine to support the underlying hypervisor for microVMs.

### GitHub CLI
- **Kind**: tool
- **Note**: Installed and authenticated on the host machine to securely pipe tokens into the sandbox.

### Claude Code
- **Kind**: tool
- **Note**: The AI coding agent to be run inside the isolated sandbox environment.

## Steps

### Install Docker Sandboxes
- **Timestamp**: [06:23](https://www.youtube.com/watch?v=iUDuN9dyuTY&t=383)
- **Action**: Copy the installation command for your OS from the Docker website and run it in your terminal (e.g., PowerShell on Windows).
- **Command Or Clicks**: Copy Windows command from website -> Paste into PowerShell -> Run
- **Choice Branch**: Choose the command corresponding to your operating system.

### Initialize and Login
- **Timestamp**: [07:10](https://www.youtube.com/watch?v=iUDuN9dyuTY&t=430)
- **Action**: Run the spx command to log in and confirm the authentication code to complete the setup.
- **Command Or Clicks**: spx login
- **Choice Branch**: Follow the on-screen prompt to confirm the code.

### Run Claude in Sandbox
- **Timestamp**: [07:10](https://www.youtube.com/watch?v=iUDuN9dyuTY&t=430)
- **Action**: Open your project terminal and run Claude Code wrapped in the spx command to start it in an isolated microVM.
- **Command Or Clicks**: spx run claude
- **Choice Branch**: Replace 'claude' with 'codeex' or 'copilot' if using different agents.

### Select Network Policy
- **Timestamp**: [08:32](https://www.youtube.com/watch?v=iUDuN9dyuTY&t=512)
- **Action**: Choose a network policy when prompted. 'Balanced' allows common dev sites like npm but blocks others like Amazon.
- **Command Or Clicks**: Select 'balanced' from the wizard options
- **Choice Branch**: Options are: open (all access), lockdown (no access), or balanced (dev sites only).

### Authenticate Claude Code
- **Timestamp**: [08:32](https://www.youtube.com/watch?v=iUDuN9dyuTY&t=512)
- **Action**: Inside the sandbox, run the login command to authenticate your Claude Code subscription or API keys.
- **Command Or Clicks**: /login
- **Choice Branch**: Follow the authentication workflow provided by the CLI.

### Unblock Specific Domains
- **Timestamp**: [09:31](https://www.youtube.com/watch?v=iUDuN9dyuTY&t=571)
- **Action**: If a domain is blocked in balanced mode, copy the unblock command provided by the agent and paste it into a new session.
- **Command Or Clicks**: Paste the command provided by the agent to unblock direct fetches
- **Choice Branch**: The agent suggests the command when it encounters a forbidden domain.

### Reset Policy if Needed
- **Timestamp**: [09:31](https://www.youtube.com/watch?v=iUDuN9dyuTY&t=571)
- **Action**: If the policy is too strict, reset it to return to the wizard and choose a different setting.
- **Command Or Clicks**: spx policy reset
- **Choice Branch**: Confirm with 'yes' to reset.

### Securely Inject GitHub Token
- **Timestamp**: [11:38](https://www.youtube.com/watch?v=iUDuN9dyuTY&t=698)
- **Action**: On the host machine, pipe your GitHub token into the sandbox's secret store to avoid storing it on the host or leaking it via prompt injection.
- **Command Or Clicks**: gh auth token | spx secret set github
- **Choice Branch**: Ensure gh CLI is authenticated on the host first.

### Verify Secret Injection
- **Timestamp**: [11:38](https://www.youtube.com/watch?v=iUDuN9dyuTY&t=698)
- **Action**: Inside the sandbox, list secrets to confirm the GitHub token is present alongside the default Anthropic secret.
- **Command Or Clicks**: spx secret ls
- **Choice Branch**: None.

### Recreate Sandbox for Env Vars
- **Timestamp**: [13:10](https://www.youtube.com/watch?v=iUDuN9dyuTY&t=790)
- **Action**: Delete the current sandbox and recreate it so the newly injected environment variables become active.
- **Command Or Clicks**: spx ls -> spx rm <sandbox-name> -> spx run claude
- **Choice Branch**: Copy the sandbox name from spx ls before removing it.

### Triage Issues with Agent
- **Timestamp**: [13:27](https://www.youtube.com/watch?v=iUDuN9dyuTY&t=807)
- **Action**: Ask the agent to connect to your GitHub repo, triage open issues, and create a prioritized HTML report.
- **Command Or Clicks**: Prompt: 'Connect to AutoForge GitHub repo and triage open issues... create an HTML file'
- **Choice Branch**: Switch model to 'fable' and set effort to 'high' for complex tasks.

### Review and Merge PR
- **Timestamp**: [17:11](https://www.youtube.com/watch?v=iUDuN9dyuTY&t=1031)
- **Action**: Review the generated pull request in GitHub. If satisfied, merge it. The sandbox is disposable and can be removed afterward.
- **Command Or Clicks**: Merge PR in GitHub UI -> spx rm <sandbox-name>
- **Choice Branch**: The sandbox is disposable; delete it when done.

## Gotchas

### Running agents in YOLO mode on the host allows them to access all files, credentials, and sibling folders, risking data leaks or unintended changes.
- **Severity**: blocking
- **Timestamp**: [01:10](https://www.youtube.com/watch?v=iUDuN9dyuTY&t=70)

### Environment variables injected into the sandbox do not take effect until you delete and recreate the sandbox instance.
- **Severity**: serious
- **Timestamp**: [13:10](https://www.youtube.com/watch?v=iUDuN9dyuTY&t=790)

### Storing secrets on the host machine risks leakage if the agent is prompted to read them; use spx secret to store them securely inside the sandbox.
- **Severity**: serious
- **Timestamp**: [11:38](https://www.youtube.com/watch?v=iUDuN9dyuTY&t=698)

## Where to go next

Docker Sandboxes provide microVM isolation for AI agents. Explore how to configure network policies for specific domains or integrate other coding agents like CodeEx into this secure workflow.

## Concepts surfaced

[[docker-sandboxes]] · [[claude-code]] · [[ai-safety]] · [[prompt-injection]] · [[microvm]] · [[secure-secrets]]
