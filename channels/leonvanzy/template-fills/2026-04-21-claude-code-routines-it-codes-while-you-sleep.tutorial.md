---
video_id: 5LCjeni0Z-U
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-04-21-claude-code-routines-it-codes-while-you-sleep.md
source_transcript: ../transcripts/2026-04-21-claude-code-routines-it-codes-while-you-sleep.md
source_summary_hash: sha256:c93554e0d22be25edd1aaed9bfa62af0783c9f098e0472e990a59f974f176d9f
source_transcript_hash: sha256:bb6092f230c1bb609e6d91633c28a95b114be0b6379eeac5bc058bddced21e10
fill_id: 229d7285-e8d5-4c3a-b60d-5e1bcbba3540
published_at: '2026-05-18T05:47:00.471098'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Set up automated Claude Code Routines to scan for OWASP security vulnerabilities and implement app improvements via pull requests without manual intervention.

## Prerequisites

### Anthropic Account
- **Kind**: account
- **Note**: Required to access Claude Code web interface and routines. Max plan offers 15 daily runs; Pro plan offers fewer.

### GitHub Repository
- **Kind**: tool
- **Note**: A public or private repo is needed to host the code base and receive the automated pull requests.

### Claude Code Skills
- **Kind**: tool
- **Note**: Skills must be installed directly into the project repository folder, not just uploaded via the chat interface.

## Steps

### Access Routines in Claude Code Web
- **Timestamp**: [04:33](https://www.youtube.com/watch?v=5LCjeni0Z-U&t=273)
- **Action**: Navigate to the Claude Code web interface, select the Routines tab, and initiate a new routine setup.
- **Command Or Clicks**: Go to ClaudeCode web -> Routines -> New routine
- **Choice Branch**: Select the 'Auto Improver' template or start blank.

### Configure Auto-Improver Routine
- **Timestamp**: [04:33](https://www.youtube.com/watch?v=5LCjeni0Z-U&t=273)
- **Action**: Name the routine 'auto improver', select the target repository, and input a prompt instructing Claude to find and implement one meaningful improvement (UI, UX, feature, or bug fix) and create a PR without merging.
- **Command Or Clicks**: Prompt: "Explore the code base and identify one meaningful improvement... Implement the change and create the PR. I'll just add do not merge yet."
- **Choice Branch**: Choose model (e.g., Opus 4.7) and trigger type.

### Set Trigger and Connectors
- **Timestamp**: [04:33](https://www.youtube.com/watch?v=5LCjeni0Z-U&t=273)
- **Action**: Configure the routine to run on a schedule (e.g., every hour) or via GitHub events. Optionally add connectors like Gmail for notifications.
- **Command Or Clicks**: Trigger: Schedule (Every hour) -> Add Connector (Gmail)
- **Choice Branch**: None

### Execute and Review Auto-Improvement
- **Timestamp**: [07:36](https://www.youtube.com/watch?v=5LCjeni0Z-U&t=456)
- **Action**: Manually start the routine or wait for the schedule. Monitor the web session as it creates an isolated feature branch and generates a pull request. Review the PR and merge it to main if satisfied.
- **Command Or Clicks**: Click 'Run' -> Open session -> View PR -> Merge to main
- **Choice Branch**: None

### Install Security Scanner Skill
- **Timestamp**: [08:34](https://www.youtube.com/watch?v=5LCjeni0Z-U&t=514)
- **Action**: Download the 'security scanner' skill from the provided GitHub repository and install it directly into the project's code folder. Note: Chat interface skills do not work for routines.
- **Command Or Clicks**: Clone skill repo -> Copy 'security scanner' folder into project root
- **Choice Branch**: None

### Configure Security Audit Routine
- **Timestamp**: [08:34](https://www.youtube.com/watch?v=5LCjeni0Z-U&t=514)
- **Action**: Create a new routine named 'to-do security audit'. Use a prompt invoking the security scanner skill to audit against OWASP Top 10, fix issues, and create a PR. Decide whether to auto-merge or require review.
- **Command Or Clicks**: Prompt: "Use your security scanner skill... implement fixes... create a pull request and merge the PR once all checks have passed."
- **Choice Branch**: Auto-merge vs. Manual Review

### Run Security Audit and Verify Fixes
- **Timestamp**: [10:21](https://www.youtube.com/watch?v=5LCjeni0Z-U&t=621)
- **Action**: Execute the security routine. Check the generated audit report in the 'audit' folder for critical issues (e.g., hardcoded keys, SQL injection). Verify the PR fixes the vulnerabilities, such as moving keys to environment variables.
- **Command Or Clicks**: Run routine -> Check 'audit' folder -> Review PR -> Merge
- **Choice Branch**: None

## Gotchas

### Skills used in routines must be installed in the project repository folder; standard chat interface skills will not work.
- **Severity**: blocking
- **Timestamp**: [08:34](https://www.youtube.com/watch?v=5LCjeni0Z-U&t=514)

### Routine execution limits depend on your plan; Max plan allows 15 runs/day, while Pro plan has fewer.
- **Severity**: serious
- **Timestamp**: [01:42](https://www.youtube.com/watch?v=5LCjeni0Z-U&t=102)

### Routines run in the cloud, not on your local machine, so you can close your browser without stopping the process.
- **Severity**: heads_up
- **Timestamp**: [07:36](https://www.youtube.com/watch?v=5LCjeni0Z-U&t=456)

## Where to go next

Explore the Agentic Coding Masterclass at Agentic Labs for advanced agent workflows. Check the Claude Code Routines GitHub repo for more skills like the security scanner.

## Concepts surfaced

[[claude-code-routines]] · [[owasp-top-10]] · [[automated-security-audit]] · [[agentic-coding]] · [[pull-request-automation]] · [[cloud-based-ai-agents]]
