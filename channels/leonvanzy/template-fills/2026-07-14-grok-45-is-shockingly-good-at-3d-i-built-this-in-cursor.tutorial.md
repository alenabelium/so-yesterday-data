---
video_id: Rdxo4Drwh10
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-07-14-grok-45-is-shockingly-good-at-3d-i-built-this-in-cursor.md
source_transcript: ../transcripts/2026-07-14-grok-45-is-shockingly-good-at-3d-i-built-this-in-cursor.md
source_summary_hash: sha256:7298e35655acaed1aa00ee8338443bb6db6f38dc323a333808a45b52b353b150
source_transcript_hash: sha256:36dcbf304f5c74e15727dddcc1dbc3a6a27f80d16aaa6e7bd14037423b32377e
fill_id: 3fbea305-f42b-4ca7-abb1-99cd05bae568
published_at: '2026-09-29T11:20:21.744692'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Build and deploy a 3D website using Grok 4.5 in Cursor with planning mode and Hostinger MCP integration.

## Prerequisites

### Cursor Individual Plan
- **Kind**: account
- **Note**: Free tier excludes Grok 4.5; upgrade required for model access.

### Hostinger Account
- **Kind**: account
- **Note**: Required for hosting; use code Leon Hosting for 10% discount.

### Hostinger API Config
- **Kind**: tool
- **Note**: JSON config from Hostinger dashboard needed for MCP setup.

## Steps

### Install Cursor and Sign In
- **Timestamp**: [01:04](https://www.youtube.com/watch?v=Rdxo4Drwh10&t=64)
- **Action**: Download Cursor from the official site, install it, and sign in with your account. Ensure you are on the Individual plan to access Grok 4.5.
- **Command Or Clicks**: Go to cursor.com/download, click download, install, then click sign in in the bottom left.
- **Choice Branch**: Select Agent View for accessibility or IDE View for developer familiarity.

### Configure Grok 4.5 and Planning Mode
- **Timestamp**: [04:19](https://www.youtube.com/watch?v=Rdxo4Drwh10&t=259)
- **Action**: Open a new folder for the project. Select Grok 4.5 as the model with high reasoning effort. Switch to Planning Mode to avoid context window limits and agent crashes during long tasks.
- **Command Or Clicks**: Click open folder, select Grok 4.5, set reasoning to high, hold shift+tab to enter planning mode.
- **Choice Branch**: Enable fast mode for speed at higher cost, or keep standard for balance.

### Generate Implementation Plan
- **Timestamp**: [06:46](https://www.youtube.com/watch?v=Rdxo4Drwh10&t=406)
- **Action**: Provide a detailed prompt describing the interior design page and 3D elements. Review the generated plan and to-do list before building.
- **Command Or Clicks**: Type prompt describing design system and 3D room, then send.
- **Choice Branch**: Modify the plan if needed before clicking build.

### Build and Iterate on 3D Scene
- **Timestamp**: [08:49](https://www.youtube.com/watch?v=Rdxo4Drwh10&t=529)
- **Action**: Let the agent build the site. Iterate using natural language or voice commands to fix issues like zoom levels or black walls. Use Cursor's image generation for assets.
- **Command Or Clicks**: Click build, then use voice or text to say 'rotate with mouse' or 'remove black wall'.
- **Choice Branch**: Use embedded image generation for avatars or icons if needed.

### Configure Hostinger MCP in Cursor
- **Timestamp**: [10:59](https://www.youtube.com/watch?v=Rdxo4Drwh10&t=659)
- **Action**: Sign up for Hostinger, get the API JSON config from the dashboard, and paste it into Cursor's MCP settings to enable deployment tools.
- **Command Or Clicks**: Hostinger Dashboard > Dev Tools > API > Copy JSON. In Cursor: Settings > Tools and MCPs > Open Customize > New MCP Server > Paste JSON.
- **Choice Branch**: Ensure all scopes (websites, domain, DNS, etc.) are selected.

### Deploy to Production
- **Timestamp**: [12:11](https://www.youtube.com/watch?v=Rdxo4Drwh10&t=731)
- **Action**: Ask the agent to deploy the project to Hostinger. Authenticate the account via the browser popup when prompted. The agent will handle commits and provide the live URL.
- **Command Or Clicks**: Ask agent: 'Deploy this project to Hostinger', then click authenticate in the browser popup.
- **Choice Branch**: Register a custom domain later via the same process.

## Gotchas

### Grok 4.5 crashes or makes mistakes after ~30 minutes of continuous work. Use Planning Mode to save state and resume safely.
- **Severity**: blocking
- **Timestamp**: [06:46](https://www.youtube.com/watch?v=Rdxo4Drwh10&t=406)

### Grok 4.5 has a 256k context window, much smaller than Opus/GPT. Build iteratively in new sessions rather than one massive solution.
- **Severity**: serious
- **Timestamp**: [08:49](https://www.youtube.com/watch?v=Rdxo4Drwh10&t=529)

### Cursor free tier does not include Grok 4.5. You must upgrade to at least the Individual plan to use this model.
- **Severity**: blocking
- **Timestamp**: [02:27](https://www.youtube.com/watch?v=Rdxo4Drwh10&t=147)

## Where to go next

Explore Agentic coding masterclasses for design systems or try deploying full-stack apps with iterative sessions to manage context limits effectively.

## Concepts surfaced

[[agentic-coding]] · [[cursor-ide]] · [[grok-4-5]] · [[mcp-integration]] · [[hostinger-deployment]] · [[planning-mode]]
