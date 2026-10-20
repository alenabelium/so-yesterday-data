---
video_id: KX0GurmgAoo
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-02-05-90-of-ai-users-are-getting-mediocre-output-dont-be-one-of-th.md
source_transcript: ../transcripts/2026-02-05-90-of-ai-users-are-getting-mediocre-output-dont-be-one-of-th.md
source_summary_hash: sha256:06ba4552b77f66699f84e5522bae7f93753c3628c28d72a90dee6360423c8673
source_transcript_hash: sha256:00204228440387212b531a4f4fccaf2a70a3a3dc1aa7f656a9dab1e706a5b572
fill_id: ea13b377-ed03-442a-b17e-321d8e1ca514
published_at: '2026-10-20T01:21:44.531857'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Learn the four levers beyond prompting—memory, instructions, tools, and style—to escape AI's median output and get personalized results.

## Prerequisites

### An AI assistant account
- **Kind**: account
- **Note**: Access to ChatGPT, Claude, or Gemini with settings for memory, instructions, and tools.

## Steps

### Understand the averaging problem
- **Timestamp**: [00:00](https://www.youtube.com/watch?v=KX0GurmgAoo&t=0)
- **Action**: Learn why AI outputs feel generic: models are trained via RLHF to satisfy the median user, not you specifically. Recognize that default settings produce average results.

### Lever 1: Configure memory in ChatGPT
- **Timestamp**: [04:33](https://www.youtube.com/watch?v=KX0GurmgAoo&t=273)
- **Action**: Use ChatGPT's memory features: saved memories for explicit facts, chat history references, and project-scoped memory. Tell ChatGPT to remember specific preferences for reliable personalization.
- **Command Or Clicks**: Say: 'Remember that I prefer one-sentence answers to factual questions.'

### Lever 1: Configure memory in Claude
- **Timestamp**: [06:20](https://www.youtube.com/watch?v=KX0GurmgAoo&t=380)
- **Action**: Claude uses project-scoped memory with search and summaries. Create separate projects for distinct contexts to keep memory clean. Use memory import/export for interoperability.
- **Command Or Clicks**: Create a project for client engagement to isolate memory.

### Lever 1: Configure memory in Gemini
- **Timestamp**: [07:35](https://www.youtube.com/watch?v=KX0GurmgAoo&t=455)
- **Action**: Gemini's personal intelligence connects to Google apps like Gmail and YouTube. Decide which apps to connect in Settings > Personalization to balance personalization with privacy.
- **Command Or Clicks**: Settings > Personalization > Connect or disconnect Google apps.

### Lever 2: Set up instructions in ChatGPT
- **Timestamp**: [08:30](https://www.youtube.com/watch?v=KX0GurmgAoo&t=510)
- **Action**: Use custom instructions, project workspaces, and custom GPTs. Be specific: instead of 'be concise', say 'For factual questions, answer in a sentence; for analysis, walk through reasoning step by step.'
- **Command Or Clicks**: Custom Instructions > Add specific behavioral rules.

### Lever 2: Set up instructions in Claude
- **Timestamp**: [09:13](https://www.youtube.com/watch?v=KX0GurmgAoo&t=553)
- **Action**: Claude has profile preferences, project instructions, and styles. Use the custom style feature to upload samples of your best writing for Claude to match your voice. For developers, maintain a CLAUDE.md file.
- **Command Or Clicks**: Upload writing samples to generate a style profile.

### Lever 3: Connect apps and tools
- **Timestamp**: [10:26](https://www.youtube.com/watch?v=KX0GurmgAoo&t=626)
- **Action**: Enable tools like web search, code execution, and MCP servers. ChatGPT connects to apps like Gmail; Claude supports many MCP servers; Gemini is limited. Choose tools that steer inputs to your real files and workflows.
- **Command Or Clicks**: Enable MCP servers or connect apps in settings.

### Lever 4: Adjust style and tone
- **Timestamp**: [13:20](https://www.youtube.com/watch?v=KX0GurmgAoo&t=800)
- **Action**: Use style presets and custom styles. ChatGPT has eight personalities and granular controls; Claude has formal, concise, explanatory, and custom styles. Pick a style that matches your actual usage, not aspirational.
- **Command Or Clicks**: Select a personality or upload a style sample.

### Capture corrections and encode them
- **Timestamp**: [14:46](https://www.youtube.com/watch?v=KX0GurmgAoo&t=886)
- **Action**: When AI output isn't right, write down the correction. Add it to instructions, memory, or style settings. This compounding effect separates 10x users from mediocre ones.
- **Command Or Clicks**: Keep a notes file or update CLAUDE.md with rules.

## Gotchas

### Be concise is too vague to steer the model; it doesn't change output shape.
- **Severity**: serious
- **Timestamp**: [14:46](https://www.youtube.com/watch?v=KX0GurmgAoo&t=886)

### Conflicting instructions (e.g., verbose in instructions, concise in personality) waste tokens and confuse the model.
- **Severity**: serious
- **Timestamp**: [13:20](https://www.youtube.com/watch?v=KX0GurmgAoo&t=800)

### Steering doesn't fix hallucinations or creative gravity; it only addresses personalization.
- **Severity**: heads_up
- **Timestamp**: [16:56](https://www.youtube.com/watch?v=KX0GurmgAoo&t=1016)

### If you use AI only occasionally, investing in levers may not be worth the effort.
- **Severity**: heads_up
- **Timestamp**: [16:56](https://www.youtube.com/watch?v=KX0GurmgAoo&t=1016)

## Where to go next

Start with one task where your AI output feels off. Over the next few sessions, note your corrections and add them to your instructions. Iterate to compound personalization.

## Concepts surfaced

[[reinforcement-learning-from-human-feedback]] · [[model-context-protocol]] · [[custom-instructions]] · [[memory-management]] · [[style-controls]]
