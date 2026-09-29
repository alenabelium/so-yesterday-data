---
video_id: rqVzTX8w_w0
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-05-30-the-ai-workflow-shift-nobody-is-talking-about.md
source_transcript: ../transcripts/2026-05-30-the-ai-workflow-shift-nobody-is-talking-about.md
source_summary_hash: sha256:d57983db5d09a9820743436fdf624cfe4e978e6eff82e5c45c9ed1ef4e737780
source_transcript_hash: sha256:3be263f73816d460f543e604138dcb73d49976f5dbb0897c8f2a9de55c791847
fill_id: f39c382b-7550-4b8c-b39d-57ffff327885
published_at: '2026-05-31T15:06:47.328549'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

By the end you'll know how to assemble a clean local context window in Codex and shift from rigid prompts to collaborative task definition for long, complex work.

## Prerequisites

### Codex
- **Kind**: tool
- **Note**: The host stresses this workflow works in Codex specifically, not Claude Code or Claude co-work.

### Local file system access
- **Kind**: hardware
- **Note**: Codex reads and copies files from folders on your own machine.

## Steps

### Ask Codex to find files by natural-language description
- **Timestamp**: [00:00](https://www.youtube.com/watch?v=rqVzTX8w_w0&t=0)
- **Action**: Tell Codex to look across your whole local file system and locate files by describing what they're about and roughly when you made them, rather than naming the title or subtitle exactly.
- **Command Or Clicks**: Describe the file: 'This is what it's about, this is about when I made it, can you please find it?'
- **Choice Branch**: Describe content and date, not exact filenames.

### Let Codex copy the files into a clean working folder
- **Timestamp**: [00:00](https://www.youtube.com/watch?v=rqVzTX8w_w0&t=0)
- **Action**: Have Codex make copies of the found files into a single neat working folder, assembling a clean, efficient context window on your local machine for the task.
- **Command Or Clicks**: Codex pulls the matched files in as copies into one tidy working folder.

### Open a new chat and point Codex at the folder
- **Timestamp**: [00:00](https://www.youtube.com/watch?v=rqVzTX8w_w0&t=0)
- **Action**: Open a new chat in Codex, tell it you have a clean context window, point it at that particular folder, and give it the task. If you have detailed instructions, copy them into the folder as a transcript that is part of the task.
- **Command Or Clicks**: 'We've got a really clean context window here. Look at this folder and here is your task.'
- **Choice Branch**: Add detailed instructions as a file in the folder when the task needs them.

### Shift prompting from instructions to defining standards
- **Timestamp**: [02:05](https://www.youtube.com/watch?v=rqVzTX8w_w0&t=125)
- **Action**: Instead of structuring a rigid prompt, give the model the meaningful questions that circle the standards you want to meet, share the relevant files, and ask it to help define the shape of the task first.
- **Command Or Clicks**: 'Here are files I think are relevant. Help me define the shape of this task first.'
- **Choice Branch**: Stay in the messy collaborative stage before executing.

### Tell Codex to execute the task agentically
- **Timestamp**: [02:05](https://www.youtube.com/watch?v=rqVzTX8w_w0&t=125)
- **Action**: Once you've defined the shape of the task together, switch gears and tell the model to go execute it agentically; the host finds the model doesn't get lost when you say 'now go do it.'
- **Command Or Clicks**: 'Now go do it. Now go get it done.'

### Scale up with multi-threading and parallel drafting
- **Timestamp**: [04:16](https://www.youtube.com/watch?v=rqVzTX8w_w0&t=256)
- **Action**: Use the clean local folders, long-running agent, and the auto-review system to multi-thread: do simultaneous drafting, or develop a series of eight or nine prompts to run sequentially, incubating multiple ideas at once.
- **Command Or Clicks**: Let the agent run on your computer while auto-review puts guardrails around it.

## Gotchas

### This workflow is specific to Codex. The host tried the same workflow with Claude Code and Claude co-work and it does not work.
- **Severity**: blocking
- **Timestamp**: [00:00](https://www.youtube.com/watch?v=rqVzTX8w_w0&t=0)

### Don't lean on pre-2025 prompt-engineering structure for this; that still helps for one-off prompts, but here you define standards and let the model help shape the task.
- **Severity**: heads_up
- **Timestamp**: [02:05](https://www.youtube.com/watch?v=rqVzTX8w_w0&t=125)

## Where to go next

This is the first of a weekly series on how the host is using AI; expect future entries as models shift. Try the local-folder context-window approach on a long document or coding project and lean on the auto-review guardrails when running agents on your machine.

## Concepts surfaced

[[context-window-assembly]] · [[agentic-workflow]] · [[prompt-engineering]] · [[multi-threading]]
