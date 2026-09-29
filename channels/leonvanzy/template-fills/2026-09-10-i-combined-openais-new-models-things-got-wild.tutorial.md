---
video_id: 2v6vgWOqYC0
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-09-10-i-combined-openais-new-models-things-got-wild.md
source_transcript: ../transcripts/2026-09-10-i-combined-openais-new-models-things-got-wild.md
source_summary_hash: sha256:3f78d7363c47127ade9e968209df6dba1525aeda5f499716748e12a4f9802822
source_transcript_hash: sha256:ae0f7523ccf7b87b75bced17f36f71029119e7b782174f54d50fdb8c892fe18c
fill_id: f702339b-8b1a-4193-8cf2-74eeac5aadd3
published_at: '2026-09-29T11:24:11.324001'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Combine GPT-6 Astra and Image 2.5 in ChatGPT Work mode to build parallax websites and playable 2D games.

## Prerequisites

### ChatGPT Desktop App
- **Kind**: tool
- **Note**: Required to access GPT-6 Astra in Work mode.

### GPT-6 Astra Model
- **Kind**: account
- **Note**: Select this model in Work mode settings.

## Steps

### Configure Work Mode
- **Timestamp**: [00:30](https://www.youtube.com/watch?v=2v6vgWOqYC0&t=30)
- **Action**: Switch to Work mode and select GPT-6 Astra with high reasoning effort.
- **Command Or Clicks**: Select 'Work' mode -> Model: 'GPT-6 Astra' -> Reasoning: 'High/Extra High'

### Generate Base Image
- **Timestamp**: [01:39](https://www.youtube.com/watch?v=2v6vgWOqYC0&t=99)
- **Action**: Prompt GPT-6 Astra to use Image 2.5 for a specific scene description.
- **Command Or Clicks**: Paste prompt describing scene layers and style (e.g., 'flat 2D illustrated style').

### Handle Transparency Bug
- **Timestamp**: [03:24](https://www.youtube.com/watch?v=2v6vgWOqYC0&t=204)
- **Action**: If Image 2.5 outputs a checkerboard background, switch to Code Interpreter.
- **Command Or Clicks**: Switch to 'Code Interpreter' -> Paste same prompt for transparent layers.

### Build Game Assets
- **Timestamp**: [05:50](https://www.youtube.com/watch?v=2v6vgWOqYC0&t=350)
- **Action**: Prompt GPT-6 Astra in Code Interpreter to generate sprite sheets and backgrounds.
- **Command Or Clicks**: Paste prompt: 'build a 2D sidescrolling clone... use GPT image 2.5 to generate all assets'.

## Gotchas

### Image 2.5 may output checkerboard backgrounds instead of transparency; switch to Code Interpreter to fix.
- **Severity**: blocking
- **Timestamp**: [03:24](https://www.youtube.com/watch?v=2v6vgWOqYC0&t=204)

## Where to go next

Join Agentic Labs for agentic coding masterclass and live streams on avoiding application breaks.

## Concepts surfaced

[[gpt-6-astra]] · [[image-2-5]] · [[parallax-websites]] · [[agentic-coding]] · [[code-interpreter]]
