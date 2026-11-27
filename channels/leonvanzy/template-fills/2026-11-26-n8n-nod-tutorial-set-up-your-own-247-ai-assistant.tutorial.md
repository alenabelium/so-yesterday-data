---
video_id: vy_NCzx_hAE
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-11-26-n8n-nod-tutorial-set-up-your-own-247-ai-assistant.md
source_transcript: ../transcripts/2026-11-26-n8n-nod-tutorial-set-up-your-own-247-ai-assistant.md
source_summary_hash: sha256:035f908ce3a62df9ffc78aa60adc94e95b3573c18c44c97d85e2358961760e3d
source_transcript_hash: sha256:f200839c97b59590208484b790c42ff5bb1e4ec37ca1df69dbea726dc05cc597
fill_id: b6d3df63-1799-484f-9c1b-fc34a3cd9000
published_at: '2026-11-27T11:30:15.105354'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

By the end of this tutorial, you'll have your own 24/7 AI assistant running on a VPS, connected to email, calendar, and Telegram, with built-in security features.

## Prerequisites

### Hostinger VPS (KVM 4 recommended)
- **Kind**: account
- **Note**: A virtual private server to host Node 24/7; KVM 4 plan recommended for resource-intensive tasks.

### OpenAI ChatGPT account
- **Kind**: account
- **Note**: Recommended for using your ChatGPT subscription instead of paying API rates.

### Telegram account
- **Kind**: account
- **Note**: Used to create a bot and connect Node to Telegram for mobile access.

### Gmail or Outlook account
- **Kind**: account
- **Note**: For connecting email and calendar to Node.

### n8n instance
- **Kind**: tool
- **Note**: Optional but shown for integration; requires MCP server enabled in settings.

## Steps

