---
video_id: EqcfiT6t53s
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-05-21-mcp-servers-explained-build-your-first-one-with-claude.md
source_transcript: ../transcripts/2026-05-21-mcp-servers-explained-build-your-first-one-with-claude.md
source_summary_hash: sha256:6add9d03e303ad0169edc22e7cca1ce26f95474659faa1ed4b00250c08b06263
source_transcript_hash: sha256:c06c03bce7d11cd5e4cfaeba25e2bb9a826342c38a10d297623ac4a0ba06a840
fill_id: c1f2f1ab-bf21-4521-a088-1e828fe41c4c
published_at: '2026-05-30T11:14:18.919714'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Build an agent-ready Next.js app with auth and Postgres, expose it via an MCP server, test it, and deploy to Vercel.

## Prerequisites

### Neon Account
- **Kind**: account
- **Note**: Free tier account for Postgres database hosting and branch management.

### Vercel Account
- **Kind**: account
- **Note**: Account required to deploy the Next.js application to a public URL.

### Claude Code
- **Kind**: tool
- **Note**: Coding agent used to generate the app, plan, and MCP server configuration.

### Node.js Environment
- **Kind**: tool
- **Note**: Required to run npx commands and the Next.js application locally.

## Steps

### Initialize Next.js project
- **Timestamp**: [01:38](https://www.youtube.com/watch?v=EqcfiT6t53s&t=98)
- **Action**: Create a blank project folder and initialize a Next.js application using the CLI.
- **Command Or Clicks**: npx create-next-app@latest

### Install agent skills
- **Timestamp**: [02:15](https://www.youtube.com/watch?v=EqcfiT6t53s&t=135)
- **Action**: Install specific skills for Next.js, auth, and UI design from the Anthropic skills repository.
- **Command Or Clicks**: Visit skills.anthropic.com, copy skill commands, and run them in the terminal.

### Plan the application
- **Timestamp**: [03:29](https://www.youtube.com/watch?v=EqcfiT6t53s&t=209)
- **Action**: Switch to planning mode in Claude Code, upload the architectural diagram, and paste the app planning prompt to generate a development plan.
- **Command Or Clicks**: Paste planning prompt in Claude Code; save plan to ./plans folder.

### Generate the app code
- **Timestamp**: [04:30](https://www.youtube.com/watch?v=EqcfiT6t53s&t=270)
- **Action**: Clear the context window, load the saved plan, and instruct Claude Code to implement the entire application without skipping steps.
- **Command Or Clicks**: Run goal command, load plan, say: 'Please implement this entire plan. Do not skip anything.'

### Set up Neon database
- **Timestamp**: [05:36](https://www.youtube.com/watch?v=EqcfiT6t53s&t=336)
- **Action**: Sign up for Neon, create a project, and create a 'development' branch to get a connection string.
- **Command Or Clicks**: Neon Dashboard -> Create Project -> Create Branch 'development' -> Copy Connection String.

### Configure environment variables
- **Timestamp**: [07:02](https://www.youtube.com/watch?v=EqcfiT6t53s&t=422)
- **Action**: Rename .env.example to .env, paste the Neon development connection string, and allow Claude to proceed with migrations.
- **Command Or Clicks**: Rename .env.example to .env; update DATABASE_URL with Neon connection string.

### Test MCP server locally
- **Timestamp**: [08:41](https://www.youtube.com/watch?v=EqcfiT6t53s&t=521)
- **Action**: Open a new terminal, launch the MCP Inspector, connect via streamable HTTP, and authenticate with an API key.
- **Command Or Clicks**: npx @modelcontextprotocol/inspector; Select 'streamable HTTP'; Paste API key after 'Bearer'.

### Configure local MCP client
- **Timestamp**: [10:16](https://www.youtube.com/watch?v=EqcfiT6t53s&t=616)
- **Action**: Create mcp.json in the project root, add the server URL, API key, and set the transport type to HTTP.
- **Command Or Clicks**: Create mcp.json; add url, apiKey, and type: 'http'; restart Claude Code.

### Deploy to Vercel
- **Timestamp**: [12:11](https://www.youtube.com/watch?v=EqcfiT6t53s&t=731)
- **Action**: Push code to a public GitHub repo, import it to Vercel, set environment variables including the production Neon DB URL, and deploy.
- **Command Or Clicks**: Vercel Dashboard -> New Project -> Import Repo -> Set env vars -> Deploy.

### Finalize production config
- **Timestamp**: [13:53](https://www.youtube.com/watch?v=EqcfiT6t53s&t=833)
- **Action**: Copy the Vercel production URL, update the BETTER_AUTH_URL environment variable, redeploy, and update the local MCP client with the production URL and key.
- **Command Or Clicks**: Vercel Dashboard -> Settings -> Environment Variables -> Update BETTER_AUTH_URL -> Redeploy.

## Gotchas

### Do not bypass permissions by saying 'yes'; use escape to enter change mode and save plans manually for context management.
- **Severity**: serious
- **Timestamp**: [04:30](https://www.youtube.com/watch?v=EqcfiT6t53s&t=270)

### Ensure the MCP transport type is explicitly set to 'HTTP' in the mcp.json configuration file.
- **Severity**: blocking
- **Timestamp**: [11:11](https://www.youtube.com/watch?v=EqcfiT6t53s&t=671)

### You must update the BETTER_AUTH_URL environment variable in Vercel after deployment to match the new public domain.
- **Severity**: blocking
- **Timestamp**: [13:53](https://www.youtube.com/watch?v=EqcfiT6t53s&t=833)

## Where to go next

Explore the Agenty Coding Masterclass for full auth and payment integration details. Check the linked GitHub repo for the architectural diagram and planning prompts.

## Concepts surfaced

[[model-context-protocol]] · [[claude-code]] · [[next-js]] · [[vercel-deployment]] · [[neon-database]] · [[agent-skills]]
