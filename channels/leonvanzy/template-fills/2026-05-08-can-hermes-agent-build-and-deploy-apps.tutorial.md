---
video_id: gxx39SE0aDw
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-05-08-can-hermes-agent-build-and-deploy-apps.md
source_transcript: ../transcripts/2026-05-08-can-hermes-agent-build-and-deploy-apps.md
source_summary_hash: sha256:4f323cb584fd5e7bb7278b921e42ccd5cb5a3d7097bf8cfdef25989d1b8b9e25
source_transcript_hash: sha256:e80b14d22bf13c4f4251842733161c3d9986348ef77c1223212fd0bf93e95a85
fill_id: edf502c4-7142-4bed-9e7b-f61a2a78eb8b
published_at: '2026-10-19T21:39:36.131167'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Turn your Hermes agent into a remote coding assistant that can build and deploy web apps to Vercel from a single Telegram prompt.

## Prerequisites

### Hermes agent
- **Kind**: tool
- **Note**: A running Hermes agent instance, ideally on a VPS with Docker and Telegram integration.

### VPS
- **Kind**: hardware
- **Note**: A virtual private server (e.g., Hostinger KVM2) to host the Hermes agent.

### Vercel account
- **Kind**: account
- **Note**: A free Vercel account to deploy the generated web apps.

### Telegram bot
- **Kind**: account
- **Note**: A Telegram bot token and your user ID for messaging the agent.

### OpenAI API key
- **Kind**: account
- **Note**: An OpenAI API key with access to a coding-capable model like GPT-5.5.

## Steps

### Deploy Hermes on a VPS
- **Timestamp**: [01:23](https://www.youtube.com/watch?v=gxx39SE0aDw&t=83)
- **Action**: Deploy Hermes on a VPS using a one-click installer. Choose a plan, apply a coupon code, and complete checkout. Save the admin username and password.
- **Command Or Clicks**: Hostinger → select KVM2 → deploy → apply coupon 'LeonHermes' → checkout
- **Choice Branch**: If you forgot credentials, access them via Docker manager → manage → environment.

### Configure Hermes with OpenAI and Telegram
- **Timestamp**: [02:30](https://www.youtube.com/watch?v=gxx39SE0aDw&t=150)
- **Action**: During setup, choose OpenAI as the provider, select a coding-capable model (e.g., GPT-5.5), and configure Telegram messaging by providing your bot token and user ID.
- **Command Or Clicks**: Setup wizard → OpenAI → model: GPT-5.5 → Telegram → paste bot token and user ID
- **Choice Branch**: If Telegram messages aren't received, ask Hermes to start the gateway.

### Install Vercel CLI on the server
- **Timestamp**: [04:37](https://www.youtube.com/watch?v=gxx39SE0aDw&t=277)
- **Action**: Ask Hermes to install the Vercel CLI globally on the server. This tool will let the agent connect to Vercel and deploy projects.
- **Command Or Clicks**: npm install -g vercel

### Set the Vercel token as an environment variable
- **Timestamp**: [05:56](https://www.youtube.com/watch?v=gxx39SE0aDw&t=356)
- **Action**: Create a Vercel access token, then set it as an environment variable inside the Hermes container. Use Docker exec to run the export command and source the bashrc.
- **Command Or Clicks**: docker exec -it <container> bash
echo 'export VERCEL_TOKEN="<token>"' >> /root/.bashrc
source /root/.bashrc
vercel whoami

### Install the Vercel CLI skill
- **Timestamp**: [08:22](https://www.youtube.com/watch?v=gxx39SE0aDw&t=502)
- **Action**: Install the 'vercel-cli-with-token' skill from skills.sh to give Hermes the ability to use Vercel with the token. Start a new conversation to load the skill.
- **Command Or Clicks**: Ask Hermes: 'Please install this agent skill for using Vercel with the token' and paste the skill URL.

### Add project workflow rules
- **Timestamp**: [09:47](https://www.youtube.com/watch?v=gxx39SE0aDw&t=587)
- **Action**: Instruct Hermes to always create projects in a 'projects' folder, use git for version control, and deploy to production with Vercel. The agent will save these rules to its memory.
- **Command Or Clicks**: Tell Hermes: 'Whenever the user asks you to write code, create a subfolder in /projects, use git, and deploy with Vercel CLI to production.'

### Install the frontend design skill
- **Timestamp**: [10:56](https://www.youtube.com/watch?v=gxx39SE0aDw&t=656)
- **Action**: Install the 'frontend-design' skill globally so Hermes can create beautiful UIs for any project.
- **Command Or Clicks**: Ask Hermes: 'Please install this skill' and paste the skill URL.

### Prompt Hermes to build a portfolio app
- **Timestamp**: [11:30](https://www.youtube.com/watch?v=gxx39SE0aDw&t=690)
- **Action**: Send a prompt asking Hermes to create a new portfolio web app, scrape your YouTube channel, and use the frontend design skill. Wait for the agent to finish and provide a live URL.
- **Command Or Clicks**: Message: 'Create a new web app for my portfolio page. Scrape info from my YouTube channel and use your frontend design skill.'

### Verify the deployed app and update it
- **Timestamp**: [12:08](https://www.youtube.com/watch?v=gxx39SE0aDw&t=728)
- **Action**: Open the production URL to check the app. Then send a follow-up prompt to update the app (e.g., add a profile image) and confirm Hermes redeploys automatically.
- **Command Or Clicks**: Message: 'Please update my portfolio app with this profile image.'

## Gotchas

### Do not share your Vercel token directly with the agent. It will be sent over the network to the model provider. Instead, set it as an environment variable.
- **Severity**: serious
- **Timestamp**: [05:56](https://www.youtube.com/watch?v=gxx39SE0aDw&t=356)

### If you don't receive Telegram messages, the gateway may not be running. Ask Hermes to start it.
- **Severity**: heads_up
- **Timestamp**: [03:30](https://www.youtube.com/watch?v=gxx39SE0aDw&t=210)

### The agent may try to deploy to a preview environment. You must instruct it to deploy to production.
- **Severity**: blocking
- **Timestamp**: [09:47](https://www.youtube.com/watch?v=gxx39SE0aDw&t=587)

## Where to go next

If you want to build real software with coding agents, join Agentic Labs for the Agentic Coding Masterclass. New videos added daily, plus a community of 700+ AI builders and weekly Q&A sessions.

## Concepts surfaced

[[ai-agents]] · [[coding-agents]] · [[vercel-cli]] · [[telegram-bot]] · [[vps-deployment]] · [[frontend-design]]