### Deploy Node on Hostinger VPS
- **Timestamp**: [04:52](https://www.youtube.com/watch?v=vy_NCzx_hAE&t=292)
- **Action**: Choose the KVM 4 plan for better performance, select the term, ensure Node is selected, and apply the coupon code 'Leon' for an extra 10% discount.
- **Command Or Clicks**: Select KVM 4 plan → Choose term → Ensure Node is selected → Click 'I have a coupon' → Enter 'Leon'
- **Choice Branch**: If you prefer a cheaper option, KVM 2 is available but may be resource-constrained.

### Log in to Node via Hostinger control panel
- **Timestamp**: [05:57](https://www.youtube.com/watch?v=vy_NCzx_hAE&t=357)
- **Action**: Navigate to your server in Hostinger, copy the username, click 'Manage Program', enter your username and password, then log in to Node.
- **Command Or Clicks**: Copy username → Click 'Manage Program' → Enter username → Enter password → Click 'Log in'

### Connect email and set preferences
- **Timestamp**: [05:57](https://www.youtube.com/watch?v=vy_NCzx_hAE&t=357)
- **Action**: Connect your Gmail or Outlook account, tell Node about your work/personal balance, and select your interests.
- **Command Or Clicks**: Select Gmail → Choose Google account → Select 'Both' for work/personal → Choose interests

### Connect ChatGPT as the AI provider
- **Timestamp**: [05:57](https://www.youtube.com/watch?v=vy_NCzx_hAE&t=357)
- **Action**: Choose OpenAI and log in with ChatGPT. If you see a URL page, copy the entire URL and paste it into Node's input field to connect.
- **Command Or Clicks**: Select OpenAI → Click 'Log in with ChatGPT' → Copy URL if needed → Paste into Node → Choose GPT-4o

### Connect Google Calendar
- **Timestamp**: [08:11](https://www.youtube.com/watch?v=vy_NCzx_hAE&t=491)
- **Action**: Go to the applications section, search for Google Calendar, and click 'Connect' to add the calendar connector.
- **Command Or Clicks**: Go to Applications → Search 'Google Calendar' → Click 'Connect'

### Turn off usage data sharing
- **Timestamp**: [09:04](https://www.youtube.com/watch?v=vy_NCzx_hAE&t=544)
- **Action**: Navigate to Settings > Privacy and Data, and turn off usage data sharing to protect your privacy.
- **Command Or Clicks**: Settings → Privacy and Data → Toggle off 'Usage data sharing'

### Add additional AI providers (optional)
- **Timestamp**: [09:04](https://www.youtube.com/watch?v=vy_NCzx_hAE&t=544)
- **Action**: Go to Models, add a new connection, choose Anthropic, create an API key on platform.claude.com, and paste it to add Claude.
- **Command Or Clicks**: Models → Add connection → Anthropic → Create API key → Paste key → Connect

### Add a memory manually
- **Timestamp**: [10:01](https://www.youtube.com/watch?v=vy_NCzx_hAE&t=601)
- **Action**: Ask Node to remember a detail, such as your YouTube channel name, and it will appear in the memory settings.
- **Command Or Clicks**: Chat: 'Please add this memory: My YouTube channel is called Leon Van Zyl'

### Create a scheduled task
- **Timestamp**: [10:01](https://www.youtube.com/watch?v=vy_NCzx_hAE&t=601)
- **Action**: Ask Node to add a schedule for 9:00 AM every morning to read emails and calendar events, then verify it in the calendar.
- **Command Or Clicks**: Chat: 'Please add a new schedule for 9:00 every morning. Read my letters and calendar events and take a quick look.'

### Connect Telegram
- **Timestamp**: [12:08](https://www.youtube.com/watch?v=vy_NCzx_hAE&t=728)
- **Action**: Create a new bot on Telegram using /newbot, copy the API key, paste it into Node, open the bot, and pair it with the provided message.
- **Command Or Clicks**: Telegram: /newbot → Name bot → Copy API key → Paste in Node → Open bot → Click 'Run' → Copy pairing message → Paste in chat

### Test prompt injection resistance
- **Timestamp**: [13:03](https://www.youtube.com/watch?v=vy_NCzx_hAE&t=783)
- **Action**: Send an email with a prompt injection attempt, then ask Node to read your latest emails to see if it refuses to follow the injected instructions.
- **Command Or Clicks**: Send email with injection → Chat: 'Please read our latest emails'

### Use browser for research tasks
- **Timestamp**: [14:02](https://www.youtube.com/watch?v=vy_NCzx_hAE&t=842)
- **Action**: Ask Node to use its browser to compare prices across retailers, and view the activity in the browser tab.
- **Command Or Clicks**: Chat: 'Use your browser to compare prices for the RTX 5090 across three major South African retailers and tabulate the results.'

### Connect Node to n8n
- **Timestamp**: [14:58](https://www.youtube.com/watch?v=vy_NCzx_hAE&t=898)
- **Action**: In n8n, enable the MCP server in settings. Then in Node, go to Applications, find n8n, enter your n8n address, and allow access.
- **Command Or Clicks**: n8n: Settings → MCP instance level → Enable MCP server → Node: Applications → n8n → Connect → Enter n8n address → Allow access

### Run an n8n workflow via Node
- **Timestamp**: [15:54](https://www.youtube.com/watch?v=vy_NCzx_hAE&t=954)
- **Action**: Ask Node to list your n8n workflows, then ask it to run a specific workflow, and verify the execution in n8n.
- **Command Or Clicks**: Chat: 'Please list all my n8n workflows' → 'Run the daily AI briefing workflow'

## Gotchas

### If you have a Claude subscription, you cannot use it; you must enter an API key and pay API rates.
- **Severity**: serious
- **Timestamp**: [05:57](https://www.youtube.com/watch?v=vy_NCzx_hAE&t=357)

### Node stops when your laptop sleeps or closes; deploy on a VPS for 24/7 operation.
- **Severity**: blocking
- **Timestamp**: [02:10](https://www.youtube.com/watch?v=vy_NCzx_hAE&t=130)

### Security checks use AI and can be wrong; always review agent actions.
- **Severity**: heads_up
- **Timestamp**: [03:21](https://www.youtube.com/watch?v=vy_NCzx_hAE&t=201)

### When connecting ChatGPT, if you see a URL page, copy the entire URL and paste it into Node; otherwise, connection fails.
- **Severity**: blocking
- **Timestamp**: [05:57](https://www.youtube.com/watch?v=vy_NCzx_hAE&t=357)

## Where to go next

Now that your Node assistant is live, explore connecting more apps, setting up advanced workflows, or integrating with n8n for automation. Check out the linked n8n tutorial for deeper workflow management.

## Concepts surfaced

[[ai-agents]] · [[open-source-ai]] · [[prompt-injection]] · [[vps-deployment]] · [[n8n-integration]] · [[telegram-bot]]
