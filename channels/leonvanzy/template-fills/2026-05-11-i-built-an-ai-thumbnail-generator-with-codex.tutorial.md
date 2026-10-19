---
video_id: prLO7NGU4f0
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-05-11-i-built-an-ai-thumbnail-generator-with-codex.md
source_transcript: ../transcripts/2026-05-11-i-built-an-ai-thumbnail-generator-with-codex.md
source_summary_hash: sha256:889fb08df1e2b94f1d6d3def71f94fef9b8d5d1933cc14a4796125450b76a442
source_transcript_hash: sha256:81d280bf95e157840835ff8530c18cd68cd133730e798770ee77fbf1baa5e4c1
fill_id: 43c7e202-251b-4d85-be5f-680103f361ea
published_at: '2026-10-19T21:39:34.552598'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

You'll have a working AI thumbnail generator app built entirely with Codex CLI, from design system to live image generation.

## Prerequisites

### ChatGPT Plus subscription
- **Kind**: account
- **Note**: Basic plus plan used; may hit usage limits during long builds.

### OpenAI API key
- **Kind**: account
- **Note**: Required for image generation; must load credits onto the account.

### Docker
- **Kind**: tool
- **Note**: Used to run a local Postgres database via docker compose.

### Node.js and npm
- **Kind**: tool
- **Note**: Needed to scaffold Next.js app and run database migrations.

### VS Code
- **Kind**: tool
- **Note**: Recommended for easier project navigation and running Codex.

## Steps

