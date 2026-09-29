---
video_id: VX3RXec-Ots
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-07-02-openai-codex-full-tutorial-the-claude-code-alternative.md
source_transcript: ../transcripts/2026-07-02-openai-codex-full-tutorial-the-claude-code-alternative.md
source_summary_hash: sha256:a26c0f58b060e768f76f33b61fdaeb6a7a639972f38eba4b483214fd67adfcc8
source_transcript_hash: sha256:1665d057af679b6491d15b043ccc97f01a7f014afe5297a8bb901dd74673885d
fill_id: af22c0c0-bd4d-4d6d-b09f-786ed713c62e
published_at: '2026-09-29T11:06:37.741616'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Build and test a full AI web app autonomously using OpenAI Codex's visual workspace, parallel sessions, and integrated browser testing.

## Prerequisites

### ChatGPT Paid Account
- **Kind**: account
- **Note**: Free tier hits limits fast; paid plan needed for meaningful coding work.

### Codex Desktop App
- **Kind**: tool
- **Note**: Download from openai.com/codex for macOS or Windows.

### Ollama
- **Kind**: tool
- **Note**: Install to run local LLMs like Qwen 3.6 for the project.

## Steps

### Install Codex and configure usage limits
- **Timestamp**: [00:00](https://www.youtube.com/watch?v=VX3RXec-Ots&t=0)
- **Action**: Download the Codex app from openai.com/codex for your OS. Open the app, go to Settings > Usage and Billing to monitor your 5-hour and weekly usage limits to avoid being locked out.
- **Command Or Clicks**: Go to openai.com/codex, click download for Windows/macOS, open app, Settings > Usage and Billing.
- **Choice Branch**: Use paid plan for meaningful coding; free tier limits are restrictive.

### Enable browser control and integrations
- **Timestamp**: [03:25](https://www.youtube.com/watch?v=VX3RXec-Ots&t=205)
- **Action**: In Settings > Browser, enable 'Let Codex control the built-in browser' so the agent can test its own code. Configure MCP servers and computer use permissions as needed.
- **Command Or Clicks**: Settings > Browser > Enable 'Let Codex control the built-in browser'.
- **Choice Branch**: Disable computer use if you don't want agent access to Chrome/apps.

### Create project and configure agent settings
- **Timestamp**: [04:57](https://www.youtube.com/watch?v=VX3RXec-Ots&t=297)
- **Action**: Click 'New Project', name it (e.g., 'My Fitness Guru'), and select a folder. Set approval mode and model selection (e.g., GPT 5.5, Extra High reasoning).
- **Command Or Clicks**: Click 'New Project', name folder, select GPT 5.5 model.
- **Choice Branch**: Use 'Ask for approval' for safety or 'Full access' for autonomy.

### Set up planning mode and custom skills
- **Timestamp**: [06:15](https://www.youtube.com/watch?v=VX3RXec-Ots&t=375)
- **Action**: Enter planning mode (Shift+Tab) to discuss the project without code changes. Install skills via Plugins or by asking the agent to install a skill from skills.sh (e.g., 'Grill Me' skill).
- **Command Or Clicks**: Shift+Tab for plan mode. Ask agent: 'Please add this skill [command from skills.sh]'.
- **Choice Branch**: Ensure skills are installed at global/user level if not found.

### Generate design mockups with parallel sessions
- **Timestamp**: [10:15](https://www.youtube.com/watch?v=VX3RXec-Ots&t=615)
- **Action**: Create a second session in the same workspace. Use the ImageGen skill to generate a UI mockup while the first session plans the architecture.
- **Command Or Clicks**: New Session > 'Please use ImageGen 2 to generate a mock-up for our app idea.'
- **Choice Branch**: Run parallel sessions for design and planning simultaneously.

### Refine plan and split into feature files
- **Timestamp**: [12:23](https://www.youtube.com/watch?v=VX3RXec-Ots&t=743)
- **Action**: Save the plan to a /plans folder without implementing. Ask the agent to split the plan into individual feature files with clear instructions to avoid context window overload.
- **Command Or Clicks**: Shift+Tab > 'Please save this plan in the /plans folder... Do not implement anything yet.' Then 'Split the plan up into separate feature files.'
- **Choice Branch**: Never click 'Yes, implement this plan' directly; split first.

### Implement project with /goal command
- **Timestamp**: [15:07](https://www.youtube.com/watch?v=VX3RXec-Ots&t=907)
- **Action**: Start a new session and use the /goal command to instruct the agent to implement all features in the features folder and test them using the integrated browser.
- **Command Or Clicks**: Type '/goal' > 'Please implement all features in the features folder. Do not stop until all features are built and tested. Use your integrated browser for testing.'
- **Choice Branch**: Use /goal for autonomous completion rather than file-by-file implementation.

### Monitor progress and verify final app
- **Timestamp**: [16:21](https://www.youtube.com/watch?v=VX3RXec-Ots&t=981)
- **Action**: Use the /pet command to track agent activity via the avatar. Once done, open the app in your browser to verify functionality and context updates.
- **Command Or Clicks**: Type '/pet' to view avatar updates. Open generated app in browser.
- **Choice Branch**: Archive sessions when no longer needed to keep workspace tidy.

## Gotchas

### Hitting usage limits will lock you out until the 5-hour or weekly reset. Monitor limits in Settings.
- **Severity**: serious
- **Timestamp**: [02:31](https://www.youtube.com/watch?v=VX3RXec-Ots&t=151)

### Clicking 'Yes, implement this plan' directly is bad practice; always split the plan into feature files first to manage context.
- **Severity**: blocking
- **Timestamp**: [12:23](https://www.youtube.com/watch?v=VX3RXec-Ots&t=743)

### Skills may install in the wrong location; ask the agent to install them at global or user level if not visible.
- **Severity**: heads_up
- **Timestamp**: [09:26](https://www.youtube.com/watch?v=VX3RXec-Ots&t=566)

## Where to go next

Explore the Agenty Coding Masterclass for design systems and Cloud Code course. Check the description for links to Agenty Labs and Ollama setup guides.

## Concepts surfaced

[[agentic-coding]] · [[openai-codex]] · [[ollama-local-llm]] · [[parallel-agent-sessions]] · [[automated-browser-testing]] · [[context-window-management]]
