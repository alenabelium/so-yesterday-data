---
video_id: japT66frdhM
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-03-13-one-simple-system-gave-all-my-ai-tools-a-memory-heres-how.md
source_transcript: ../transcripts/2026-03-13-one-simple-system-gave-all-my-ai-tools-a-memory-heres-how.md
source_summary_hash: sha256:06b6aae1496ef267f0a0f2861f16068ca7984d3d3fdb6307569db0b1794b652c
source_transcript_hash: sha256:46450e4ca8bc2f54ce08279bf6ba035df166505e346a2275fea2eb45082b55d9
fill_id: c7accb2e-6a55-460d-b1fa-0daaba9fdc31
published_at: '2026-10-20T00:41:07.463070'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Build a human-facing web view over your Open Brain Supabase tables so both you and your AI agents read and write the same data through different doors.

## Prerequisites

### Open Brain setup
- **Kind**: knowledge
- **Note**: A personal Supabase database connected to an AI via an MCP server, as described in the previous Open Brain video.

### Supabase account
- **Kind**: account
- **Note**: The same Supabase instance used for Open Brain; you'll create tables and use the built-in table editor.

### Vercel account
- **Kind**: account
- **Note**: Free hosting service to deploy the web app your AI generates; paid plans exist but not needed for this.

### AI coding assistant
- **Kind**: tool
- **Note**: Claude, ChatGPT, or similar to generate the web application code from your description.

## Steps

### Create a table in Supabase for your project
- **Timestamp**: [07:26](https://www.youtube.com/watch?v=japT66frdhM&t=446)
- **Action**: In the same Supabase dashboard you used for Open Brain, create a new table and add columns for the data you want to track. Your agent can immediately reach it through MCP.
- **Command Or Clicks**: Supabase dashboard → New table → define columns
- **Choice Branch**: Start with the built-in table editor if you want a quick functional view; it's not pretty but works.

### Describe your desired view to an AI
- **Timestamp**: [08:13](https://www.youtube.com/watch?v=japT66frdhM&t=493)
- **Action**: Talk to Claude or ChatGPT and describe the mobile-friendly view you want, including fields and highlights. The AI will generate a small web application that connects to your Supabase data.
- **Command Or Clicks**: Prompt: 'I want a mobile friendly view of my maintenance table. It should show every appliance, warranty date, last service date, and highlight anything expiring in the next 30 days.'
- **Choice Branch**: Iterate with the AI on layout and highlights until you're satisfied.

### Deploy the app on Vercel
- **Timestamp**: [08:59](https://www.youtube.com/watch?v=japT66frdhM&t=539)
- **Action**: Create a Vercel account, upload the application your AI built, and Vercel will give you a live URL you can open on any device. Bookmark it on your home screen to behave like an app.
- **Command Or Clicks**: Vercel → New Project → Upload app → Deploy
- **Choice Branch**: Alternatively, connect Supabase to Lovable for a shortcut, but you may prefer to avoid the middleman.

## Gotchas

### Don't add a sync layer or middleware between your data and the view; the table must remain the single source of truth to avoid breakage or lag.
- **Severity**: serious
- **Timestamp**: [04:03](https://www.youtube.com/watch?v=japT66frdhM&t=243)

### The app only lives on your computer until you deploy it; you need Vercel to give it a URL accessible from any device.
- **Severity**: blocking
- **Timestamp**: [08:59](https://www.youtube.com/watch?v=japT66frdhM&t=539)

## Where to go next

Check the Substack guide for build kits and more use cases, or feed this video to your AI to build the extensions yourself.

## Concepts surfaced

[[open-brain]] · [[mcp-server]] · [[supabase]] · [[vercel]] · [[agentic-memory]] · [[single-source-of-truth]]
