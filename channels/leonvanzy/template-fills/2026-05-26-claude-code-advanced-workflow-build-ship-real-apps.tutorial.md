---
video_id: zVZotTk6ZWU
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-05-26-claude-code-advanced-workflow-build-ship-real-apps.md
source_transcript: ../transcripts/2026-05-26-claude-code-advanced-workflow-build-ship-real-apps.md
source_summary_hash: sha256:3e9955c9029b9da791bf40bda326d1f77089fea3590963c21828d3c9c57d3f89
source_transcript_hash: sha256:7712cfd3c5ab237b82007526da48aa30c24ed3881c4bf52acec2d2c8c382bb2d
fill_id: 5274e330-a0ad-4e61-aed8-6c0a5c948a00
published_at: '2026-05-31T16:27:58.578984'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Build real apps with Claude Code using reusable skills, parallel agent waves, and automated checkpoints.

## Prerequisites

### Claude Code
- **Kind**: tool
- **Note**: The primary AI coding agent used for scaffolding, implementation, and testing.

### GitHub Account
- **Kind**: account
- **Note**: Required to host and retrieve reusable agent skills via npx.

### OpenRouter API Key
- **Kind**: account
- **Note**: Needed for the app's AI summarization and tagging features.

### Oxyabs Account
- **Kind**: account
- **Note**: Required for the web scraping API used in the demo application.

## Steps

### Install boilerplate skill
- **Timestamp**: [01:03](https://www.youtube.com/watch?v=zVZotTk6ZWU&t=63)
- **Action**: Run the npx command to install a reusable agent skill from a GitHub repository, then restart Claude Code to load it.
- **Command Or Clicks**: npx skills <github-repo-name>
- **Choice Branch**: Select the specific skill (e.g., 'create a genic app') from the list of available skills.

### Scaffold project
- **Timestamp**: [02:20](https://www.youtube.com/watch?v=zVZotTk6ZWU&t=140)
- **Action**: Ask the agent to set up the boilerplate project. Answer setup questions (subfolder, database, etc.) to generate the initial structure.
- **Command Or Clicks**: please set up the boilerplate project
- **Choice Branch**: Answer interactive prompts regarding database and folder structure.

### Create design system
- **Timestamp**: [04:25](https://www.youtube.com/watch?v=zVZotTk6ZWU&t=265)
- **Action**: Use a front-end design skill to generate a unique design system, then lock it into a design.md file for consistent UI generation.
- **Command Or Clicks**: Use front-end design skill prompt to generate design, then 'store the design system in the design.md file'
- **Choice Branch**: Review the generated design and approve the plan.

### Generate implementation plan
- **Timestamp**: [08:43](https://www.youtube.com/watch?v=zVZotTk6ZWU&t=523)
- **Action**: Describe the app requirements and constraints in planning mode to generate a detailed implementation plan split into phases.
- **Command Or Clicks**: Describe app requirements including URL scraping, AI summarization, and multi-user support.
- **Choice Branch**: Review the plan and ensure no clarifying questions remain.

### Convert plan to spec
- **Timestamp**: [10:39](https://www.youtube.com/watch?v=zVZotTk6ZWU&t=639)
- **Action**: Run the 'create spec' skill to convert the high-level plan into detailed task files organized by waves in the specs folder.
- **Command Or Clicks**: run create spec skill
- **Choice Branch**: Verify the specs folder contains individual task files with dependencies.

### Run parallel implementation
- **Timestamp**: [12:01](https://www.youtube.com/watch?v=zVZotTk6ZWU&t=721)
- **Action**: Use the goal command in agent view to implement the entire spec, using checkpoint and testing skills automatically.
- **Command Or Clicks**: claude agents --dangerously-skip-permissions
- **Choice Branch**: Use arrow keys in agent view to switch between parallel sessions.

### Set up credentials
- **Timestamp**: [14:22](https://www.youtube.com/watch?v=zVZotTk6ZWU&t=862)
- **Action**: Manually create API keys for OpenRouter and Oxyabs, then add them to the project's .env file.
- **Command Or Clicks**: Add OPEN_ROUTER_API_KEY and OXYABS credentials to .env file
- **Choice Branch**: Restart the implementation session after adding credentials.

### Automate audits and UI
- **Timestamp**: [16:52](https://www.youtube.com/watch?v=zVZotTk6ZWU&t=1012)
- **Action**: Use the loop command to schedule recurring security audits and UI improvements every 10-15 minutes.
- **Command Or Clicks**: loop every 10 minutes [security scanner skill]
- **Choice Branch**: Add another loop for UI review and minor improvements.

## Gotchas

### Do not hit 'bypass permissions' after generating the plan; it tries to implement everything in a single session, which is ineffective.
- **Severity**: blocking
- **Timestamp**: [10:39](https://www.youtube.com/watch?v=zVZotTk6ZWU&t=639)

### Keep the agents.md file lean (e.g., 37 lines) to save tokens and reduce costs while maintaining concise agent instructions.
- **Severity**: serious
- **Timestamp**: [04:25](https://www.youtube.com/watch?v=zVZotTk6ZWU&t=265)

### Web scraping is complex; do not rely on default fetches. Use a dedicated API like Oxyabs and provide developer docs to the agent.
- **Severity**: serious
- **Timestamp**: [09:48](https://www.youtube.com/watch?v=zVZotTk6ZWU&t=588)

## Where to go next

Explore the linked GitHub repository for the boilerplate skills, prompts, and design system templates used in this workflow. Try implementing a different app type using the same parallel agent strategy.

## Concepts surfaced

[[claude-code-workflow]] · [[agent-skills]] · [[parallel-implementation]] · [[design-system-automation]] · [[web-scraping-integration]] · [[automated-testing]]
