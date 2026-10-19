---
video_id: uZGDO0L-Dr4
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-05-05-opencode-tutorial-for-beginners-setup-agents-skills-mcp.md
source_transcript: ../transcripts/2026-05-05-opencode-tutorial-for-beginners-setup-agents-skills-mcp.md
source_summary_hash: sha256:330b279ec2a4c7b2997e5fc68c2f72a9d7a4d956ee503728aa8c189b309a423c
source_transcript_hash: sha256:5ab67c4e2597229b32372a3ce87de09115d84a25696cb30dda61fc2e511db915
fill_id: bd1aa640-fe24-4700-8f34-039edf58b770
published_at: '2026-10-19T21:39:37.966868'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

By the end of this video, you'll have OpenCode installed, connected to your preferred LLM, and configured with skills, memory files, sub-agents, and MCP for a full agentic coding workflow.

## Prerequisites

### Terminal or command prompt
- **Kind**: os
- **Note**: Required to run the installation command and interact with OpenCode.

### OpenCode Zen account
- **Kind**: account
- **Note**: Optional but recommended for free model access; requires API key creation.

### OpenAI subscription (Pro/Plus)
- **Kind**: account
- **Note**: Recommended for paid model access; avoids API key billing.

### OpenRouter account
- **Kind**: account
- **Note**: Used for AI SDK inference in the example app; requires API key.

### Node.js and npm
- **Kind**: tool
- **Note**: Needed to run the Next.js project and npm commands.

### VS Code or Cursor (optional)
- **Kind**: tool
- **Note**: Optional but helpful for viewing files created by the agent.

## Steps

