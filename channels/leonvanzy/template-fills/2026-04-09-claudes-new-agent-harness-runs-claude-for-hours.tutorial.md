---
video_id: DpfLbBuhHOg
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-04-09-claudes-new-agent-harness-runs-claude-for-hours.md
source_transcript: ../transcripts/2026-04-09-claudes-new-agent-harness-runs-claude-for-hours.md
source_summary_hash: sha256:70f03f0e6f6d1b88dc17729a658eefc930096b3912514d4205fec39231a39835
source_transcript_hash: sha256:de2ed27069d1f9a770405b2010596c7ace5e91b4bc696fb36e06c574ba7a76f5
fill_id: ad72547d-e919-4740-a3d6-91b99f46f134
published_at: '2026-10-19T21:47:43.587690'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Build Ship It, a web app that delegates coding tasks to Claude's fully managed, long-running agents on Anthropic's infrastructure.

## Prerequisites

### Anthropic Console account
- **Kind**: account
- **Note**: Required to create an API key; does not work with Claude Code subscription.

### Anthropic API key
- **Kind**: account
- **Note**: Create at platform.claude.com; used for all Managed Agents interactions.

### Node.js and npm
- **Kind**: tool
- **Note**: Needed to run the CLI and install the Next.js project.

### TypeScript
- **Kind**: knowledge
- **Note**: The SDK example uses TypeScript; familiarity helps.

## Steps

### Create an Anthropic API key
- **Timestamp**: [03:42](https://www.youtube.com/watch?v=DpfLbBuhHOg&t=222)
- **Action**: Sign in to platform.claude.com, navigate to API keys, create a new key named 'managed agents demo', and copy it to a safe place.
- **Command Or Clicks**: platform.claude.com → Get API key → Create new key

### Prototype an agent in the console
- **Timestamp**: [04:32](https://www.youtube.com/watch?v=DpfLbBuhHOg&t=272)
- **Action**: Open the Managed Agents console via the quick start link, choose a template like 'structured extractor', configure the environment, and test the agent in the live panel.
- **Command Or Clicks**: platform.claude.com → Managed Agents → Quick start → Structured extractor

### Set up the CLI and create an agent
- **Timestamp**: [06:19](https://www.youtube.com/watch?v=DpfLbBuhHOg&t=379)
- **Action**: Install the CLI dependencies, verify with `ant --version`, set your API key, then create an agent using the `agents create` command with name, model, and system prompt.
- **Command Or Clicks**: npm install
ant --version
ant beta agents create --name shipit-agent --model '{"id":"opus"}' --system-prompt '...'

### Create an environment and start a session
- **Timestamp**: [08:33](https://www.youtube.com/watch?v=DpfLbBuhHOg&t=513)
- **Action**: Create an environment with `environments create`, then start a session with `sessions create` using the agent and environment IDs.
- **Command Or Clicks**: ant beta environments create --name shipit-env --type cloud --network unrestricted
ant beta sessions create --agent-id <AGENT_ID> --environment-id <ENV_ID> --name shipit-quickstart

### Send a message and stream events
- **Timestamp**: [09:43](https://www.youtube.com/watch?v=DpfLbBuhHOg&t=583)
- **Action**: Send a user message via the events send command, then stream the agent's response with events stream.
- **Command Or Clicks**: ant beta events send --session-id <SESSION_ID> --event '{"type":"user","message":{"role":"user","content":"Hello, introduce yourself in one sentence."}}'
ant beta events stream --session-id <SESSION_ID>

### Scaffold the Next.js project
- **Timestamp**: [10:59](https://www.youtube.com/watch?v=DpfLbBuhHOg&t=659)
- **Action**: Create a new folder, install Next.js with the create-next-app command, and create a `.env` file with your Anthropic API key.
- **Command Or Clicks**: npx create-next-app@latest .
# .env
ANTHROPIC_API_KEY=your-key

### Use Claude to build the UI and scrape docs
- **Timestamp**: [12:15](https://www.youtube.com/watch?v=DpfLbBuhHOg&t=735)
- **Action**: Ask Claude to replace the boilerplate with a chat window, install the front-end design skill from skills.sh, and scrape the Managed Agents documentation into a docs folder.
- **Command Or Clicks**: Claude: 'Please use your front-end design skill to make this look awesome.'
Claude: 'Scrape all pages related to managed agents and store them in docs/managed-agents as markdown.'

### Plan and implement the Ship It app
- **Timestamp**: [14:24](https://www.youtube.com/watch?v=DpfLbBuhHOg&t=864)
- **Action**: In planning mode, describe the Ship It application, assign the front-end design skill, and let Claude create a plan. Then approve and let Claude implement the full integration.
- **Command Or Clicks**: Claude: 'Build Ship It, a UI that sends prompts to Claude Managed Agents and streams responses.'

### Run the agent and monitor in console
- **Timestamp**: [17:58](https://www.youtube.com/watch?v=DpfLbBuhHOg&t=1078)
- **Action**: Send a task like 'build a kanban board like Trello', fix the skill creation error, and watch the agent run in the console's agents, sessions, and debug tabs.
- **Command Or Clicks**: Claude: 'Build a kanban board like Trello.'

## Gotchas

### Managed Agents does not work with a Claude Code subscription; you must use a paid API key.
- **Severity**: blocking
- **Timestamp**: [03:42](https://www.youtube.com/watch?v=DpfLbBuhHOg&t=222)

### The front-end design skill must be created in the remote session before use; the SDK provides a function for this.
- **Severity**: serious
- **Timestamp**: [16:30](https://www.youtube.com/watch?v=DpfLbBuhHOg&t=990)

### The CLI commands are beta and may change; check `ant --help` for current usage.
- **Severity**: heads_up
- **Timestamp**: [07:32](https://www.youtube.com/watch?v=DpfLbBuhHOg&t=452)

## Where to go next

Now that you've built Ship It, explore adding MCP servers, custom skills, or more complex agent tasks. For deeper learning, consider the Agentic Coding Masterclass mentioned in the video.

## Concepts surfaced

[[managed-agents]] · [[agent-harness]] · [[prompt-caching]] · [[remote-execution]] · [[sdk-integration]] · [[skills]]
