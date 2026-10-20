---
video_id: HaEZgh2RadQ
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-10-19-build-a-full-game-with-claude-code-story-voices-ending.md
source_transcript: ../transcripts/2026-10-19-build-a-full-game-with-claude-code-story-voices-ending.md
source_summary_hash: sha256:ea0a117fe76a29d31d87aa35917853e1610a221483acad26c4e3d896caceab40
source_transcript_hash: sha256:dc14ee27dd17177a44165842438ddaf6cb838627a40e16e7987e4cd838d67bfd
fill_id: c27cf52d-13c8-4b9a-bbb6-84a96deece37
published_at: '2026-10-20T05:28:26.605193'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Create a complete game with story, voice acting, music, and deployment using Claude Code, no coding required.

## Prerequisites

### Claude subscription
- **Kind**: account
- **Note**: Required for Claude Code; API tokens not recommended for this complex task.

### Claude desktop app
- **Kind**: tool
- **Note**: Used in the video; create a new session and select a project folder.

### 11 Labs account (optional)
- **Kind**: account
- **Note**: For voice acting and sound effects; local open-source alternatives exist.

### Hostinger account
- **Kind**: account
- **Note**: For hosting the game online; offers free domain and multiple sites.

## Steps

### Set up Claude Code session
- **Timestamp**: [01:41](https://www.youtube.com/watch?v=HaEZgh2RadQ&t=101)
- **Action**: Create a new session in Claude Code and select a folder on your computer. Use Opus 3.5 with 'extra effort' enabled, or 'high' for good results.
- **Command Or Clicks**: Open Claude desktop app → New session → Select folder
- **Choice Branch**: Use 'high' effort if you prefer faster results.

### Develop plot, characters, and locations
- **Timestamp**: [02:40](https://www.youtube.com/watch?v=HaEZgh2RadQ&t=160)
- **Action**: Provide a general idea of your game (e.g., cozy horror) and let Claude develop the plot, characters, backstories, mechanics, scare moments, and ending. Claude saves this to the docs folder for future sessions.
- **Command Or Clicks**: Paste prompt: 'We want to make a cozy horror game...'
- **Choice Branch**: You can refine characters, backstories, and scare moments at this stage.

### Set up debugging tools
- **Timestamp**: [04:32](https://www.youtube.com/watch?v=HaEZgh2RadQ&t=272)
- **Action**: Ask Claude to create its own debugging tools so it can test specific scenes without playing the whole game. Ensure objects are aligned and not floating or clipping.
- **Command Or Clicks**: Prompt: 'Create debugging tools to inspect scenes and objects.'

### Create art style mockups
- **Timestamp**: [05:24](https://www.youtube.com/watch?v=HaEZgh2RadQ&t=324)
- **Action**: Ask Claude to generate three unique art style mockups. Review them, request variations, and choose one. Then have Claude turn it into a rulebook for appearance, colors, materials, lighting, animation, and menus.
- **Command Or Clicks**: Prompt: 'Create three different art style mockups.'
- **Choice Branch**: You can request a fourth style like 'grounded realism'.

### Integrate audio with 11 Labs
- **Timestamp**: [07:15](https://www.youtube.com/watch?v=HaEZgh2RadQ&t=435)
- **Action**: Optional: Use 11 Labs for voice acting, music, and sound effects. Create an API key, paste it into the .env file, and let Claude generate an audio page to review and adjust voices.
- **Command Or Clicks**: 11Labs.io → Developer → API keys → Create key → Copy → Paste into .env
- **Choice Branch**: If not using 11 Labs, ask Claude to generate sound effects locally.

### Create a vertical slice with critic agents
- **Timestamp**: [10:22](https://www.youtube.com/watch?v=HaEZgh2RadQ&t=622)
- **Action**: Ask Claude to build a short version of the game including characters, scares, and audio. Launch three critic agents: a harsh critic, a horror director, and a narrative agent to review and improve the slice.
- **Command Or Clicks**: Prompt: 'Create a vertical slice with critic agents.'
- **Choice Branch**: You can adjust the number of critic agents.

### Review and fix the vertical slice
- **Timestamp**: [12:03](https://www.youtube.com/watch?v=HaEZgh2RadQ&t=723)
- **Action**: Play the vertical slice several times, note any issues, and give feedback to Claude. Once satisfied, lock it in and ask Claude to create the rest of the game, allowing it to make small decisions autonomously.
- **Command Or Clicks**: Play the game → Note issues → Provide feedback to Claude
- **Choice Branch**: You can let Claude work for 12+ hours without waiting for your input.

### Final polishing
- **Timestamp**: [12:49](https://www.youtube.com/watch?v=HaEZgh2RadQ&t=769)
- **Action**: Play the game from start to finish and report any issues to Claude, such as lighting, missing voice lines, or wrong audio files. Optimize for different devices and get feedback from others.
- **Command Or Clicks**: Play the game → Report issues → Ask Claude to fix
- **Choice Branch**: Ask someone else to play and provide feedback.

### Deploy the game online with Hostinger
- **Timestamp**: [13:45](https://www.youtube.com/watch?v=HaEZgh2RadQ&t=825)
- **Action**: Sign up for Hostinger, choose a plan, and get a free domain. Use the Hostinger connector in Claude Code to deploy your game. Verify your account and get a working URL.
- **Command Or Clicks**: Hostinger → Choose plan → Get domain → Claude Code → Connectors → Hostinger → Add → Deploy
- **Choice Branch**: Use coupon 'LeonHosting' for 10% discount.

## Gotchas

### Don't use API tokens for this complex task; you need a Claude subscription. Even with a $20 plan, you'll hit limits—wait for reset.
- **Severity**: blocking
- **Timestamp**: [02:40](https://www.youtube.com/watch?v=HaEZgh2RadQ&t=160)

### Claude can't analyze the game at 60fps; it needs its own debugging tools to test specific scenes.
- **Severity**: heads_up
- **Timestamp**: [04:32](https://www.youtube.com/watch?v=HaEZgh2RadQ&t=272)

### If you don't like a voice or animation, ask Claude to change it; don't settle.
- **Severity**: heads_up
- **Timestamp**: [08:24](https://www.youtube.com/watch?v=HaEZgh2RadQ&t=504)

### The game must be optimized for different devices, especially laptops, since it runs in the browser.
- **Severity**: serious
- **Timestamp**: [12:49](https://www.youtube.com/watch?v=HaEZgh2RadQ&t=769)

## Where to go next

You can now create any game with Claude Code. Explore the free agent skill to automate the entire process. Try different genres and share your creations online.

## Concepts surfaced

[[claude-code]] · [[ai-game-development]] · [[voice-acting]] · [[hostinger-deployment]] · [[vertical-slice]] · [[critic-agents]]
