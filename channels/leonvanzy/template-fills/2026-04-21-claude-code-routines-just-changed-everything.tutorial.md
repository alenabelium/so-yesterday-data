---
video_id: bzYheNpYl8Y
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-04-21-claude-code-routines-just-changed-everything.md
source_transcript: ../transcripts/2026-04-21-claude-code-routines-just-changed-everything.md
source_summary_hash: sha256:86cced3c052b1ed919c7a75c3cf5a2d2ff0c9a7b50cce8f8c2c2c08337919772
source_transcript_hash: sha256:3a1db2d0ef1e2a8d8350401d2300be5f90c430e38012cd7eded14a979ee3b66b
fill_id: 82d4824c-2b89-41de-9ee3-33fb2e5a5f88
published_at: '2026-05-19T08:13:17.739552'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Automate code audits and improvements with Claude Code Routines to fix security vulnerabilities and UX gaps without manual effort.

## Prerequisites

### Claude Code Max/Pro Plan
- **Kind**: account
- **Note**: Requires a paid plan; Max allows 15 daily runs, Pro allows fewer.

### GitHub Repository
- **Kind**: tool
- **Note**: A public or private repo is needed to hook up to the routine.

### OWASP Top 10 Knowledge
- **Kind**: knowledge
- **Note**: Understanding of the top 10 critical web application security risks.

## Steps

### Create auto-improver routine
- **Timestamp**: [02:45](https://www.youtube.com/watch?v=bzYheNpYl8Y&t=165)
- **Action**: Navigate to Claude Code web, select new routine, name it 'auto improver', and select your repository.
- **Command Or Clicks**: Go to Claude Code web > Routines > New routine > Name: auto improver > Select Repo
- **Choice Branch**: Select the repository you want to improve.

### Configure improvement prompt
- **Timestamp**: [04:33](https://www.youtube.com/watch?v=bzYheNpYl8Y&t=273)
- **Action**: Enter a prompt instructing Claude to find one meaningful improvement (UI/UX/feature), implement it, and create a PR without merging.
- **Command Or Clicks**: Prompt: 'Explore the code base and identify one meaningful improvement... Implement the change and create the PR. I'll just add do not merge yet.'
- **Choice Branch**: Choose Opus 4.7 model or default.

### Set schedule trigger
- **Timestamp**: [05:15](https://www.youtube.com/watch?v=bzYheNpYl8Y&t=315)
- **Action**: Set the trigger to run on a schedule (e.g., every hour) and optionally add connectors like Gmail for notifications.
- **Command Or Clicks**: Trigger: Schedule (every hour) > Add Connector (Gmail) > Create routine
- **Choice Branch**: Choose between schedule, GitHub event, or API endpoint trigger.

### Install OWASP security skill
- **Timestamp**: [09:10](https://www.youtube.com/watch?v=bzYheNpYl8Y&t=550)
- **Action**: Clone the provided GitHub repository containing the 'security scanner' skill and install it into your project folder.
- **Command Or Clicks**: Clone repo > Copy 'security scanner' skill into project folder
- **Choice Branch**: Skills must be installed in the code project repository, not just the chat interface.

### Create security audit routine
- **Timestamp**: [10:00](https://www.youtube.com/watch?v=bzYheNpYl8Y&t=600)
- **Action**: Create a new routine named 'to-do security audit' with a prompt invoking the security scanner skill to fix issues and merge PRs.
- **Command Or Clicks**: Prompt: 'Use your security scanner skill... implement fixes... create a pull request and merge the PR once all checks have passed.'
- **Choice Branch**: Choose to auto-merge or review PRs first.

### Run and verify audit
- **Timestamp**: [11:22](https://www.youtube.com/watch?v=bzYheNpYl8Y&t=682)
- **Action**: Execute the routine, check the generated audit report in the 'audit' folder, and verify the merged pull request fixes vulnerabilities.
- **Command Or Clicks**: Run routine > Check 'audit' folder for report > Verify PR merge
- **Choice Branch**: Review the executive summary and specific issues like broken access control.

## Gotchas

### Skills for routines must be installed in the actual code project repository, not just the Claude chat interface.
- **Severity**: blocking
- **Timestamp**: [09:30](https://www.youtube.com/watch?v=bzYheNpYl8Y&t=570)

### Daily run limits depend on your plan; Max allows 15 runs, Pro allows fewer.
- **Severity**: serious
- **Timestamp**: [02:10](https://www.youtube.com/watch?v=bzYheNpYl8Y&t=130)

### Hardcoded API keys in public repos expose sensitive data immediately.
- **Severity**: serious
- **Timestamp**: [03:00](https://www.youtube.com/watch?v=bzYheNpYl8Y&t=180)

## Where to go next

Explore the Agentic Labs masterclass for advanced agentic coding skills. Check the provided GitHub repo for the OWASP security scanner skill template.

## Concepts surfaced

[[claude-code-routines]] · [[automated-security-audit]] · [[owasp-top-10]] · [[pull-request-automation]] · [[cloud-based-ai-agents]]
