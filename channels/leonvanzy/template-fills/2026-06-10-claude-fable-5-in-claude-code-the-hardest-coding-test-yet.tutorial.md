---
video_id: I3PYGi_tGy0
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-06-10-claude-fable-5-in-claude-code-the-hardest-coding-test-yet.md
source_transcript: ../transcripts/2026-06-10-claude-fable-5-in-claude-code-the-hardest-coding-test-yet.md
source_summary_hash: sha256:f23aca1eed3542567878061c6315e43f8191e955b9d7ea85b3fee26b23750881
source_transcript_hash: sha256:a1e5de0c4b60c22c26ae0f09eb1b0982dabc08e8f31abe51fde87f801683fc27
fill_id: 8a36d036-19ef-4bef-9009-546ffa701c2c
published_at: '2026-06-11T15:54:11.107405'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Claude Code with Fable 5 builds a complex ray-tracing game engine in 2 hours, outperforming GPT-5.5 in visual fidelity.

## Prerequisites

### Claude Code
- **Kind**: tool
- **Note**: Must be updated to the latest version to access the Fable 5 model.

### Fable 5 Model
- **Kind**: account
- **Note**: Select Fable in the model selector; it is not the default model.

### Ramp Framework
- **Kind**: tool
- **Note**: Optional development framework for agentic coding workflows.

## Steps

### Update Claude Code and Select Fable 5
- **Timestamp**: [01:09](https://www.youtube.com/watch?v=I3PYGi_tGy0&t=69)
- **Action**: Update Claude Code to the latest version. Open the model selector and choose Fable 5, as it is not the default model.
- **Command Or Clicks**: Update Claude Code. Open model selector. Select Fable.
- **Choice Branch**: Ensure Fable is selected instead of the default Opus 4.8.

### Set Reasoning Effort to Extra High
- **Timestamp**: [01:45](https://www.youtube.com/watch?v=I3PYGi_tGy0&t=105)
- **Action**: Run the effort command to set reasoning to 'extra high' for complex tasks. Avoid 'maxlevel' to prevent diminishing returns and hallucinations.
- **Command Or Clicks**: /effort extra high
- **Choice Branch**: Use 'extra high' for complex tasks; avoid 'maxlevel'.

### Generate Implementation Plan
- **Timestamp**: [02:30](https://www.youtube.com/watch?v=I3PYGi_tGy0&t=150)
- **Action**: Enter planning mode. Paste the detailed prompt asking for a game engine with ray tracing. Ask the agent to grill you on requirements.
- **Command Or Clicks**: Paste prompt. Ask agent to grill on design.
- **Choice Branch**: Answer clarifying questions or let the agent decide.

### Break Plan into Feature Files
- **Timestamp**: [03:22](https://www.youtube.com/watch?v=I3PYGi_tGy0&t=202)
- **Action**: Exit planning mode into edit mode. Paste a prompt to break the implementation plan into separate feature files for autopilot implementation.
- **Command Or Clicks**: Paste prompt to split plan into feature files.
- **Choice Branch**: Must be in edit mode to paste the prompt.

### Initiate Autopilot Implementation
- **Timestamp**: [04:49](https://www.youtube.com/watch?v=I3PYGi_tGy0&t=289)
- **Action**: Create a new repository. Exit Claude Code. Start in Yolo mode. Run the goal command with the plan folder, instructing it to implement features and use Opus for background reviews.
- **Command Or Clicks**: Run goal command. Pull in plan folder. Use Opus for review.
- **Choice Branch**: Use Opus for review agents to save costs.

### Review Results and Compare to GPT-5.5
- **Timestamp**: [08:16](https://www.youtube.com/watch?v=I3PYGi_tGy0&t=496)
- **Action**: Wait for the ~2 hour implementation. Run the generated game. Compare the ray tracing and reflections against GPT-5.5's output.
- **Command Or Clicks**: Run the generated command. Play the game.

## Gotchas

### Fable 5 is expensive: $10 per 1M input tokens and $50 per 1M output tokens. It is double the cost of Opus 4.8.
- **Severity**: serious
- **Timestamp**: [02:45](https://www.youtube.com/watch?v=I3PYGi_tGy0&t=165)

### Using 'maxlevel' for reasoning effort may cause diminishing returns and hallucinations where the model gaslights itself.
- **Severity**: blocking
- **Timestamp**: [01:55](https://www.youtube.com/watch?v=I3PYGi_tGy0&t=115)

### The implementation took nearly 2 hours and burned ~1/2 million tokens. Background agents may not be included in the total count.
- **Severity**: heads_up
- **Timestamp**: [08:25](https://www.youtube.com/watch?v=I3PYGi_tGy0&t=505)

## Where to go next

Try the free Ramp framework course or test the generated game online. Compare Fable 5's ray tracing capabilities with other models in future agentic coding challenges.

## Concepts surfaced

[[agentic-coding]] · [[ray-tracing]] · [[claude-code]] · [[fable-5]] · [[cost-management]]
