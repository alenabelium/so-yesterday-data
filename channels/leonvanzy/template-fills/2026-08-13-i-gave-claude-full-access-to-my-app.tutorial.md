---
video_id: N2Ogvx_U8uM
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-08-13-i-gave-claude-full-access-to-my-app.md
source_transcript: ../transcripts/2026-08-13-i-gave-claude-full-access-to-my-app.md
source_summary_hash: sha256:efcf527fac2b47464c9cf7573178cb51c7f3b930a5465abed11fc57652f7f8d3
source_transcript_hash: sha256:c2ad74ef0c2834869f922bcd1baae9009f6bb26bc87a6eafc9eee305381af22a
fill_id: 95bb005b-d429-4599-a958-8934df2ee793
published_at: '2026-09-29T11:22:28.586221'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Build a custom MCP server with OAuth to let Claude interact with your app.

## Prerequisites

### Vercel Account
- **Kind**: account
- **Note**: Required for deploying the app to a public URL for Claude to access.

### GitHub Account
- **Kind**: account
- **Note**: Needed to host the source code and link it to Vercel.

### VS Code + Claude Code
- **Kind**: tool
- **Note**: Used to generate the app and manage the MCP server integration.

### Coding Agent Knowledge
- **Kind**: knowledge
- **Note**: Understanding of prompting agents to build features and handle context.

## Steps