### Install OpenCode via curl
- **Timestamp**: [00:52](https://www.youtube.com/watch?v=uZGDO0L-Dr4&t=52)
- **Action**: Copy the curl command from opencode.ai and paste it into your terminal to install OpenCode.
- **Command Or Clicks**: curl -fsSL https://opencode.ai/install | bash

### Start OpenCode in a project folder
- **Timestamp**: [01:45](https://www.youtube.com/watch?v=uZGDO0L-Dr4&t=105)
- **Action**: Navigate to your project folder and run 'opencode' to start the tool. Optionally, start from VS Code or Cursor to view files easily.
- **Command Or Clicks**: cd your-project && opencode

### Connect to a provider
- **Timestamp**: [01:45](https://www.youtube.com/watch?v=uZGDO0L-Dr4&t=105)
- **Action**: Run '/connect' to select a provider. For free models, choose OpenCode Zen and create an API key from the dashboard.
- **Command Or Clicks**: /connect
- **Choice Branch**: Select OpenCode Zen for free models, or later choose OpenAI for paid subscription.

### Select a model
- **Timestamp**: [03:17](https://www.youtube.com/watch?v=uZGDO0L-Dr4&t=197)
- **Action**: After connecting, pick a model from the list. For free models, options like Big Pickle, HY3, Miniax 2.5, and Neotron 3 are available.
- **Choice Branch**: Choose a free model for testing or a premium model like GPT-5.5 for production.

### Scaffold a Next.js project
- **Timestamp**: [03:17](https://www.youtube.com/watch?v=uZGDO0L-Dr4&t=197)
- **Action**: Ask the agent to set up a new Next.js project using the npx command in the current directory.
- **Command Or Clicks**: Please set up a new Next.js project using the npx command in the current working directory.

### Run the dev server
- **Timestamp**: [04:19](https://www.youtube.com/watch?v=uZGDO0L-Dr4&t=259)
- **Action**: Ask the agent to start the dev server. Interrupt with Escape if needed and clear the session with '/new'.
- **Command Or Clicks**: Please start the dev server.

### Connect to a paid provider (OpenAI)
- **Timestamp**: [05:22](https://www.youtube.com/watch?v=uZGDO0L-Dr4&t=322)
- **Action**: Run '/connect' again and select OpenAI. Choose the subscription option (Pro/Plus) and sign in via the browser.
- **Command Or Clicks**: /connect
- **Choice Branch**: Select 'ChatGPT Pro or Plus' to use your subscription.

### Change model and reasoning effort
- **Timestamp**: [06:31](https://www.youtube.com/watch?v=uZGDO0L-Dr4&t=391)
- **Action**: Use '/models' to select GPT-5.5. Then use '/variance' to set reasoning effort to high.
- **Command Or Clicks**: /models
/variance

### Install front-end design skill
- **Timestamp**: [08:23](https://www.youtube.com/watch?v=uZGDO0L-Dr4&t=503)
- **Action**: From skills.sh, copy the install command for the front-end design skill and run it in a new terminal. Install at project level.
- **Command Or Clicks**: opencode skill add frontend-design

### Install Next.js and AI SDK skills
- **Timestamp**: [09:00](https://www.youtube.com/watch?v=uZGDO0L-Dr4&t=540)
- **Action**: Install the Next.js skill from Vercel Labs and the AI SDK skill from skills.sh, both at project level.
- **Command Or Clicks**: opencode skill add nextjs
opencode skill add ai-sdk

### Verify skills and restart if needed
- **Timestamp**: [10:44](https://www.youtube.com/watch?v=uZGDO0L-Dr4&t=644)
- **Action**: Run '/skills' to confirm the skills are available. If not, exit and reopen OpenCode.
- **Command Or Clicks**: /skills
/exit

### Create and configure agents.md
- **Timestamp**: [10:44](https://www.youtube.com/watch?v=uZGDO0L-Dr4&t=644)
- **Action**: Create an agents.md file in the project root. Use '/init' to auto-generate it, then replace with your own strict instructions.
- **Command Or Clicks**: /init

### Add rules to agents.md
- **Timestamp**: [12:05](https://www.youtube.com/watch?v=uZGDO0L-Dr4&t=725)
- **Action**: Add rules like 'respond with emojis only' to test, then replace with production rules: concise responses, ask clarifying questions in plan mode, use sub-agents for implementation, and enforce design system.

### Create design.md
- **Timestamp**: [14:06](https://www.youtube.com/watch?v=uZGDO0L-Dr4&t=846)
- **Action**: Create a design.md file in the project root with the UI design system details (colors, spacing, etc.) and reference it in agents.md.

### Start a new session and commit
- **Timestamp**: [15:00](https://www.youtube.com/watch?v=uZGDO0L-Dr4&t=900)
- **Action**: Create a new session to load the updated agents.md. Commit the memory files and design system.
- **Command Or Clicks**: /new
git add . && git commit -m "memory files and design system"

### Plan the app in plan mode
- **Timestamp**: [18:44](https://www.youtube.com/watch?v=uZGDO0L-Dr4&t=1124)
- **Action**: Switch to plan mode (Shift+Tab) and provide a detailed prompt for the AI project planner app. Answer clarifying questions and confirm the plan.
- **Command Or Clicks**: Shift+Tab

### Persist the plan
- **Timestamp**: [21:24](https://www.youtube.com/watch?v=uZGDO0L-Dr4&t=1284)
- **Action**: Create a plans folder in the agents folder and ask the agent to store the plan there without making code changes.
- **Command Or Clicks**: mkdir -p .agents/plans

### Implement the plan in build mode
- **Timestamp**: [22:58](https://www.youtube.com/watch?v=uZGDO0L-Dr4&t=1378)
- **Action**: Switch to build mode, create a new session, and ask the agent to implement the plan. The agent will split tasks and use sub-agents.
- **Command Or Clicks**: Shift+Tab
/new

### Set up environment variables
- **Timestamp**: [23:55](https://www.youtube.com/watch?v=uZGDO0L-Dr4&t=1435)
- **Action**: Create a .env file in the project root and add the OpenRouter API key.
- **Command Or Clicks**: touch .env
echo "OPENROUTER_API_KEY=your-key" >> .env

### Create a custom sub-agent
- **Timestamp**: [24:05](https://www.youtube.com/watch?v=uZGDO0L-Dr4&t=1445)
- **Action**: Run 'opencode agent create' to create a custom agent, e.g., a coder agent, in the local project.
- **Command Or Clicks**: opencode agent create

### View sub-agent progress
- **Timestamp**: [25:14](https://www.youtube.com/watch?v=uZGDO0L-Dr4&t=1514)
- **Action**: Press Ctrl+X and then Down to view sub-agents. Use Right/Left to switch between them.
- **Command Or Clicks**: Ctrl+X, Down

### Test the app manually
- **Timestamp**: [26:34](https://www.youtube.com/watch?v=uZGDO0L-Dr4&t=1594)
- **Action**: Start the dev server with 'npm run dev' and test the app in the browser.
- **Command Or Clicks**: npm run dev

### Request UI and streaming improvements
- **Timestamp**: [27:38](https://www.youtube.com/watch?v=uZGDO0L-Dr4&t=1658)
- **Action**: Ask the agent to use AI SDK structured output streaming and replace JSON arrays with editable cards.

### Add Playwright MCP server
- **Timestamp**: [29:14](https://www.youtube.com/watch?v=uZGDO0L-Dr4&t=1754)
- **Action**: Create an opencode.json file in the project root and add the Playwright MCP configuration.
- **Command Or Clicks**: touch opencode.json

### Restart OpenCode to load MCP
- **Timestamp**: [30:16](https://www.youtube.com/watch?v=uZGDO0L-Dr4&t=1816)
- **Action**: Exit OpenCode and reopen to load the MCP configuration. Verify with '/mcps'.
- **Command Or Clicks**: /exit
opencode
/mcps

### Revamp UI and test with Playwright
- **Timestamp**: [30:56](https://www.youtube.com/watch?v=uZGDO0L-Dr4&t=1856)
- **Action**: Ask the agent to revamp the UI using the front-end design skill and test the app using Playwright MCP tools.

## Gotchas

### Free models may use your prompts for training; avoid sensitive data.
- **Severity**: serious
- **Timestamp**: [03:17](https://www.youtube.com/watch?v=uZGDO0L-Dr4&t=197)

### Using API keys for coding is the most expensive option; prefer subscriptions.
- **Severity**: serious
- **Timestamp**: [05:22](https://www.youtube.com/watch?v=uZGDO0L-Dr4&t=322)

### Anthropic subscriptions are being banned for tools like OpenCode; avoid using them.
- **Severity**: blocking
- **Timestamp**: [05:22](https://www.youtube.com/watch?v=uZGDO0L-Dr4&t=322)

### If skills don't appear, exit and reopen OpenCode.
- **Severity**: heads_up
- **Timestamp**: [10:44](https://www.youtube.com/watch?v=uZGDO0L-Dr4&t=644)

### Keep agents.md minimal; too much info can bloat the context window.
- **Severity**: heads_up
- **Timestamp**: [12:05](https://www.youtube.com/watch?v=uZGDO0L-Dr4&t=725)

### Never commit .env files with API keys to public repositories.
- **Severity**: serious
- **Timestamp**: [23:55](https://www.youtube.com/watch?v=uZGDO0L-Dr4&t=1435)

## Where to go next

Now that you've mastered OpenCode's core features, explore creating custom sub-agents for specialized tasks, integrating more MCP servers, and building your own design systems. Check out the Agentic Labs community for advanced tutorials and live Q&A.

## Concepts surfaced

[[agentic-coding]] · [[mcp-servers]] · [[sub-agents]] · [[skills]] · [[memory-files]] · [[open-source-ai]]
