---
video_id: ix8SsXjBc7M
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-09-07-there-are-jobs-you-could-never-give-ai-i-gave-gpt-6-astra-20.md
source_transcript: ../transcripts/2026-09-07-there-are-jobs-you-could-never-give-ai-i-gave-gpt-6-astra-20.md
source_summary_hash: sha256:ecd2ce4fa19ab477a72a847a5f7924faa6f8d028a5aee0f1191fedc9c3e0f75a
source_transcript_hash: sha256:f0302ba4680de3aa631974e092fc5e5af8fb418fdaa4f1b450f87156a86c5923
fill_id: c78f1ec6-173a-4310-89d5-ee72333cfa2b
published_at: '2026-09-29T11:23:58.273999'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Use GPT-6 Astra's manager loop and recipe cards to automate complex, multi-step admin tasks like household moves while retaining human oversight for critical decisions.

## Prerequisites

### GPT-6 Astra Access
- **Kind**: account
- **Note**: Access to the GPT-6 model (code-named Astra) capable of autonomous execution and multi-agent supervision.

### Manager Loop Knowledge
- **Kind**: knowledge
- **Note**: Understanding that you delegate high-level goals to a supervisor agent rather than micromanaging sub-tasks.

## Steps

### Define the High-Level Goal
- **Timestamp**: [09:18](https://www.youtube.com/watch?v=ix8SsXjBc7M&t=558)
- **Action**: Start by giving a single, high-level instruction to the Astra manager agent, such as moving your household to a new city by a specific date.
- **Command Or Clicks**: "I need to move my household to Seattle by June 1st."

### Answer Manager Interview Questions
- **Timestamp**: [11:38](https://www.youtube.com/watch?v=ix8SsXjBc7M&t=698)
- **Action**: Allow the manager agent to interview you for necessary details like budget, family size, neighborhood criteria, and existing accounts.
- **Command Or Clicks**: Answer questions about who is moving, budget, home type, schools, doctors, vehicles, and pets.

### Deploy Recipe Card Prompt
- **Timestamp**: [22:24](https://www.youtube.com/watch?v=ix8SsXjBc7M&t=1344)
- **Action**: Use a structured 'recipe card' prompt to define task boundaries, approval points, and information needs for the agent.
- **Command Or Clicks**: "I need to move my household to X city by Y date... Please start this task by showing me which parts of the move you can handle completely. Ask me about who's moving, about the budget... You are the central point of contact for this task."

### Delegate Execution to Sub-Agents
- **Timestamp**: [12:41](https://www.youtube.com/watch?v=ix8SsXjBc7M&t=761)
- **Action**: Let the manager agent delegate specific research, comparison, and form-prep tasks to execution agents while you wait for choices.
- **Command Or Clicks**: Allow Astra to manage work across housing, schools, DMV, and utilities without step-by-step oversight.

### Review Critical Decisions
- **Timestamp**: [18:08](https://www.youtube.com/watch?v=ix8SsXjBc7M&t=1088)
- **Action**: Retain control over final choices like selecting a house or doctor, while the agent handles the grunt work of gathering options.
- **Command Or Clicks**: Approve or reject the options presented by the agent for irreversible decisions.

## Gotchas

### Do not give Astra your credit card to autonomously move your family while you sleep; human oversight is required for trust and safety.
- **Severity**: blocking
- **Timestamp**: [02:06](https://www.youtube.com/watch?v=ix8SsXjBc7M&t=126)

### Avoid trying to define the entire complex job in a single prompt; use recipe cards to break down tasks that are too large for one instruction.
- **Severity**: serious
- **Timestamp**: [19:26](https://www.youtube.com/watch?v=ix8SsXjBc7M&t=1166)

## Where to go next

Access the paid Substack guide containing 23 complete, long-form recipe cards for specific admin tasks to apply this manager loop technique in your business or home.

## Concepts surfaced

[[manager-loop]] · [[recipe-cards]] · [[autonomous-agents]] · [[human-in-the-loop]] · [[gpt-6-astra]]