### Scaffold Next.js project with create-next-app
- **Timestamp**: [00:48](https://www.youtube.com/watch?v=prLO7NGU4f0&t=48)
- **Action**: Open a terminal, cd into the project folder, and run create-next-app to scaffold a Next.js project with user authentication, Postgres database, Drizzle ORM, and other essentials.
- **Command Or Clicks**: cd into project folder; run: create-next-app@latest .

### Start Postgres and run migrations
- **Timestamp**: [01:30](https://www.youtube.com/watch?v=prLO7NGU4f0&t=90)
- **Action**: Start the Postgres database using Docker Compose, then run the database migration to create user tables. Optionally, use db studio to view the database contents.
- **Command Or Clicks**: docker compose up -d; npm run db:migrate; npm run db:studio

### Open project in VS Code
- **Timestamp**: [02:11](https://www.youtube.com/watch?v=prLO7NGU4f0&t=131)
- **Action**: Open the project folder in VS Code to simplify navigation and run Codex within the editor.
- **Command Or Clicks**: Open folder in VS Code

### Create a new design system
- **Timestamp**: [03:44](https://www.youtube.com/watch?v=prLO7NGU4f0&t=224)
- **Action**: In Codex, instruct the agent to redesign the homepage as an AI image studio using the front-end design skill, with dark mode as default. The agent will use Playwright to test and screenshot the result.
- **Command Or Clicks**: Prompt: 'Hey there. So currently we've got a boilerplate Next.js application set up...'

### Run dev server and review design
- **Timestamp**: [05:41](https://www.youtube.com/watch?v=prLO7NGU4f0&t=341)
- **Action**: Run the dev server and open the app in the browser to review the new design. Test sign-up/sign-in flow.
- **Command Or Clicks**: npm run dev

### Save design system to design.md
- **Timestamp**: [06:30](https://www.youtube.com/watch?v=prLO7NGU4f0&t=390)
- **Action**: Add the design file to the chat and ask Codex to update the design.md file with the new design system for future consistency.
- **Command Or Clicks**: Attach design file; prompt: 'I really like this design system. Please can you update the design.md file...'

### Commit design system and push to GitHub
- **Timestamp**: [06:45](https://www.youtube.com/watch?v=prLO7NGU4f0&t=405)
- **Action**: Commit the untracked files with a message 'design system' and publish to GitHub.
- **Command Or Clicks**: git commit -m 'design system'; git push

### Plan dashboard UI in planning mode
- **Timestamp**: [07:03](https://www.youtube.com/watch?v=prLO7NGU4f0&t=423)
- **Action**: Switch to planning mode and describe the dashboard pages: library of thumbnails, upload reference images, assets, and generate page. Instruct agent to ask clarifying questions and not implement AI functionality yet.
- **Command Or Clicks**: Switch to plan mode; prompt describing dashboard features

### Save plan to plans folder
- **Timestamp**: [09:32](https://www.youtube.com/watch?v=prLO7NGU4f0&t=572)
- **Action**: Press escape in Codex and ask to store the plan in a new 'plans' subfolder. Then start a new conversation to clear context.
- **Command Or Clicks**: Press escape; prompt: 'Please store this plan in the plans folder.'

### Implement plan with sub-agents
- **Timestamp**: [10:00](https://www.youtube.com/watch?v=prLO7NGU4f0&t=600)
- **Action**: Start a new conversation, pull in the plan, and instruct Codex to implement it. Ensure not in planning mode. Codex will run multiple sub-agents in parallel.
- **Command Or Clicks**: New conversation; attach plan; prompt: 'Please go ahead and implement this plan.'

### Fix permissions for sub-agents
- **Timestamp**: [10:44](https://www.youtube.com/watch?v=prLO7NGU4f0&t=644)
- **Action**: If sub-agents stall, run the permissions command in Codex and allow full access, then retry.
- **Command Or Clicks**: /permissions

### Review dashboard and fix nav
- **Timestamp**: [13:42](https://www.youtube.com/watch?v=prLO7NGU4f0&t=822)
- **Action**: Restart dev server, sign in, and review the new dashboard. Report that top nav buttons don't work; Codex fixes them. Check responsiveness with F12.
- **Command Or Clicks**: npm run dev; F12 for mobile view

### Commit dashboard changes
- **Timestamp**: [14:53](https://www.youtube.com/watch?v=prLO7NGU4f0&t=893)
- **Action**: Commit all changes with message 'dashboard'.
- **Command Or Clicks**: git commit -m 'dashboard'

### Plan AI image generation integration
- **Timestamp**: [15:30](https://www.youtube.com/watch?v=prLO7NGU4f0&t=930)
- **Action**: Switch to planning mode and instruct Codex to integrate GPT Image 2 for image generation, referencing the OpenAI API article for instructions.
- **Command Or Clicks**: Switch to plan mode; prompt with article URL

### Set up OpenAI API key
- **Timestamp**: [16:30](https://www.youtube.com/watch?v=prLO7NGU4f0&t=990)
- **Action**: Create an API key at platform.openai.com/api-keys, then add it to the .env file under AI integration section. Remove OpenRouter variables if not used.
- **Command Or Clicks**: Create key; edit .env: OPENAI_API_KEY=...

### Save plan and implement
- **Timestamp**: [17:16](https://www.youtube.com/watch?v=prLO7NGU4f0&t=1036)
- **Action**: Press escape, store the plan in plans folder, start new conversation, pull in plan, and instruct to implement.
- **Command Or Clicks**: Press escape; prompt: 'Please store this plan in the plans folder.'; new conversation; prompt: 'Please go ahead and implement this plan.'

### Test thumbnail generation
- **Timestamp**: [18:30](https://www.youtube.com/watch?v=prLO7NGU4f0&t=1110)
- **Action**: Upload avatar images and an asset (e.g., cursor logo), then generate a thumbnail with a prompt. Verify the output uses the reference images.
- **Command Or Clicks**: Upload images; prompt: 'Create a thumbnail with my avatar on the right, cursor logo on the left, text full tutorial.'

### Redesign homepage
- **Timestamp**: [19:46](https://www.youtube.com/watch?v=prLO7NGU4f0&t=1186)
- **Action**: Commit working dashboard, then instruct Codex to redesign the homepage as a landing page with marketing copy, removing image generation capability. Codex can generate its own stock images.
- **Command Or Clicks**: git commit -m 'working dashboard'; prompt for homepage redesign

## Gotchas

### Sub-agents may stall waiting for permissions; run /permissions and allow full access to continue.
- **Severity**: blocking
- **Timestamp**: [10:44](https://www.youtube.com/watch?v=prLO7NGU4f0&t=644)

### ChatGPT Plus plan has usage limits; you may hit the 5-hour limit mid-build and need to upgrade.
- **Severity**: serious
- **Timestamp**: [11:43](https://www.youtube.com/watch?v=prLO7NGU4f0&t=703)

### Generating images with OpenAI is not free; you must load credits onto your account.
- **Severity**: serious
- **Timestamp**: [17:16](https://www.youtube.com/watch?v=prLO7NGU4f0&t=1036)

### The homepage initially allowed image generation; it should be a landing page only, requiring login to generate.
- **Severity**: heads_up
- **Timestamp**: [19:46](https://www.youtube.com/watch?v=prLO7NGU4f0&t=1186)

## Where to go next

Now that you have a working AI thumbnail generator, consider adding more features like batch generation, style presets, or integrating with other AI models. Join the Gentic Labs community for weekly build challenges.

## Concepts surfaced

[[codex-cli]] · [[next-js]] · [[gpt-image-2]] · [[design-system]] · [[sub-agents]] · [[playwright-testing]]
