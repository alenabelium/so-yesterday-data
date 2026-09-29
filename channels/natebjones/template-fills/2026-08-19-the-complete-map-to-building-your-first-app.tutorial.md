---
video_id: joRXo6x7Pgk
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-08-19-the-complete-map-to-building-your-first-app.md
source_transcript: ../transcripts/2026-08-19-the-complete-map-to-building-your-first-app.md
source_summary_hash: sha256:2d26d3b04d51483c9ddcf4c2e6249529af1d610ca7ab3044056c4e08b4a28c14
source_transcript_hash: sha256:6eff512578e4b4aae029a135e596e173d111f8176a9a6393f82964c8007d4e83
fill_id: 4ddcc385-5c8b-4e34-bdc1-c365356bf79b
published_at: '2026-09-29T11:22:54.895962'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

A complete map for non-developers to build personal software using five 'software shapes' and AI coding agents like Lovable or Claude Code.

## Prerequisites

### Lovable Account
- **Kind**: account
- **Note**: Hosted AI builder for quick web app validation without installing languages.

### GitHub Account
- **Kind**: account
- **Note**: Optional but recommended for source code portability and history tracking.

### Basic Tech Literacy
- **Kind**: knowledge
- **Note**: Understanding that you don't need to memorize stacks, just make one good decision at a time.

## Steps

### Define your software shape
- **Timestamp**: [03:18](https://www.youtube.com/watch?v=joRXo6x7Pgk&t=198)
- **Action**: Identify if your project is a local tool, web app, native mobile app, background service, or hardware integration to determine the right technical approach.
- **Command Or Clicks**: N/A
- **Choice Branch**: Start with Lovable for quick web apps; use coding agents for complex or hardware projects.

### Set up hosted builder and GitHub
- **Timestamp**: [07:22](https://www.youtube.com/watch?v=joRXo6x7Pgk&t=442)
- **Action**: Use Lovable to describe your software, create the project, and connect GitHub to ensure data portability from the start.
- **Command Or Clicks**: Connect GitHub in Lovable settings.
- **Choice Branch**: Choose Lovable Cloud for ease or Supabase for long-term data ownership.

### Choose database strategy
- **Timestamp**: [08:21](https://www.youtube.com/watch?v=joRXo6x7Pgk&t=501)
- **Action**: Decide between Lovable Cloud for simplicity or Supabase for a separate, portable Postgres database and auth layer.
- **Command Or Clicks**: Select Supabase in Lovable if portability is critical.
- **Choice Branch**: Use SQLite for simple local-only tools.

### Configure coding agent environment
- **Timestamp**: [10:46](https://www.youtube.com/watch?v=joRXo6x7Pgk&t=646)
- **Action**: For advanced control, use CodeEx or Claude Code with GitHub Desktop, Supabase, and Vercel for a decoupled stack.
- **Command Or Clicks**: Install GitHub Desktop; connect Supabase and Vercel.
- **Choice Branch**: Use GLM 5.3 via API key if you prefer open-source models.

### Create project documentation files
- **Timestamp**: [17:31](https://www.youtube.com/watch?v=joRXo6x7Pgk&t=1051)
- **Action**: Write four markdown files to guide the AI: project.md, decisions.md, scenarios.md, and agents.md/claude.md.
- **Command Or Clicks**: Create project.md, decisions.md, scenarios.md, and agents.md in your repo.
- **Choice Branch**: Keep secrets out of code; use host-provided secret settings.

### Test with real-world scenarios
- **Timestamp**: [27:43](https://www.youtube.com/watch?v=joRXo6x7Pgk&t=1663)
- **Action**: Manually test the app against the scenarios in your documentation to ensure it handles edge cases and unhappy paths.
- **Command Or Clicks**: Run through scenarios like unreadable photos or missing data.
- **Choice Branch**: Do not rely solely on the agent's claim that testing is done.

## Gotchas

### Never put API keys or passwords in visible code, screenshots, or GitHub commits; use host secret settings instead.
- **Severity**: serious
- **Timestamp**: [19:53](https://www.youtube.com/watch?v=joRXo6x7Pgk&t=1193)

### Do not make apps public or add paid services without explicitly asking the model to explain cost and access implications first.
- **Severity**: blocking
- **Timestamp**: [18:30](https://www.youtube.com/watch?v=joRXo6x7Pgk&t=1110)

### Hiding a button is not access control; enforce permissions at the database level to prevent data leakage between users.
- **Severity**: serious
- **Timestamp**: [25:01](https://www.youtube.com/watch?v=joRXo6x7Pgk&t=1501)

## Where to go next

Check the Substack guide for setup details and join the Slack community for peer support on your specific software shape.

## Concepts surfaced

[[personal-software]] · [[ai-coding-agents]] · [[software-shapes]] · [[data-portability]] · [[vibe-coding-best-practices]]
