---
video_id: Y8vAQ1FgNbM
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-07-29-dont-let-claude-token-limits-hold-you-back-heres-how.md
source_transcript: ../transcripts/2026-07-29-dont-let-claude-token-limits-hold-you-back-heres-how.md
source_summary_hash: sha256:81a19b9ce7bc0b8c92014a2f26b00779343ccc7e6cd5a14ef7e95f0fb5b0dc4a
source_transcript_hash: sha256:d3637174250280dc05982ac2f7b487e5cf008678028ae7713d6583a61579bfb1
fill_id: e0adb14f-5833-4d66-bfc3-c47eed9273b6
published_at: '2026-09-29T11:21:29.191963'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Master 15 rules to manage AI context windows, install a 'Token Saver' skill, and use the Ringer multi-agent framework to eliminate wasted tokens.

## Prerequisites

### Claude/Codex Account
- **Kind**: account
- **Note**: Access to Claude, Codex, ChatGPT, or Kimmy to apply token-saving habits.

### OpenBrain Database
- **Kind**: tool
- **Note**: Optional external database for storing and retrieving answers to avoid recalculation.

## Steps

### Understand Reused Input
- **Timestamp**: [01:05](https://www.youtube.com/watch?v=Y8vAQ1FgNbM&t=65)
- **Action**: Recognize that 96% of tokens are reused conversation history, not new input. The model wraps the entire chat history with each new message.
- **Command Or Clicks**: None
- **Choice Branch**: None

### Edit Mistakes Instantly
- **Timestamp**: [04:07](https://www.youtube.com/watch?v=Y8vAQ1FgNbM&t=247)
- **Action**: Use the edit button to correct typos or unclear requests immediately. Do not start a new chat to say 'that was wrong,' as that adds more reused input.
- **Command Or Clicks**: Click edit button
- **Choice Branch**: None

### Group Related Questions
- **Timestamp**: [04:54](https://www.youtube.com/watch?v=Y8vAQ1FgNbM&t=294)
- **Action**: Combine multiple questions from the same source into one query. Specify the desired output format (e.g., bullets, 150 words) to reduce ambiguity.
- **Command Or Clicks**: None
- **Choice Branch**: None

### Start Clean Tasks
- **Timestamp**: [05:52](https://www.youtube.com/watch?v=Y8vAQ1FgNbM&t=352)
- **Action**: Start a new thread when the job changes. Long conversations carry massive amounts of reused tokens, hitting limits faster.
- **Command Or Clicks**: Start new thread
- **Choice Branch**: None

### Carry Only the Answer
- **Timestamp**: [06:57](https://www.youtube.com/watch?v=Y8vAQ1FgNbM&t=417)
- **Action**: When moving between stages (e.g., research to writing), copy only the final artifact. Do not paste the entire research history or rejected drafts.
- **Command Or Clicks**: Copy final artifact
- **Choice Branch**: None

### Request Precise Output
- **Timestamp**: [07:58](https://www.youtube.com/watch?v=Y8vAQ1FgNbM&t=478)
- **Action**: Ask for exactly what you need (e.g., 50 words, JSON, 5 bullets). Concise output saves tokens on the current turn and all future turns where it becomes input.
- **Command Or Clicks**: Specify length/format
- **Choice Branch**: None

### Search Files Manually
- **Timestamp**: [09:05](https://www.youtube.com/watch?v=Y8vAQ1FgNbM&t=545)
- **Action**: Search files yourself and paste only the relevant snippets. Letting the model search the entire file burns significant tokens.
- **Command Or Clicks**: Search file, paste snippet
- **Choice Branch**: None

### Convert Sources to Text
- **Timestamp**: [09:05](https://www.youtube.com/watch?v=Y8vAQ1FgNbM&t=545)
- **Action**: Convert PDFs or screenshots to plain text or markdown before pasting. Layout data wastes tokens if only the words matter.
- **Command Or Clicks**: Convert PDF to text
- **Choice Branch**: None

### Store Answers in Database
- **Timestamp**: [11:02](https://www.youtube.com/watch?v=Y8vAQ1FgNbM&t=662)
- **Action**: Save accepted answers in a searchable database like OpenBrain. This allows the AI to retrieve data instead of recalculating it.
- **Command Or Clicks**: Save to OpenBrain
- **Choice Branch**: None

### Install Token Saver Skill
- **Timestamp**: [11:02](https://www.youtube.com/watch?v=Y8vAQ1FgNbM&t=662)
- **Action**: Install the 'Token Saver' skill in Claude Code or Codex. It automates searching, snippet selection, and length constraints.
- **Command Or Clicks**: Install token saver skill
- **Choice Branch**: None

### Load Only Necessary Tools
- **Timestamp**: [12:20](https://www.youtube.com/watch?v=Y8vAQ1FgNbM&t=740)
- **Action**: Be aware that tool definitions burn tokens. Use context editing or compaction features to clear old tool results and thinking blocks.
- **Command Or Clicks**: Enable context editing
- **Choice Branch**: None

### Use Smaller Models
- **Timestamp**: [14:12](https://www.youtube.com/watch?v=Y8vAQ1FgNbM&t=852)
- **Action**: Use the 'dumbest' model that can complete the task. The Token Saver skill can help approximate which model is most token-efficient.
- **Command Or Clicks**: Select smaller model
- **Choice Branch**: None

### Implement Ringer Framework
- **Timestamp**: [16:20](https://www.youtube.com/watch?v=Y8vAQ1FgNbM&t=980)
- **Action**: Deploy Ringer, a local multi-agent framework that intercepts requests before they hit the provider. It can return cached answers, enforce hard limits, and optimize payloads.
- **Command Or Clicks**: Deploy Ringer locally
- **Choice Branch**: None

### Enforce Hard Limits
- **Timestamp**: [18:30](https://www.youtube.com/watch?v=Y8vAQ1FgNbM&t=1110)
- **Action**: Use Ringer to enforce strict size limits on input and output packets, preventing massive token waste on any single call.
- **Command Or Clicks**: Set hard limits in Ringer
- **Choice Branch**: None

## Gotchas

### Reused input compounds rapidly; by message 30, your new text is a rounding error. Labs won't fix this; you must manage it.
- **Severity**: serious
- **Timestamp**: [01:05](https://www.youtube.com/watch?v=Y8vAQ1FgNbM&t=65)

### Tool definitions burn ~55,000 tokens before the model acts. Don't connect unnecessary tools.
- **Severity**: serious
- **Timestamp**: [12:20](https://www.youtube.com/watch?v=Y8vAQ1FgNbM&t=740)

### Skills cannot make the call they are inside of. They work on future requests, not the current one already sent.
- **Severity**: blocking
- **Timestamp**: [16:20](https://www.youtube.com/watch?v=Y8vAQ1FgNbM&t=980)

## Where to go next

The 15 rules and Token Saver skill are on Substack. Watch the dedicated Ringer intro video for advanced local interception setup.

## Concepts surfaced

[[token-efficiency]] · [[context-window-management]] · [[multi-agent-frameworks]] · [[prompt-caching]] · [[ai-best-practices]]
