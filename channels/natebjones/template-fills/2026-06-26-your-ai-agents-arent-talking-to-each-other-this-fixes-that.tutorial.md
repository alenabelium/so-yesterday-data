---
video_id: QSK4vf_ZTRA
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-06-26-your-ai-agents-arent-talking-to-each-other-this-fixes-that.md
source_transcript: ../transcripts/2026-06-26-your-ai-agents-arent-talking-to-each-other-this-fixes-that.md
source_summary_hash: sha256:195bf8bfa76f058194b641e6dc0ff387419c307758af6ceb7f1464b84ce01b3e
source_transcript_hash: sha256:6f7ee56d23354563ad71ed8958e7ea9702b1e6531b7fc3eadfc355745d6c1f1d
fill_id: 2135c7d7-777b-4615-b0ab-e73b2d8484bf
published_at: '2026-09-29T11:06:09.023536'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Use a shared ticketing queue like Linear to let AI agents coordinate work without manual handoffs.

## Prerequisites

### Linear or Jira
- **Kind**: tool
- **Note**: A ticketing queue that agents can write to and humans can read.

### OpenClaw or Hermes
- **Kind**: tool
- **Note**: Agent frameworks to point at the Open Engine skills.

### Open Engine Skills
- **Kind**: tool
- **Note**: Setup, status, run, and smoke test skills for the queue.

## Steps

### Set up the shared queue
- **Timestamp**: [06:17](https://www.youtube.com/watch?v=QSK4vf_ZTRA&t=377)
- **Action**: Choose a ticketing system like Linear or Jira that both humans and agents can access to serve as the common state layer.
- **Command Or Clicks**: N/A
- **Choice Branch**: Use Linear's free plan or your existing Jira instance.

### Install Open Engine skills
- **Timestamp**: [09:36](https://www.youtube.com/watch?v=QSK4vf_ZTRA&t=576)
- **Action**: Point your agent framework (e.g., OpenClaw) to the Open Engine skills which define the protocol for using the ticketing system.
- **Command Or Clicks**: N/A
- **Choice Branch**: Install setup, status, run, and smoke test skills.

### Run the smoke test
- **Timestamp**: [13:35](https://www.youtube.com/watch?v=QSK4vf_ZTRA&t=815)
- **Action**: Execute the smoke test to verify the agent interaction loop works by creating a simple issue and moving it through the statuses.
- **Command Or Clicks**: Create an issue called 'say hello' from the queue
- **Choice Branch**: Assign to human or agent, label as agent instructions, and move to done.

### Delegate tasks via tickets
- **Timestamp**: [13:35](https://www.youtube.com/watch?v=QSK4vf_ZTRA&t=815)
- **Action**: Write a self-contained Linear issue with context, assign it to the target agent, and label it as agent instructions.
- **Command Or Clicks**: N/A
- **Choice Branch**: The target agent picks it up on its heartbeat and claims the issue.

### Manage handoffs and receipts
- **Timestamp**: [16:34](https://www.youtube.com/watch?v=QSK4vf_ZTRA&t=994)
- **Action**: Ensure agents move issues through statuses (agent to-do -> agent working -> agent done) and leave receipts explaining what was done.
- **Command Or Clicks**: N/A
- **Choice Branch**: If ambiguous, move to 'needs input' and ask the human for clarification.

## Gotchas

### Chat logs and Slack are terrible for state management; work must leave the chat to be auditable.
- **Severity**: blocking
- **Timestamp**: [07:55](https://www.youtube.com/watch?v=QSK4vf_ZTRA&t=475)

### Agents start from zero without a true memory system that lives between them.
- **Severity**: serious
- **Timestamp**: [05:23](https://www.youtube.com/watch?v=QSK4vf_ZTRA&t=323)

### Do not rely on unpredictable memory in tools like OpenClaw for long-term multi-role tasks.
- **Severity**: serious
- **Timestamp**: [03:14](https://www.youtube.com/watch?v=QSK4vf_ZTRA&t=194)

## Where to go next

Join the Substack community and active Slack to get the full Open Engine guide and share your use cases.

## Concepts surfaced

[[ai-agent-coordination]] · [[ticketing-queue-state]] · [[open-engine-framework]] · [[agent-handoffs]] · [[linear-integration]]
