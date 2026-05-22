---
video_id: EqcfiT6t53s
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-05-21-mcp-servers-explained-build-your-first-one-with-claude.md
source_transcript: ../transcripts/2026-05-21-mcp-servers-explained-build-your-first-one-with-claude.md
source_summary_hash: sha256:6add9d03e303ad0169edc22e7cca1ce26f95474659faa1ed4b00250c08b06263
source_transcript_hash: sha256:c06c03bce7d11cd5e4cfaeba25e2bb9a826342c38a10d297623ac4a0ba06a840
fill_id: f7e3a6d8-ea68-4f4d-8bb6-b9780d07355d
published_at: '2026-05-21T23:52:26.433093'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Build an agent-ready Next.js app with auth and Postgres, expose it via an MCP server, test locally, and deploy to Vercel.

## Prerequisites

### Claude Code
- **Kind**: tool
- **Note**: Coding agent used to generate the app code and manage skills.

### Neon Database
- **Kind**: account
- **Note**: Postgres provider for storing user records and prompts.

### Vercel Account
- **Kind**: account
- **Note**: Hosting platform for deploying the final application.

### Node.js
- **Kind**: tool
- **Note**: Required to run npx commands and Next.js.

## Steps

### Initialize Next.js project
- **Timestamp**: [01:38](https://www.youtube.com/watch?v=EqcfiT6t53s&t=98)
- **Action**: Create a blank project folder and initialize it with Next.js using the terminal.
- **Command Or Clicks**: npx create-next-app@latest

### Install Claude Code skills
- **Timestamp**: [02:15](https://www.youtube.com/watch?v=EqcfiT6t53s&t=135)
- **Action**: Install specific skills from skills.anthropic.com to help build the app, such as Next Best Practices, Better Auth, and MCP builder.
- **Command Or Clicks**: Run the specific skill installation commands provided on skills.anthropic.com

### Plan the app with Claude Code
- **Timestamp**: [03:29](https://www.youtube.com/watch?v=EqcfiT6t53s&t=209)
- **Action**: Switch to planning mode in Claude Code, upload the architectural diagram, and paste the app planning prompt to generate a development plan.
- **Command Or Clicks**: Paste the planning prompt into Claude Code

### Implement the plan
- **Timestamp**: [04:30](https://www.youtube.com/watch?v=EqcfiT6t53s&t=270)
- **Action**: Save the plan to a folder, clear the context, and instruct Claude Code to implement the entire plan using the goal command.
- **Command Or Clicks**: goal [plan file path]

### Set up Neon Database
- **Timestamp**: [05:36](https://www.youtube.com/watch?v=EqcfiT6t53s&t=336)
- **Action**: Create a free Neon account, create a new project, and create a development branch to get a connection string.
- **Command Or Clicks**: Create project 'AI prompt MCP' and branch 'development' in Neon dashboard

### Configure environment variables
- **Timestamp**: [07:02](https://www.youtube.com/watch?v=EqcfiT6t53s&t=422)
- **Action**: Rename .env.example to .env, paste the Neon development connection string into DATABASE_URL, and let Claude Code migrate the tables.
- **Command Or Clicks**: Rename .env.example to .env and update DATABASE_URL

### Test MCP server locally
- **Timestamp**: [08:41](https://www.youtube.com/watch?v=EqcfiT6t53s&t=521)
- **Action**: Install and run the MCP Inspector to test the server's tools (save prompt, search prompts) with authentication.
- **Command Or Clicks**: npx @modelcontextprotocol/inspector

### Configure mcp.json for Claude Code
- **Timestamp**: [10:16](https://www.youtube.com/watch?v=EqcfiT6t53s&t=616)
- **Action**: Create an mcp.json file in the project root with the server URL, type (HTTP), and API key to connect Claude Code to the app.
- **Command Or Clicks**: Create mcp.json with type: 'http', url, and apiKey

### Deploy to Vercel
- **Timestamp**: [12:11](https://www.youtube.com/watch?v=EqcfiT6t53s&t=731)
- **Action**: Push code to a public GitHub repo, import it to Vercel, set environment variables including the production Neon connection string, and deploy.
- **Command Or Clicks**: Deploy via Vercel dashboard

### Update production auth URL
- **Timestamp**: [13:15](https://www.youtube.com/watch?v=EqcfiT6t53s&t=795)
- **Action**: Copy the Vercel app URL, update the BETTER_AUTH_URL environment variable in Vercel, and redeploy to finalize authentication.
- **Command Or Clicks**: Update BETTER_AUTH_URL env var and redeploy

## Gotchas

### Do not bypass permissions by saying 'yes'; use escape to enter change mode and save plans manually for better context management.
- **Severity**: heads_up
- **Timestamp**: [04:30](https://www.youtube.com/watch?v=EqcfiT6t53s&t=270)

### Ensure you create a development branch in Neon to separate production data from development work.
- **Severity**: serious
- **Timestamp**: [06:15](https://www.youtube.com/watch?v=EqcfiT6t53s&t=375)

### You must add the 'type': 'http' field to mcp.json for the server to connect correctly to Claude Code.
- **Severity**: blocking
- **Timestamp**: [11:11](https://www.youtube.com/watch?v=EqcfiT6t53s&t=671)

### You must update the BETTER_AUTH_URL environment variable in Vercel with the new production domain after deployment.
- **Severity**: blocking
- **Timestamp**: [13:15](https://www.youtube.com/watch?v=EqcfiT6t53s&t=795)

## Where to go next

Explore the Agenty Coding Masterclass for full auth and payment integration. Check the linked GitHub repo for the architectural diagram and planning prompts used in this tutorial.

## Concepts surfaced

[[model-context-protocol]] · [[claude-code]] · [[next-js]] · [[vercel-deployment]] · [[neon-database]] · [[agent-skills]]
