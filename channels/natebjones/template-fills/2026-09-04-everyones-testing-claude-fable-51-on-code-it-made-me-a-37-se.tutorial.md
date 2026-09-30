---
video_id: 55rDzRkUVdE
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-09-04-everyones-testing-claude-fable-51-on-code-it-made-me-a-37-se.md
source_transcript: ../transcripts/2026-09-04-everyones-testing-claude-fable-51-on-code-it-made-me-a-37-se.md
source_summary_hash: sha256:65dfe06f3a5e27c7709f316c822a9d2c98b9ceb4c9f38ef2b51fc0fa52ed1f31
source_transcript_hash: sha256:c32b59e8a616542b79ec89ee5a755b2fe161ceb7e0b7ae11c3ddf73fc946f7de
fill_id: 5ce8397e-17d8-416c-854b-2fda41e638a2
published_at: '2026-09-30T13:58:22.180115'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Claude Fable 5.1 turns a single address into a 37-second Blender film and a full acquisition model, proving it's a knowledge-work powerhouse.

## Prerequisites

### Claude Fable 5.1 access
- **Kind**: account
- **Note**: Subscription or API access to Claude Fable 5.1, with effort settings (low/extra) available.

### Blender
- **Kind**: tool
- **Note**: Free, open-source 3D creation suite; used by the model to generate the architectural film.

### Excel
- **Kind**: tool
- **Note**: Spreadsheet software to open and review the generated financial workbooks.

### Basic knowledge of financial modeling
- **Kind**: knowledge
- **Note**: Understanding of DCF, WACC, and scenario analysis to evaluate the model's output.

## Steps

### Set up the knowledge work prompt
- **Timestamp**: [01:44](https://www.youtube.com/watch?v=55rDzRkUVdE&t=104)
- **Action**: Give Claude Fable 5.1 a real-world knowledge work task: research a company acquisition, build a post-acquisition DCF model in Excel, and create an executive deck. Use plain language, no special formatting.
- **Command Or Clicks**: Prompt: 'Research the GoPro acquisition by Starman. Build a post-acquisition discounted cash flow model only. Put it in Excel and turn it into a deck I can understand.'
- **Choice Branch**: Choose a company in the news; ensure it has missing financial data to test the model's handling of uncertainty.

### Run Fable 5.1 on low effort
- **Timestamp**: [02:35](https://www.youtube.com/watch?v=55rDzRkUVdE&t=155)
- **Action**: Select the 'low' effort setting to get a fast, cost-efficient first draft. Expect a complete but less rigorous output: a 7-sheet workbook and 13-slide deck with working formulas and meaningful scenarios.
- **Command Or Clicks**: In Claude, set effort to 'low' before sending the prompt.
- **Choice Branch**: Use low when you need a quick draft to iterate on, not a final deliverable.

### Review the low-effort output for gaps
- **Timestamp**: [05:01](https://www.youtube.com/watch?v=55rDzRkUVdE&t=301)
- **Action**: Open the generated Excel file and check for missing elements like a sources sheet or a checks sheet. The file is complete but lacks the extra verification layers that help analysts trust the numbers.
- **Command Or Clicks**: Open the workbook in Excel; look for tabs like 'Sources' or 'Checks'.
- **Choice Branch**: If you need full auditability, consider running at extra effort.

### Run Fable 5.1 on extra effort
- **Timestamp**: [06:05](https://www.youtube.com/watch?v=55rDzRkUVdE&t=365)
- **Action**: Switch to 'extra' effort for a more thorough analysis. Expect a 9-sheet workbook and 15-slide deck with separate business valuations, deal-close probability, WACC, exit multiple checks, and 26 linked sources.
- **Command Or Clicks**: In Claude, set effort to 'extra' and re-run the same prompt.
- **Choice Branch**: Use extra when you need deeper due diligence and are willing to spend more tokens.

### Compare with ChatGPT Soul
- **Timestamp**: [07:00](https://www.youtube.com/watch?v=55rDzRkUVdE&t=420)
- **Action**: Run the same prompt on ChatGPT Soul at extra high for comparison. Soul produces a compact 10-sheet workbook and 10-slide deck with a dedicated sources sheet and check sheet, making it easier to inspect.
- **Command Or Clicks**: Prompt ChatGPT Soul with the same acquisition task.
- **Choice Branch**: Use Soul when you need a clean, auditable starting point for another analyst.

### Test writing with a 100-word constraint
- **Timestamp**: [09:06](https://www.youtube.com/watch?v=55rDzRkUVdE&t=546)
- **Action**: Ask Fable 5.1, Fable 5, and GPT Soul to explain in 100 words how Toyota entered and won the US car market. Compare the choices each model makes in facts, causality, and style.
- **Command Or Clicks**: Prompt: 'Explain in 100 words how Toyota entered and won the car market in the United States.'
- **Choice Branch**: Use this test to see which model fits your audience: Soul for general, 5.1 for executive.

### Generate a Blender film from a property address
- **Timestamp**: [12:19](https://www.youtube.com/watch?v=55rDzRkUVdE&t=739)
- **Action**: Give Fable 5.1 a property listing and ask it to create a cinematic architectural walkthrough in Blender. The model builds the 3D model, plans camera angles, renders stills, inspects them, and edits until satisfied.
- **Command Or Clicks**: Prompt: 'Create a cinematic architectural walkthrough of this property in Blender.'
- **Choice Branch**: Use this for any visual concept that needs video communication, not just architecture.

### Review the film output
- **Timestamp**: [14:25](https://www.youtube.com/watch?v=55rDzRkUVdE&t=865)
- **Action**: Watch the generated 37-second film. Fable 5.1 produces the strongest, highest-quality sequence among the models tested, with stylized trees and simple glass as minor imperfections.
- **Command Or Clicks**: Play the rendered video file.
- **Choice Branch**: If you need a quick concept, Fable 5.1 is your choice; for polished edits, a human editor is still needed.

### Understand token efficiency and pricing
- **Timestamp**: [15:32](https://www.youtube.com/watch?v=55rDzRkUVdE&t=932)
- **Action**: Note that Fable 5.1 costs $10 per million input tokens and $50 per million output tokens on API billing, with cache reads dropped to $0.25 per million. Anthropic estimates typical workloads cost ~25% less than Fable 5, and highly agentic work ~45% less.
- **Command Or Clicks**: Check API pricing on Anthropic's site.
- **Choice Branch**: Use low effort to stretch subscription limits further.

## Gotchas

### Low-effort output lacks a sources sheet and checks sheet, making it harder to verify assumptions and formula correctness.
- **Severity**: serious
- **Timestamp**: [05:01](https://www.youtube.com/watch?v=55rDzRkUVdE&t=301)

### Fable 5.1 still has tighter usage limits than OpenAI's models; token efficiency doesn't mean unlimited.
- **Severity**: heads_up
- **Timestamp**: [16:30](https://www.youtube.com/watch?v=55rDzRkUVdE&t=990)

### The film's trees are stylized and glass is simple; don't expect production-ready quality for client work.
- **Severity**: heads_up
- **Timestamp**: [14:25](https://www.youtube.com/watch?v=55rDzRkUVdE&t=865)

## Where to go next

Next video: Fable 5.1 vs Astra. I'll dive into Astra's release, its strategic angle for OpenAI, and how I'd use each model. Tell me in the comments what you want tested.

## Concepts surfaced

[[knowledge-work]] · [[token-efficiency]] · [[effort-settings]] · [[blender]] · [[financial-modeling]] · [[writing-quality]]
