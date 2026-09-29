---
video_id: 2omtxQ0dSFk
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-05-28-this-claude-code-alternative-is-10x-cheaper.md
source_transcript: ../transcripts/2026-05-28-this-claude-code-alternative-is-10x-cheaper.md
source_summary_hash: sha256:b57c6bdcabcb70d50e1b9f85e75ecb09d3bbe4e922183058cb9a2ae578fd4ca1
source_transcript_hash: sha256:c20c9aa0a802bc1d816058a8164f9b0ba1ef0b36e66b61a1b7e7ee2ab249863c
fill_id: b2cf515c-c658-41d8-b058-28673c5a8abf
published_at: '2026-05-31T15:05:17.103407'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

By the end, you will have a feature-complete Reddit clone built inside Claude Code, powered by the cheaper open-weight Minimax M2.7 model instead of premium Claude models.

## Prerequisites

### Minimax account
- **Kind**: account
- **Note**: Sign up at minimax.io, open the API platform, and choose a token plan (starter, plus, or max) to get an API key.

### Claude Code
- **Kind**: tool
- **Note**: The host drives everything through Claude Code, simply pointing it at the Minimax endpoint instead of Anthropic's.

## Steps

### Configure settings.json for Minimax
- **Timestamp**: [00:46](https://www.youtube.com/watch?v=2omtxQ0dSFk&t=46)
- **Action**: In a blank project's Claude folder, create a settings.json and add the configuration that points the Anthropic base URL to the Minimax Anthropic endpoint, authenticates with your Minimax API key, and disables Claude Code sending usage logs to Anthropic.
- **Command Or Clicks**: Create .claude/settings.json; you can download the full config from the GitHub repo linked in the description.
- **Choice Branch**: Most users pick the standard Minimax M2.7 plan; power users can choose the high-speed plan.

### Get and paste your Minimax API key
- **Timestamp**: [00:46](https://www.youtube.com/watch?v=2omtxQ0dSFk&t=46)
- **Action**: Go to minimax.io, log in, open the API platform and the token plan page, click manage plan, and pick a plan. Pricing is per request every 5 hours (the plus plan gives 4,500 requests), not per token, so detailed prompts give massive headroom.
- **Command Or Clicks**: Scroll to API key on the token plan page, copy the key, and add it to settings.json.
- **Choice Branch**: Choose starter, plus, or max; the token plan also unlocks image, video, and speech models.

### Plan the app in planning mode
- **Timestamp**: [02:26](https://www.youtube.com/watch?v=2omtxQ0dSFk&t=146)
- **Action**: Open Claude Code, enter planning mode, and paste a prompt describing the tech stack and the Reddit clone's core features, then send it. Minimax generates the plan in under two minutes.
- **Command Or Clicks**: Enter planning mode and send the prompt; copy the prompts free from the link in the description.
- **Choice Branch**: Exit planning mode, switch to change mode, and ask it to store the plan in the plans folder.

### Scaffold the stack and install skills
- **Timestamp**: [03:25](https://www.youtube.com/watch?v=2omtxQ0dSFk&t=205)
- **Action**: In agent view, pull in the plan and ask the agent to set up only the tech stack. While it scaffolds Next.js, have the agent install the front-end design skill and the agent browser skill at project level, then start the dev server on port 3000.
- **Command Or Clicks**: Ask the agent to set up the following skills, select Claude Code, install at project level; then start the dev server on port 3000.
- **Choice Branch**: Install the front-end design skill for styling and the agent browser skill for automated testing.

### Run the goal command to build the app
- **Timestamp**: [05:06](https://www.youtube.com/watch?v=2omtxQ0dSFk&t=306)
- **Action**: Run the goal command so the agent loops until everything is implemented and tested. Pull in the plan and prompt it to use the browser skill in headed mode to test changes and the front-end design skill to build the design, storing the design system in design.md.
- **Command Or Clicks**: Run the goal command; first create an empty design.md file for the design system.
- **Choice Branch**: Optionally ask the agent to use sub-agents to implement features in parallel.

### Add a loop command for UI review
- **Timestamp**: [05:58](https://www.youtube.com/watch?v=2omtxQ0dSFk&t=358)
- **Action**: After the design system is generated, start another session with the loop command set to run periodically (the host tries every 5 minutes). Prompt it to review the UI against the design system, using the browser to visually analyze rather than just reading HTML and CSS.
- **Command Or Clicks**: Start a second session with the loop command; the host notes 5 minutes may be too tight.
- **Choice Branch**: Optionally spin up multiple sub-agents working on different features at the same time.

### Unblock the agent with extra skills
- **Timestamp**: [07:17](https://www.youtube.com/watch?v=2omtxQ0dSFk&t=437)
- **Action**: When the agent slows down or stalls, ask if it is stuck. Here it could not figure out the auth system, so install the better-auth best-practices skill and the next best-practices skill, then tell the agent to use them to reason through the problem.
- **Command Or Clicks**: Install the better-auth best-practices skill and the next best-practices skill in the terminal, then point the agent at them.
- **Choice Branch**: Either let the agent install skills or do it yourself in the terminal.

### Verify the finished Reddit clone
- **Timestamp**: [08:17](https://www.youtube.com/watch?v=2omtxQ0dSFk&t=497)
- **Action**: After about 30 minutes (with a compaction or two), check the running app. You can browse posts and threads, sign up for an account, and leave a comment. The full workflow with sub-agents, skills, and browser testing used only 11% of a $20 plan.
- **Command Or Clicks**: Open the app, sign up with your details, and post a comment to confirm it works.
- **Choice Branch**: Upvoting and downvoting require being signed in.

## Gotchas

### Minimax bills per request every 5 hours, not per token, so a simple hello and a massive PRD both count as one request. Be as detailed as possible in prompts to maximize each request.
- **Severity**: heads_up
- **Timestamp**: [00:46](https://www.youtube.com/watch?v=2omtxQ0dSFk&t=46)

### Open-weight models like Minimax are not always as feature-complete as Opus and can get stuck (here, on the auth system). Assign relevant skills or detailed documentation so the model can reason through the problem.
- **Severity**: serious
- **Timestamp**: [07:17](https://www.youtube.com/watch?v=2omtxQ0dSFk&t=437)

## Where to go next

Download the config and prompts from the GitHub repo in the description, and grab your API key at minimax.io (12% off via the link in the description and pinned comment). The article on how M2.7 helped train its own successor and ranked second only to Opus and GPT-5.4 on the MLE bench is also linked there.

## Concepts surfaced

[[minimax-m2-7]] · [[claude-code]] · [[open-weight-models]] · [[agent-skills]] · [[cost-optimization]]
