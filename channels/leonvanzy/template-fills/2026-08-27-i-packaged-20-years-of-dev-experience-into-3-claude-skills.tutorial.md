---
video_id: tqi4cTZZWzQ
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-08-27-i-packaged-20-years-of-dev-experience-into-3-claude-skills.md
source_transcript: ../transcripts/2026-08-27-i-packaged-20-years-of-dev-experience-into-3-claude-skills.md
source_summary_hash: sha256:7081b71e690e3f036cd31c6642e0ec569a626eb8b97ddc1056dedaa246a52070
source_transcript_hash: sha256:3176a3bb3665c8c9883679b4b9f0760a61ac96b2bcf90889f219fd8b27edc3e9
fill_id: b7c8135b-f589-46f0-ae07-be1c3dbc6d0b
published_at: '2026-09-29T11:23:11.827371'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Package 20 years of dev experience into three Claude skills that automate app creation, security auditing, and production deployment.

## Prerequisites

### GitHub Account
- **Kind**: account
- **Note**: Required to host the skill repository and trigger deployments via GitHub Actions.

### Vercel Account
- **Kind**: account
- **Note**: Primary hosting provider for deployment; free hobby tier covers database and storage.

### Claude Code
- **Kind**: tool
- **Note**: The coding agent used to install skills, build the app, and execute deployment commands.

## Steps

### Install Skills via GitHub URL
- **Timestamp**: [10:10](https://www.youtube.com/watch?v=tqi4cTZZWzQ&t=610)
- **Action**: Navigate to the GitHub repository containing the skills, copy the URL, and instruct your coding agent to install them globally.
- **Command Or Clicks**: Paste repo URL into Claude Code and say: 'please install these skills'
- **Choice Branch**: Install globally for access across all projects or locally per project.

### Initialize App with Start Skill
- **Timestamp**: [14:26](https://www.youtube.com/watch?v=tqi4cTZZWzQ&t=866)
- **Action**: Start a new session in your agent and run the 'start an app' command to build the application structure, including authentication and database setup.
- **Command Or Clicks**: Run command: start an app
- **Choice Branch**: Choose PostgreSQL for production or SQLite only for local toy apps.

### Review App for Security and SEO
- **Timestamp**: [20:54](https://www.youtube.com/watch?v=tqi4cTZZWzQ&t=1254)
- **Action**: Run the 'review an app' skill to check for OWASP Top 10 vulnerabilities, optimize SEO with robots.txt and sitemap, and ensure design consistency.
- **Command Or Clicks**: Run command: review an app
- **Choice Branch**: Customize review rules by modifying the skill's reference files.

### Deploy to Vercel
- **Timestamp**: [22:07](https://www.youtube.com/watch?v=tqi4cTZZWzQ&t=1327)
- **Action**: Execute the 'deploy an app' command to set up production infrastructure, including database migration from SQLite to PostgreSQL if needed.
- **Command Or Clicks**: Run command: deploy an app
- **Choice Branch**: Select GitHub integration for CI/CD or direct Vercel deployment.

### Configure Domain and Connectors
- **Timestamp**: [27:06](https://www.youtube.com/watch?v=tqi4cTZZWzQ&t=1626)
- **Action**: Register a custom domain on Vercel and add the MCP server connector in Claude Code to enable AI interaction with the live app.
- **Command Or Clicks**: Add custom connector in Claude Code with the production URL
- **Choice Branch**: Temporary domains will fail MCP connection; use a valid domain.

## Gotchas

### SQLite is only for local toy apps. The deploy skill will automatically migrate to PostgreSQL for production, but you must choose Postgres initially if you plan to deploy.
- **Severity**: blocking
- **Timestamp**: [15:21](https://www.youtube.com/watch?v=tqi4cTZZWzQ&t=921)

### Temporary Vercel domains do not support MCP server connections. You must register a valid custom domain for AI assistants to connect securely.
- **Severity**: blocking
- **Timestamp**: [28:02](https://www.youtube.com/watch?v=tqi4cTZZWzQ&t=1682)

## Where to go next

Explore the 'create brand kit' bonus skill for logo generation or check the agent coding masterclass for design system fundamentals. Visit skills.sh for command-line installation options.

## Concepts surfaced

[[claude-code]] · [[mcp-server]] · [[vercel-deployment]] · [[owasp-security]] · [[seo-optimization]] · [[agentic-coding]]
