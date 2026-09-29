---
video_id: nIWGYXEzqJA
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-08-11-oracle-fusion-ai-studio-the-complete-enterprise-coding-agent.md
source_transcript: ../transcripts/2026-08-11-oracle-fusion-ai-studio-the-complete-enterprise-coding-agent.md
source_summary_hash: sha256:a999fb3eabc52a60a79025f4171ffc779a324c91483e9b42094d932248f1ab7c
source_transcript_hash: sha256:d4d48c2ce6ba2adebf28c1542413730ff80ef909f82ab4d2a7b758f086d90d16
fill_id: 84152a19-36b1-409a-8e33-590312b27d6b
published_at: '2026-09-29T11:22:15.490426'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Oracle Fusion AI Studio uses five strict rules to let coding agents autonomously build, validate, and deploy enterprise extensions using live cloud data.

## Prerequisites

### Oracle Fusion Account
- **Kind**: account
- **Note**: Access to Oracle Fusion Applications and a valid URL for authentication.

### Oracle Fusion AI Studio Repo
- **Kind**: tool
- **Note**: Public repository containing agent skills, CLI tools, and VS Code extensions.

### Coding Agent
- **Kind**: tool
- **Note**: Any coding agent like Codex or Claude Code to execute the workflow.

## Steps

### Install VS Code Extension
- **Timestamp**: [09:08](https://www.youtube.com/watch?v=nIWGYXEzqJA&t=548)
- **Action**: Extract the AI Studio extensions zip from the repo's bin folder, then install the extension in VS Code via the 'Install from VSIX' menu.
- **Command Or Clicks**: Extensions > Three Dots > Install from VSIX > Select AI Studio extension file
- **Choice Branch**: Use the VSIX installer for local extensions rather than the marketplace.

### Configure Authentication
- **Timestamp**: [10:23](https://www.youtube.com/watch?v=nIWGYXEzqJA&t=623)
- **Action**: Trigger the authentication configuration command, select basic authentication, and input your Oracle Fusion URL, username, and password to generate the env.properties file.
- **Command Or Clicks**: Ctrl+Shift+P > Search 'Fusion AI Studio' > Configure Authentication > Basic Authentication
- **Choice Branch**: Ensure you have a valid Oracle Fusion account URL before starting.

### Install Agent Skills
- **Timestamp**: [10:23](https://www.youtube.com/watch?v=nIWGYXEzqJA&t=623)
- **Action**: Extract the AI Studio skill folder and copy the skills into your project's .agents/skills directory to teach the agent domain-specific rules.
- **Command Or Clicks**: Copy AI Studio skill folder into .agents/skills
- **Choice Branch**: Create a .cloud folder if using cloud models, otherwise use .agents.

### Verify CLI and Skills
- **Timestamp**: [13:31](https://www.youtube.com/watch?v=nIWGYXEzqJA&t=811)
- **Action**: Run the CLI tool to verify it is working and list the installed skills to confirm the agent can see the new domain expertise.
- **Command Or Clicks**: Run CLI tool command > Type 'skills list skills' in agent
- **Choice Branch**: Check for function/tool output to confirm CLI connectivity.

### Prompt for Succession App
- **Timestamp**: [13:31](https://www.youtube.com/watch?v=nIWGYXEzqJA&t=811)
- **Action**: Send a detailed prompt to the coding agent to design a succession planning app, triggering the agent to use the installed succession management skill.
- **Command Or Clicks**: Send prompt: 'Design and build a succession planning agenda gap...'
- **Choice Branch**: Specify MVP scope to guide the agent's initial discovery phase.

### Manage Git and Spec
- **Timestamp**: [15:49](https://www.youtube.com/watch?v=nIWGYXEzqJA&t=949)
- **Action**: Create a .gitignore file to exclude env.properties, commit the initial structure, and review the agent's generated spec for approval.
- **Command Or Clicks**: Create .gitignore > Add 'env.properties' > Commit 'initial'
- **Choice Branch**: Never commit credentials or local environment files.

### Deploy and Test Live Data
- **Timestamp**: [19:59](https://www.youtube.com/watch?v=nIWGYXEzqJA&t=1199)
- **Action**: Click the play button to deploy the app to Fusion Cloud in draft state, then test it with live data to verify functionality and agent recommendations.
- **Command Or Clicks**: Click Play button to deploy > Test with live data queries
- **Choice Branch**: Agents cannot publish; this is a manual review gate.

## Gotchas

### The env.properties file contains credentials and must be ignored by Git to prevent security leaks.
- **Severity**: blocking
- **Timestamp**: [15:49](https://www.youtube.com/watch?v=nIWGYXEzqJA&t=949)

### Agents operate in read-only mode by default; you must explicitly instruct them to create or modify data.
- **Severity**: serious
- **Timestamp**: [05:37](https://www.youtube.com/watch?v=nIWGYXEzqJA&t=337)

### Work is not complete until validated by Oracle Agent Studio; local success does not guarantee cloud compatibility.
- **Severity**: blocking
- **Timestamp**: [06:34](https://www.youtube.com/watch?v=nIWGYXEzqJA&t=394)

## Where to go next

Explore the public Oracle Fusion AI Studio repo for more domain-specific skills like warehouse operations. Apply these five rules to your own enterprise coding workflows to bridge the gap between business requirements and technical implementation.

## Concepts surfaced

[[enterprise-ai-agents]] · [[coding-agent-workflow]] · [[oracle-fusion-ai]] · [[agent-skills]] · [[read-only-defaults]] · [[live-data-validation]]