### Initialize Project with Skill
- **Timestamp**: [01:12](https://www.youtube.com/watch?v=N2Ogvx_U8uM&t=72)
- **Action**: Open a blank project and install the 'start and app' skill via the terminal to scaffold the web application.
- **Command Or Clicks**: Paste the skill installation command into the terminal and select 'claude code' at the global level.
- **Choice Branch**: Use the 'start and app' skill to scaffold the app with battle-tested components.

### Define App Requirements
- **Timestamp**: [02:21](https://www.youtube.com/watch?v=N2Ogvx_U8uM&t=141)
- **Action**: Switch to planning mode and describe the Trello-like Kanban app requirements to the agent.
- **Command Or Clicks**: Describe requirements: multi-org support, email/password auth, drag-and-drop cards. Run 'start and app skill'.
- **Choice Branch**: Specify that the agent must use the skill to generate the initial codebase.

### Select Production Database
- **Timestamp**: [04:10](https://www.youtube.com/watch?v=N2Ogvx_U8uM&t=250)
- **Action**: Answer the agent's database question by selecting Postgres in Docker to ensure production readiness.
- **Command Or Clicks**: Select 'Postgres in docker' when prompted by the agent.
- **Choice Branch**: Avoid SQLite if you plan to deploy to production, as it creates local files.

### Expand Implementation Plan
- **Timestamp**: [05:13](https://www.youtube.com/watch?v=N2Ogvx_U8uM&t=313)
- **Action**: Store the high-level plan and prompt the agent to create a detailed implementation plan with individual feature files.
- **Command Or Clicks**: Run: 'expand this plan, create a detailed implementation plan, store it in the same folder and call it implementation plan.md'.
- **Choice Branch**: Force the agent to break down features to avoid missing details during implementation.

### Install Playwright MCP
- **Timestamp**: [07:20](https://www.youtube.com/watch?v=N2Ogvx_U8uM&t=440)
- **Action**: Install the Playwright MCP server to allow the agent to test the app in a browser.
- **Command Or Clicks**: Run: 'install the playright MCP server' (sic) in a new session.
- **Choice Branch**: Skip if using an IDE with an embedded browser like the Claude desktop app.

### Configure Testing Context
- **Timestamp**: [08:21](https://www.youtube.com/watch?v=N2Ogvx_U8uM&t=501)
- **Action**: Create agents.md and claude.md files to instruct the agent to reuse test data and use Playwright.
- **Command Or Clicks**: Create 'agents.md' with a 'testing the app' section referencing Playwright and 'test data.json'.
- **Choice Branch**: Ensure the agent reuses the same test user data instead of creating new accounts each time.

### Implement Features
- **Timestamp**: [09:29](https://www.youtube.com/watch?v=N2Ogvx_U8uM&t=569)
- **Action**: Move files to a 'foundation' folder and run the goal command to implement all features.
- **Command Or Clicks**: Run: 'go ahead and implement all the features in this folder. to not stop until everything has been implemented and tested.'
- **Choice Branch**: Use the goal command for full implementation or drag files one by one for cheaper models.

### Deploy to Vercel
- **Timestamp**: [12:16](https://www.youtube.com/watch?v=N2Ogvx_U8uM&t=736)
- **Action**: Push code to GitHub and import the project into Vercel for production hosting.
- **Command Or Clicks**: Create a public GitHub repo, push code, then import to Vercel via the dashboard.
- **Choice Branch**: Ensure the repository is public if you want others to view the code.

### Configure Environment Variables
- **Timestamp**: [13:27](https://www.youtube.com/watch?v=N2Ogvx_U8uM&t=807)
- **Action**: Set up a Neon Postgres database and update Vercel environment variables with the new URL and domain.
- **Command Or Clicks**: Create Neon database, copy URL, update 'POSTGRES_URL' and 'BETTER_AUTH_URL' in Vercel settings.
- **Choice Branch**: Update 'BETTER_AUTH_URL' to the Vercel-generated domain after deployment.

### Fix Build Command
- **Timestamp**: [14:26](https://www.youtube.com/watch?v=N2Ogvx_U8uM&t=866)
- **Action**: Troubleshoot deployment errors by checking logs and adding the database migration to the build command.
- **Command Or Clicks**: Update the Vercel build command to include 'next build' and database migration steps.
- **Choice Branch**: Add migration to the build command to ensure database tables are created in production.

### Install MCP Builder Skill
- **Timestamp**: [17:13](https://www.youtube.com/watch?v=N2Ogvx_U8uM&t=1033)
- **Action**: Install the 'better auth' and 'MCP builder' skills to help the agent create the MCP server.
- **Command Or Clicks**: Run the installation commands for the 'better auth' skill and 'MCP builder' skill in the project.
- **Choice Branch**: Install skills at the project level to provide context to the agent.

### Generate MCP Server Code
- **Timestamp**: [21:25](https://www.youtube.com/watch?v=N2Ogvx_U8uM&t=1285)
- **Action**: Prompt the agent to create a remote MCP server that exposes app tools and handles OAuth.
- **Command Or Clicks**: Prompt: 'create a remote MCP server... expose all tools... live in /mcp... use better auth skill and MCP builder skill'.
- **Choice Branch**: Include links to Better Auth and Claude connector documentation in the prompt for context.

### Add Connector in Claude
- **Timestamp**: [23:44](https://www.youtube.com/watch?v=N2Ogvx_U8uM&t=1424)
- **Action**: Add the custom connector in Claude by pasting the MCP server URL and authenticating via OAuth.
- **Command Or Clicks**: Go to 'Add Connectors', 'Add Custom Connector', paste URL, and click 'Connect'.
- **Choice Branch**: Approve the OAuth request on the generated authentication page.

### Test Agent Interaction
- **Timestamp**: [25:09](https://www.youtube.com/watch?v=N2Ogvx_U8uM&t=1509)
- **Action**: Use Claude to create and manage tasks in the app to verify the connection works.
- **Command Or Clicks**: Prompt: 'create a new task in lanes... assign the task to myself'.
- **Choice Branch**: Allow the agent to call tools when prompted to verify access.

## Gotchas

### Using SQLite prevents production deployment as it relies on local files.
- **Severity**: blocking
- **Timestamp**: [04:10](https://www.youtube.com/watch?v=N2Ogvx_U8uM&t=250)

### The app fails in production if the build command doesn't run database migrations.
- **Severity**: blocking
- **Timestamp**: [14:26](https://www.youtube.com/watch?v=N2Ogvx_U8uM&t=866)

### The Better Auth MCP authentication page in the docs is deprecated; use the new provider URL.
- **Severity**: serious
- **Timestamp**: [21:25](https://www.youtube.com/watch?v=N2Ogvx_U8uM&t=1285)

## Where to go next

Join Agentic Labs for a masterclass on working with coding agents and building SaaS applications from scratch.

## Concepts surfaced

[[mcp-server]] · [[oauth-authentication]] · [[vercel-deployment]] · [[claude-connectors]] · [[agentic-coding]]
