---
video_id: RnxXr_2ix3k
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-07-23-hermes-agent-from-setup-to-247-ai-assistant-complete-guide.md
source_transcript: ../transcripts/2026-07-23-hermes-agent-from-setup-to-247-ai-assistant-complete-guide.md
source_summary_hash: sha256:c8aa5dbe85a7897e8dc6363cd922c739cdae3104eb70b9ed722db5ec4a8fd944
source_transcript_hash: sha256:55c3bd79dfb75b9a00f8dd7e4e37a0be0810f9020d93cff1cefd50d5a5484da0
fill_id: ea70aaa1-7114-447a-a080-263d955c7df3
published_at: '2026-09-29T11:21:01.455717'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Set up Hermes Agent locally, deploy it on a VPS for 24/7 access, and sync your desktop app to control it from anywhere via Telegram.

## Prerequisites

### Hermes Agent Website
- **Kind**: account
- **Note**: Official site for downloading the desktop app and terminal installer.

### OpenAI Account
- **Kind**: account
- **Note**: Required for connecting GPT-5.6 Soul model via OAuth.

### VPS Provider
- **Kind**: account
- **Note**: Hostinger or similar for 24/7 remote deployment.

### Telegram BotFather
- **Kind**: tool
- **Note**: Needed to create a bot and get the API key for messaging.

## Steps

### Install Hermes via Terminal
- **Timestamp**: [01:19](https://www.youtube.com/watch?v=RnxXr_2ix3k&t=79)
- **Action**: Copy the installation command from the website for your OS and run it in PowerShell or terminal to install dependencies.
- **Command Or Clicks**: Copy command from website -> Paste in PowerShell -> Run
- **Choice Branch**: Choose custom endpoint (32) to connect to local Ollama or select a cloud provider.

### Configure Local Ollama
- **Timestamp**: [03:50](https://www.youtube.com/watch?v=RnxXr_2ix3k&t=230)
- **Action**: Select custom endpoint, paste your Ollama endpoint URL, use 'Ollama' as the API key, and confirm the detected model.
- **Command Or Clicks**: Enter '32' -> Paste Ollama endpoint -> Enter 'Ollama' as key -> Confirm model
- **Choice Branch**: Auto-detect the model or manually specify the model name.

### Launch Desktop App
- **Timestamp**: [05:43](https://www.youtube.com/watch?v=RnxXr_2ix3k&t=343)
- **Action**: Download and install the Hermes Desktop app from the website, then launch it to access the chat interface.
- **Command Or Clicks**: Click 'Install Hermes' -> Launch app
- **Choice Branch**: Note: Custom endpoints for local models must be set via terminal first.

### Connect OpenAI Provider
- **Timestamp**: [08:51](https://www.youtube.com/watch?v=RnxXr_2ix3k&t=531)
- **Action**: Go to Settings > Providers, select OpenAI OAuth, copy the code, and paste it into your OpenAI account to link the subscription.
- **Command Or Clicks**: Settings > Providers > OpenAI OAuth > Copy Code > Paste in Browser > Continue
- **Choice Branch**: Refresh models if GPT-5.6 does not appear immediately.

### Setup Telegram Bot
- **Timestamp**: [13:00](https://www.youtube.com/watch?v=RnxXr_2ix3k&t=780)
- **Action**: Create a bot via BotFather in Telegram, get the API key and your User ID, then enter them in Hermes Messaging settings.
- **Command Or Clicks**: BotFather: /new bot -> Copy API Key -> Get User ID -> Paste in Hermes Settings
- **Choice Branch**: Restart the gateway in Hermes after saving changes to activate the bot.

### Deploy to VPS
- **Timestamp**: [16:24](https://www.youtube.com/watch?v=RnxXr_2ix3k&t=984)
- **Action**: Rent a VPS (e.g., Hostinger), select Hermes Agent as the OS, and complete the one-click installation.
- **Command Or Clicks**: Select Plan -> Choose OS 'Hermes Agent' -> Apply Coupon -> Complete Purchase
- **Choice Branch**: Retrieve credentials from Docker Manager if forgotten.

### Sync Desktop to VPS
- **Timestamp**: [22:39](https://www.youtube.com/watch?v=RnxXr_2ix3k&t=1359)
- **Action**: In Desktop Settings > Gateway, paste the VPS URL (excluding /chat) and sign in with VPS credentials to sync the local app to the remote agent.
- **Command Or Clicks**: Settings > Gateway > Paste VPS URL > Sign In > Test Remote
- **Choice Branch**: Disable local Telegram to prevent conflicts with the VPS instance.

## Gotchas

### Desktop app cannot set custom local endpoints; you must configure them via the terminal CLI first.
- **Severity**: blocking
- **Timestamp**: [06:30](https://www.youtube.com/watch?v=RnxXr_2ix3k&t=390)

### Do not piggyback on Anthropic's Claude Code subscription; it is expensive and against their terms.
- **Severity**: serious
- **Timestamp**: [08:15](https://www.youtube.com/watch?v=RnxXr_2ix3k&t=495)

### Restart the gateway in Hermes after saving Telegram settings to ensure the bot connects.
- **Severity**: heads_up
- **Timestamp**: [13:45](https://www.youtube.com/watch?v=RnxXr_2ix3k&t=825)

## Where to go next

Explore the 7-Day Builder Challenge for the RAM framework to master agentic coding workflows.

## Concepts surfaced

[[hermes-agent-setup]] · [[ollama-local-llm]] · [[vps-deployment]] · [[telegram-bot-integration]] · [[openai-oauth]] · [[persistent-memory]]
