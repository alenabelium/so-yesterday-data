---
video_id: X_oW2ZNJfcM
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-07-08-i-cant-afford-developers-so-these-ai-agents-work-247-instead.md
source_transcript: ../transcripts/2026-07-08-i-cant-afford-developers-so-these-ai-agents-work-247-instead.md
source_summary_hash: sha256:92d2fe4ac136c588d4eeafb4adff92fc7ea29e58ab59162f1caa3988757578ca
source_transcript_hash: sha256:5e0c40c3ec7a54d94427924eea25cde48550d5a393aa061febe0d33d166bbdf4
fill_id: 5c284117-5aba-4733-8597-bd7ce9c45354
published_at: '2026-09-29T11:19:41.311800'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Deploy three autonomous AI agents on a VPS to monitor, fix, and improve your app 24/7 via GitHub pull requests.

## Prerequisites

### GitHub Account
- **Kind**: account
- **Note**: Required to host the repository and manage fine-grained access tokens for the agent.

### ChatGPT Subscription
- **Kind**: account
- **Note**: Recommended over API keys for cost efficiency when running the Codex CLI.

### VPS Hosting
- **Kind**: hardware
- **Note**: A 24/7 virtual private server (e.g., Hostinger) to keep agents running without local power issues.

### Terminal Knowledge
- **Kind**: knowledge
- **Note**: Basic ability to run commands, manage cron jobs, and handle environment variables.

## Steps

### Deploy project to GitHub
- **Timestamp**: [04:52](https://www.youtube.com/watch?v=X_oW2ZNJfcM&t=292)
- **Action**: Ensure your code is hosted on GitHub, as the agent requires repository access to clone, modify, and push changes.
- **Command Or Clicks**: Push local code to GitHub repository.
- **Choice Branch**: Use GitHub or another supported repository system.

### Create GitHub Fine-Grained Token
- **Timestamp**: [05:30](https://www.youtube.com/watch?v=X_oW2ZNJfcM&t=330)
- **Action**: Generate a fine-grained personal access token with read/write permissions for contents, metadata, issues, pull requests, and actions.
- **Command Or Clicks**: Profile > Settings > Developer settings > Personal access tokens > Fine-grained tokens > Generate token.
- **Choice Branch**: Select specific repositories rather than all public ones for security.

### Provision VPS with Codex Template
- **Timestamp**: [07:02](https://www.youtube.com/watch?v=X_oW2ZNJfcM&t=422)
- **Action**: Rent a VPS (e.g., Hostinger KVM 2) and select the OpenAI Codex application template to pre-install the CLI.
- **Command Or Clicks**: Hostinger > Choose Plan > Application: OpenAI Codex > Checkout.
- **Choice Branch**: Use promo code 'Leon Codex' for 10% off if available.

### Install and Authenticate Codex CLI
- **Timestamp**: [08:26](https://www.youtube.com/watch?v=X_oW2ZNJfcM&t=506)
- **Action**: Access the VPS terminal, run the Codex command, and authenticate using your ChatGPT subscription via the provided link.
- **Command Or Clicks**: Terminal > codex > Select option 2 (ChatGPT account) > Paste code from terminal into browser.
- **Choice Branch**: Option 1 (VPS login) won't work; Option 3 (API key) is more expensive.

### Configure GitHub Access in Codex
- **Timestamp**: [09:22](https://www.youtube.com/watch?v=X_oW2ZNJfcM&t=562)
- **Action**: Ask Codex to set up GitHub access by providing the fine-grained token and required permissions (read/write repos, PRs, issues).
- **Command Or Clicks**: In Codex CLI: 'Set up access to GitHub... Use this fine-grained personal access token: [TOKEN]'.
- **Choice Branch**: Do not share real tokens with agents; ask for secure environment variable setup instead.

### Clone Repository on VPS
- **Timestamp**: [10:09](https://www.youtube.com/watch?v=X_oW2ZNJfcM&t=609)
- **Action**: Instruct Codex to create a projects folder and clone your specific repository onto the VPS.
- **Command Or Clicks**: In Codex CLI: 'Create a new folder called projects and clone down the CRM Forge repo in that folder.'
- **Choice Branch**: Ensure the agent targets the correct directory.

### Set Up Cron Jobs for Agents
- **Timestamp**: [11:36](https://www.youtube.com/watch?v=X_oW2ZNJfcM&t=696)
- **Action**: Use Codex to generate cron jobs that run 'codex exec' every 10 minutes with specific prompts for bug fixing, security, or improvements.
- **Command Or Clicks**: In Codex CLI: 'Set up a cron job that runs every 10 minutes... runs a Codex exec session with the prompt...'
- **Choice Branch**: Create separate agents for bugs, security, and UI/UX improvements.

## Gotchas

### Do not share real GitHub tokens with agents; ask for secure environment variable setup instead to avoid security risks.
- **Severity**: serious
- **Timestamp**: [09:22](https://www.youtube.com/watch?v=X_oW2ZNJfcM&t=562)

### Codex Cloud containers are temporary (12 hours) and destroy all code/data; use a VPS for persistent background agents.
- **Severity**: blocking
- **Timestamp**: [01:06](https://www.youtube.com/watch?v=X_oW2ZNJfcM&t=66)

### Local PC setups fail due to power outages or Wi-Fi drops; a 24/7 VPS is required for reliable autonomous operation.
- **Severity**: serious
- **Timestamp**: [01:06](https://www.youtube.com/watch?v=X_oW2ZNJfcM&t=66)

## Where to go next

Check out the Agentic Coding Masterclass for deep dives into design systems, SaaS builds, and MCP tools. Subscribe for more tutorials on autonomous AI workflows.

## Concepts surfaced

[[autonomous-ai-agents]] · [[vps-deployment]] · [[github-actions]] · [[cron-jobs]] · [[codex-cli]] · [[fine-grained-tokens]]
