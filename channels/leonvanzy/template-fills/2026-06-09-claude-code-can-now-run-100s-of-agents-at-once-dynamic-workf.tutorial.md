---
video_id: Aa_6bmzDc80
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-06-09-claude-code-can-now-run-100s-of-agents-at-once-dynamic-workf.md
source_transcript: ../transcripts/2026-06-09-claude-code-can-now-run-100s-of-agents-at-once-dynamic-workf.md
source_summary_hash: sha256:0ad509b7f3f36cf3d970e54f6afe65a4c651769e873659fa2b84b734c7ef418b
source_transcript_hash: sha256:7af3276631e25de174389c08ccf98d3fd745f360f1d37ca580357c7a90047aac
fill_id: 4d49fae7-631d-4215-952a-ea82c253936d
published_at: '2026-06-10T11:23:50.731738'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Use Claude Code's dynamic workflows to run hundreds of parallel agents for scalable, repeatable tasks like security audits.

## Prerequisites

### Claude Code
- **Kind**: tool
- **Note**: Access to Claude Code with dynamic workflows generally available.

### Basic Prompting Knowledge
- **Kind**: knowledge
- **Note**: Ability to write clear instructions for agents to follow.

## Steps

### Initiate a dynamic workflow
- **Timestamp**: [01:15](https://www.youtube.com/watch?v=Aa_6bmzDc80&t=75)
- **Action**: Start your prompt with 'ultra code' followed by 'use a workflow for the following' to explicitly trigger the dynamic workflow mode.
- **Command Or Clicks**: ultra code use a workflow for the following
- **Choice Branch**: Use for repetitive, large-scale tasks; avoid for simple single-session tasks to save costs.

### Define the task and scope
- **Timestamp**: [03:34](https://www.youtube.com/watch?v=Aa_6bmzDc80&t=214)
- **Action**: Describe the specific action to repeat at scale, such as auditing a project for security issues based on OWASP top 10 categories.
- **Command Or Clicks**: Audit our project for security issues based on the OWASP top 10
- **Choice Branch**: Ensure the task is repeatable and identical for each item to justify the workflow.

### Add safety and output instructions
- **Timestamp**: [04:20](https://www.youtube.com/watch?v=Aa_6bmzDc80&t=260)
- **Action**: Instruct the agent to start with a small batch for verification and specify the final output format, such as writing findings to markdown files.
- **Command Or Clicks**: Start with a small batch so that I can verify the workflow. write all findings to this folder and you know whatever file convention I want to use dot markdown
- **Choice Branch**: Avoid human-in-the-loop requirements; workflows run without stopping for permission.

### Monitor workflow progress
- **Timestamp**: [05:08](https://www.youtube.com/watch?v=Aa_6bmzDc80&t=308)
- **Action**: Use the down arrow to view the workflow steps and the right arrow to inspect specific agents or phases like recon, audit, verify, and report.
- **Command Or Clicks**: Down arrow, Enter, Right arrow, Enter
- **Choice Branch**: Check for file contention if multiple agents modify the same codebase.

### Save and reuse the workflow
- **Timestamp**: [06:48](https://www.youtube.com/watch?v=Aa_6bmzDc80&t=408)
- **Action**: Press slash, then 'run workflows', select the workflow, press 'S' to save it, and name it for future use in new sessions.
- **Command Or Clicks**: /run workflows S [Enter] OWASP audit
- **Choice Branch**: Saved workflows are sharable and can be invoked in new sessions by name.

## Gotchas

### Workflows are expensive because they kick off multiple sessions with their own context and tool calls, burning tokens quickly.
- **Severity**: serious
- **Timestamp**: [02:10](https://www.youtube.com/watch?v=Aa_6bmzDc80&t=130)

### Do not use workflows for simple tasks achievable in a single session; use them only for repetitive, large-scale tasks.
- **Severity**: blocking
- **Timestamp**: [02:10](https://www.youtube.com/watch?v=Aa_6bmzDc80&t=130)

### Dynamic workflows do not support human-in-the-loop interactions; they run without stopping to ask for permission.
- **Severity**: blocking
- **Timestamp**: [04:20](https://www.youtube.com/watch?v=Aa_6bmzDc80&t=260)

### Multiple agents modifying the same codebase can cause file contention; consider using different branches or work trees.
- **Severity**: serious
- **Timestamp**: [04:20](https://www.youtube.com/watch?v=Aa_6bmzDc80&t=260)

## Where to go next

Check the video description for the free 7-day builder challenge and the OWASP audit workflow file to start building with dynamic workflows today.

## Concepts surfaced

[[claude-code]] · [[dynamic-workflows]] · [[agentic-coding]] · [[security-auditing]] · [[automation]] · [[prompt-engineering]]
