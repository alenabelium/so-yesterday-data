---
video_id: prLO7NGU4f0
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-05-11-i-built-an-ai-thumbnail-generator-with-codex.md
source_transcript: ../transcripts/2026-05-11-i-built-an-ai-thumbnail-generator-with-codex.md
source_summary_hash: sha256:cc210d4e05fcf34197f4bb0806576b9b8cef6bd7d356a09ae24992bc8baba878
source_transcript_hash: sha256:81d280bf95e157840835ff8530c18cd68cd133730e798770ee77fbf1baa5e4c1
fill_id: e1edaeaf-7114-4b79-9da8-ca60dc269079
published_at: '2026-05-18T07:18:09.817167'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Build a functional AI thumbnail generator app from scratch using the Codex CLI, GPT-5.5, and GPT Image 2 with a focus on iterative UI design and sub-agent delegation.

## Prerequisites

### GPT Plus Subscription
- **Kind**: account
- **Note**: Basic Plus plan used in video; upgrade may be needed for high token usage during complex builds.

### OpenAI API Key
- **Kind**: account
- **Note**: Required for GPT Image 2 integration; requires loading credit onto the account as image generation is not free.

### Docker
- **Kind**: tool
- **Note**: Needed to run `docker compose up -d` for the Postgres database.

### Node.js / npm
- **Kind**: tool
- **Note**: Required to run the Next.js app and database migrations.

### VS Code
- **Kind**: tool
- **Note**: Used to open the project folder and run Codex within the editor for better visibility.

## Steps

### Initialize project and scaffold Next.js app
- **Timestamp**: [00:48](https://www.youtube.com/watch?v=prLO7NGU4f0&t=48)
- **Action**: Open a new command prompt, navigate to the project folder, and scaffold the Next.js app with authentication, Postgres, and Drizzle ORM.
- **Command Or Clicks**: cd into the project folder
create aentic app@latest .
docker compose up -d
npm run db:migrate
- **Choice Branch**: Use GPT-5.5 with high reasoning level. Run commands manually to save tokens.

### Open project in VS Code and configure Codex
- **Timestamp**: [02:11](https://www.youtube.com/watch?v=prLO7NGU4f0&t=131)
- **Action**: Open the project in VS Code, initialize Codex, and configure the agents.md file to enforce planning mode, sub-agent delegation, and UI design rules.
- **Command Or Clicks**: code .
Open agents.md
Set planning mode instructions
Set sub-agent delegation rules
- **Choice Branch**: Use the front-end design skill and Next.js skill pre-installed in the agents folder.

### Generate initial design system
- **Timestamp**: [03:44](https://www.youtube.com/watch?v=prLO7NGU4f0&t=224)
- **Action**: Prompt Codex to replace the boilerplate with an AI image studio design system, using dark mode and the front-end design skill. Verify the output via screenshots.
- **Command Or Clicks**: Prompt: 'create a design system for this application... make dark mode the default'
npm run dev
- **Choice Branch**: Skip planning mode for speed; accept token usage for visual verification.

### Commit design and plan dashboard UI
- **Timestamp**: [05:41](https://www.youtube.com/watch?v=prLO7NGU4f0&t=341)
- **Action**: Save the design system to the design.md file, commit changes to GitHub, and switch to planning mode to outline the dashboard UI without implementing backend logic.
- **Command Or Clicks**: git commit -m 'design system'
git push
Switch to planning mode
- **Choice Branch**: Focus on UI first to avoid wasting tokens on wrong logic.

### Persist plan and implement dashboard UI
- **Timestamp**: [07:03](https://www.youtube.com/watch?v=prLO7NGU4f0&t=423)
- **Action**: Save the implementation plan to a plans folder, start a new conversation, and instruct Codex to implement the plan using sub-agents in parallel.
- **Command Or Clicks**: Create plans folder
Store plan in plans folder
Start new conversation
Prompt: 'please go ahead and implement this plan'
- **Choice Branch**: Allow full access if sub-agents stall due to permission issues.

### Fix UI bugs and verify responsiveness
- **Timestamp**: [11:43](https://www.youtube.com/watch?v=prLO7NGU4f0&t=703)
- **Action**: Review the generated dashboard, identify non-functional nav items, and prompt Codex to fix them. Check responsiveness via mobile mode.
- **Command Or Clicks**: Press F12
Switch to mobile mode
Prompt: 'fix top nav menu items'
- **Choice Branch**: Remove testing section from agents.md if token limits are reached.

### Integrate GPT Image 2 API
- **Timestamp**: [14:53](https://www.youtube.com/watch?v=prLO7NGU4f0&t=893)
- **Action**: Switch to planning mode, select GPT Image 2, and provide the OpenAI API documentation URL. Add the API key to the .env file.
- **Command Or Clicks**: platform.openai.com/api keys
Create new key
Edit .env file
Add OPENAI_API_KEY variable
- **Choice Branch**: Use GPT Image 2 for reference image editing capabilities.

### Implement image generation functionality
- **Timestamp**: [17:16](https://www.youtube.com/watch?v=prLO7NGU4f0&t=1036)
- **Action**: Instruct Codex to implement the actual image generation logic using the provided plan and API key. Test uploading avatars and assets.
- **Command Or Clicks**: Prompt: 'implement this plan'
Upload avatar and assets
Click 'generate concept'
- **Choice Branch**: Load credit onto OpenAI account as image generation costs money.

### Refine homepage and finalize build
- **Timestamp**: [19:46](https://www.youtube.com/watch?v=prLO7NGU4f0&t=1186)
- **Action**: Fix the homepage to remove direct generation capabilities and replace it with marketing copy and a Codex-generated stock image.
- **Command Or Clicks**: Prompt: 'redesign homepage... generate marketing copy'
Commit changes
- **Choice Branch**: Use Codex's built-in image generation for the homepage hero image.

## Gotchas

### Sub-agents may stall if they request permissions that aren't visible; run the permissions command to allow full access.
- **Severity**: blocking
- **Timestamp**: [10:44](https://www.youtube.com/watch?v=prLO7NGU4f0&t=644)

### GPT Image 2 integration requires loading credit onto your OpenAI account; it is not free.
- **Severity**: serious
- **Timestamp**: [17:16](https://www.youtube.com/watch?v=prLO7NGU4f0&t=1036)

### High token usage can hit GPT Plus limits quickly; consider removing the testing section from agents.md or upgrading your plan.
- **Severity**: serious
- **Timestamp**: [11:43](https://www.youtube.com/watch?v=prLO7NGU4f0&t=703)

### Homepage should not allow direct image generation; users must log in to the dashboard first.
- **Severity**: blocking
- **Timestamp**: [19:46](https://www.youtube.com/watch?v=prLO7NGU4f0&t=1186)

## Where to go next

Explore the Gentic Labs for deeper AI build workflows. Check out the OpenAI API documentation for advanced GPT Image 2 editing features.

## Concepts surfaced

[[codex-cli]] · [[gpt-image-2]] · [[next-js]] · [[sub-agent-delegation]] · [[ai-thumbnail-generator]] · [[iterative-planning]]
