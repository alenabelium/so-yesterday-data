---
video_id: cT1zhqtrDSk
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-06-22-how-i-run-my-100k-channel-with-claude-and-cowork.md
source_transcript: ../transcripts/2026-06-22-how-i-run-my-100k-channel-with-claude-and-cowork.md
source_summary_hash: sha256:e691f940b396b9efdd50f3620eaee5000b39c3269aa13e451de82a3e269d2b23
source_transcript_hash: sha256:c59529cc28016d96d10fd6a69236770fd31afe53c6bebc19fcb72d06771449db
fill_id: 78bae250-c517-4ce6-9f48-bbdd356a8bce
published_at: '2026-09-29T11:05:49.842708'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Leon van Zyl automates his 100K YouTube channel workflow using Cowork agents for research and email negotiation, and Claude with VidIQ for data-driven content creation.

## Prerequisites

### Cowork Account
- **Kind**: account
- **Note**: Required to run the automated 'good morning' research and email negotiation agents.

### VidIQ MCP
- **Kind**: tool
- **Note**: Connect to Claude to enable keyword research and channel health analysis via MCP server.

### Claude Session
- **Kind**: tool
- **Note**: Used for generating video titles, hooks, and verifying feature availability with live data.

### DaVinci Resolve
- **Kind**: tool
- **Note**: Used for final video editing, AI subtitle generation, and audio mixing.

## Steps

### Set up Cowork morning agent
- **Timestamp**: [06:07](https://www.youtube.com/watch?v=cT1zhqtrDSk&t=367)
- **Action**: Create a daily 'good morning' task in Cowork that scans for new AI tool updates and runs VidIQ analysis on your channel health and competitor outliers.
- **Command Or Clicks**: Create task 'good morning'; connect VidIQ MCP; set schedule to 7:00 AM daily.
- **Choice Branch**: Also create an email negotiation agent to filter partnership emails and handle rate discussions automatically.

### Research topic with Claude
- **Timestamp**: [14:24](https://www.youtube.com/watch?v=cT1zhqtrDSk&t=864)
- **Action**: In a new Claude session, paste your video concept and ask for packaging help, specifically requesting title ideas and a hook based on factual data rather than guesses.
- **Command Or Clicks**: Prompt: 'Help me with packaging. Intro, hook, title ideas.' Paste concept.
- **Choice Branch**: Ensure VidIQ connector is active in Claude to pull real-time search volume data.

### Validate keywords via VidIQ
- **Timestamp**: [15:52](https://www.youtube.com/watch?v=cT1zhqtrDSk&t=952)
- **Action**: Instruct Claude to use the VidIQ tool to retrieve high-search-volume keywords for your topic and score title candidates, aiming for scores over 80%.
- **Command Or Clicks**: Prompt: 'Use VidIQ tool to retrieve keywords... score titles... give top two titles over 80%.'
- **Choice Branch**: Review the generated title contenders and select the highest-scoring option.

### Generate thumbnail with ChatGPT
- **Timestamp**: [19:57](https://www.youtube.com/watch?v=cT1zhqtrDSk&t=1197)
- **Action**: Upload reference images of yourself and brand logos to ChatGPT with Image 2. Prompt it to create a YouTube thumbnail with specific text and composition instructions.
- **Command Or Clicks**: Upload image; Prompt: 'Create YouTube thumbnail... hold 100k play button... add text thank you.'
- **Choice Branch**: Use this method to avoid expensive thumbnail designers and maintain brand consistency.

### Record and edit with DaVinci
- **Timestamp**: [21:15](https://www.youtube.com/watch?v=cT1zhqtrDSk&t=1275)
- **Action**: Record screen with OBS, cut silent parts with Recut, then import to DaVinci Resolve Studio. Use AI tools to auto-generate subtitles and mix audio.
- **Command Or Clicks**: Timeline > AI Tools > Create subtitles from audio. AI Tools > Audio Assistant.
- **Choice Branch**: Use the paid version for AI audio assistant and auto-subtitles, or free version for basic editing.

## Gotchas

### Don't guess keywords or titles; use VidIQ data to ensure search intent and avoid creating content with no audience.
- **Severity**: serious
- **Timestamp**: [17:03](https://www.youtube.com/watch?v=cT1zhqtrDSk&t=1023)

### Avoid hiring thumbnail designers if you are starting out; AI generation is cheaper and prevents financial loss if videos underperform.
- **Severity**: heads_up
- **Timestamp**: [19:57](https://www.youtube.com/watch?v=cT1zhqtrDSk&t=1197)

### Don't rely solely on coding agents without understanding underlying code; value remains in learning to code manually.
- **Severity**: heads_up
- **Timestamp**: [13:24](https://www.youtube.com/watch?v=cT1zhqtrDSk&t=804)

## Where to go next

Next, explore how to build your own Cowork agent harnesses like Cole Madden's tutorials, or dive deeper into DaVinci Resolve's AI audio features for professional-grade sound mixing.

## Concepts surfaced

[[cowork-agents]] · [[vidiq-mcp]] · [[claude-research]] · [[davinci-ai]] · [[thumbnail-automation]]
