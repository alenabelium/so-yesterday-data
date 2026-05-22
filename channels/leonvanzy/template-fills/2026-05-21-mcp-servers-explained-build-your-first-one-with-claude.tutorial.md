---
video_id: EqcfiT6t53s
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-05-21-mcp-servers-explained-build-your-first-one-with-claude.md
source_transcript: ../transcripts/2026-05-21-mcp-servers-explained-build-your-first-one-with-claude.md
source_summary_hash: sha256:6add9d03e303ad0169edc22e7cca1ce26f95474659faa1ed4b00250c08b06263
source_transcript_hash: sha256:c06c03bce7d11cd5e4cfaeba25e2bb9a826342c38a10d297623ac4a0ba06a840
fill_id: 9e744246-7af5-4b2f-a035-43e187f99ebc
published_at: '2026-05-22T01:01:24.683007'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Build an agent-ready Next.js app with auth and Postgres, expose it via an MCP server, and deploy to Vercel.

## Prerequisites

### Node.js / npm
- **Kind**: tool
- **Note**: Required to run npx and create-next-app.

### Anthropic Account
- **Kind**: account
- **Note**: Needed to access skills.anthropic.com and install agent skills.

### Neon Database
- **Kind**: account
- **Note**: Free tier Postgres provider used for user and prompt storage.

### Vercel Account
- **Kind**: account
- **Note**: Required for hosting the final application publicly.

### Claude Code
- **Kind**: tool
- **Note**: Coding agent used to generate the app and MCP server configuration.

## Steps

### Initialize Next.js project
- **Timestamp**: [01:38](https://www.youtube.com/watch?v=EqcfiT6t53s&t=98)
- **Action**: Create a blank project folder and initialize it with Next.js using the CLI.
- **Command Or Clicks**: npx create-next-app@latest

### Install agent skills
- **Timestamp**: [02:15](https://www.youtube.com/watch?v=EqcfiT6t53s&t=135)
- **Action**: Visit skills.anthropic.com, search for relevant skills (e.g., front-end design, Next Best Practices, Better Auth, MCP builder), copy their installation commands, and run them in the terminal to install them into Claude Code.
- **Command Or Clicks**: Run the copied skill installation commands in the terminal.

### Plan the app in Claude Code
- **Timestamp**: [03:29](https://www.youtube.com/watch?v=EqcfiT6t53s&t=209)
- **Action**: Switch to planning mode in Claude Code, upload the architectural diagram, and paste the app planning prompt to generate a development plan.
- **Command Or Clicks**: Paste the planning prompt into Claude Code.

### Save and execute the plan
- **Timestamp**: [04:30](https://www.youtube.com/watch?v=EqcfiT6t53s&t=270)
- **Action**: Save the generated plan to a 'plans' folder, clear the context, and then use the goal command to instruct Claude to implement the entire plan without skipping steps.
- **Command Or Clicks**: Run the goal command and pull in the plan file.

### Set up Neon database
- **Timestamp**: [05:36](https://www.youtube.com/watch?v=EqcfiT6t53s&t=336)
- **Action**: Sign up for Neon, create a new project, and create a 'development' branch to get a connection string.
- **Command Or Clicks**: Create branch in Neon dashboard.

### Configure environment variables
- **Timestamp**: [07:02](https://www.youtube.com/watch?v=EqcfiT6t53s&t=422)
- **Action**: Copy the .env.example file created by Claude, rename it to .env, and replace the database URL with the Neon development connection string.
- **Command Or Clicks**: Rename .env.example to .env and update DATABASE_URL.

### Test MCP server locally
- **Timestamp**: [08:41](https://www.youtube.com/watch?v=EqcfiT6t53s&t=521)
- **Action**: Open a new terminal and run the MCP Inspector to test the server's tools (save prompt, search prompts) with authentication.
- **Command Or Clicks**: npx @modelcontextprotocol/inspector

### Configure local MCP client
- **Timestamp**: [10:16](https://www.youtube.com/watch?v=EqcfiT6t53s&t=616)
- **Action**: Create an mcp.json file in the project root with the server URL, type (HTTP), and your API key to connect Claude Code to your new server.
- **Command Or Clicks**: Create mcp.json with type: http, url, and apiKey.

### Deploy to Vercel
- **Timestamp**: [12:11](https://www.youtube.com/watch?v=EqcfiT6t53s&t=731)
- **Action**: Commit and push code to a public GitHub repo, import it into Vercel, set environment variables (including the production Neon DB URL), and deploy.
- **Command Or Clicks**: Deploy via Vercel dashboard.

### Finalize production config
- **Timestamp**: [13:53](https://www.youtube.com/watch?v=EqcfiT6t53s&t=833)
- **Action**: Update the BETTER_AUTH_URL in Vercel environment variables with the new public domain, redeploy, and update the local mcp.json to point to the production URL and use the production API key.
- **Command Or Clicks**: Update BETTER_AUTH_URL and redeploy in Vercel.

## Gotchas

### Do not bypass permissions by saying 'yes'; use escape to enter change mode and save plans manually for better context management.
- **Severity**: heads_up
- **Timestamp**: [04:30](https://www.youtube.com/watch?v=EqcfiT6t53s&t=270)

### Ensure you create a development branch in Neon to separate production data from development work.
- **Severity**: serious
- **Timestamp**: [06:15](https://www.youtube.com/watch?v=EqcfiT6t53s&t=375)

### You must add the 'type: http' field to your mcp.json configuration, otherwise the server will not connect properly.
- **Severity**: blocking
- **Timestamp**: [11:11](https://www.youtube.com/watch?v=EqcfiT6t53s&t=671)

### After deploying to Vercel, you must update the BETTER_AUTH_URL environment variable with the new public domain and redeploy for auth to work.
- **Severity**: blocking
- **Timestamp**: [13:53](https://www.youtube.com/watch?v=EqcfiT6t53s&t=833)

## Where to go next

Explore the Agenty Coding Masterclass for full auth and payment integration. Check the linked GitHub repo for the architectural diagram and planning prompts used in this tutorial.

## Concepts surfaced

[[model-context-protocol]] · [[claude-code]] · [[next-js]] · [[vercel-deployment]] · [[neon-database]] · [[agent-skills]]
