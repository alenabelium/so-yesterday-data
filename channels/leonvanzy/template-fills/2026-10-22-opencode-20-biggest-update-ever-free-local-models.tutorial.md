---
video_id: OyuId4YQiIs
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-10-22-opencode-20-biggest-update-ever-free-local-models.md
source_transcript: ../transcripts/2026-10-22-opencode-20-biggest-update-ever-free-local-models.md
source_summary_hash: sha256:984a8f2565386a597885ea8b1b1bc5694c43854331e9ae7ecc49828e8fa01b11
source_transcript_hash: sha256:a7238839435302a30b0b475ab726f94fc9e93af1445dd813cee5f505cb8267e3
fill_id: db7fb181-3826-44da-98d0-f4ba5b050842
published_at: '2026-10-23T11:28:41.313650'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Build a bill-sharing app with OpenCode 2.0's new features—cross-platform sessions, background agents, code mode, work trees, plugins, and free or local models—without spending a cent.

## Prerequisites

### OpenCode installed
- **Kind**: tool
- **Note**: Install via curl on Linux/Mac or npm on Windows; also available as a desktop app for Mac, Windows, Linux.

### OpenCode account
- **Kind**: account
- **Note**: Required for free models; log in via Google or email to get API keys.

## Steps

### Upgrade to OpenCode 2.0
- **Timestamp**: [00:00](https://www.youtube.com/watch?v=OyuId4YQiIs&t=0)
- **Action**: If already using OpenCode, run the update command in the terminal, then click refresh and restart OpenCode. For new users, install via curl (Linux/Mac) or npm (Windows) from the OpenCode site.
- **Command Or Clicks**: /update
- **Choice Branch**: Alternatively, download the desktop app from the OpenCode site for Mac, Windows, or Linux.

### Create a project folder and start OpenCode
- **Timestamp**: [01:59](https://www.youtube.com/watch?v=OyuId4YQiIs&t=119)
- **Action**: Create a new folder for your project, open a command prompt in that folder, and run `opencode` to ensure all agent-created files stay in that folder. In the desktop app, use the drop-down menu to add a project and select the folder.
- **Command Or Clicks**: mkdir bill-splitter && cd bill-splitter && opencode
- **Choice Branch**: Desktop app: click drop-down at bottom, 'Add project', select folder.

### Choose a free model and start a session
- **Timestamp**: [03:39](https://www.youtube.com/watch?v=OyuId4YQiIs&t=219)
- **Action**: Run `/models` to see available vendors. Select a free template like 'Beam'. Then prompt the agent to create a simple bill-sharing app that runs in the browser.
- **Command Or Clicks**: /models
- **Choice Branch**: If API key expired, press Ctrl+A to connect integration, go to OpenCode console, add account, log in via Google or email.

### Verify cross-platform session continuity
- **Timestamp**: [04:34](https://www.youtube.com/watch?v=OyuId4YQiIs&t=274)
- **Action**: Switch to the desktop app and see the same session started in the terminal. Ask the agent to start the development server and provide a link.
- **Command Or Clicks**: Please, can you start the development server? Give me the link.
- **Choice Branch**: None

### Move tasks to background
- **Timestamp**: [05:27](https://www.youtube.com/watch?v=OyuId4YQiIs&t=327)
- **Action**: Press Ctrl+B or click the background button to move a blocking task to the background, allowing continued interaction with the agent. Click the provided link to access the app.
- **Command Or Clicks**: Ctrl+B
- **Choice Branch**: None

### Create a background subagent
- **Timestamp**: [06:28](https://www.youtube.com/watch?v=OyuId4YQiIs&t=388)
- **Action**: Ask the main agent to create a background verification agent using a different model like 'Big Pickle'. View subagent details in the side panel and see the same session in terminal or mobile.
- **Command Or Clicks**: Create a background verification agent using Big Pickle.
- **Choice Branch**: None

### Use code mode for efficient tool execution
- **Timestamp**: [08:13](https://www.youtube.com/watch?v=OyuId4YQiIs&t=493)
- **Action**: Code mode is enabled by default; force it with a prompt like 'Use code mode to do the following...'. It runs multiple tool calls in a script, reducing context window overload. Look for execution steps calling tools.opencode.something.
- **Command Or Clicks**: Use code mode to do the following. Get documentation for Playwright MCP at this URL. Please install MCP locally. Use MCP to open our application.
- **Choice Branch**: None

### Apply changes in a work tree
- **Timestamp**: [09:19](https://www.youtube.com/watch?v=OyuId4YQiIs&t=559)
- **Action**: Ask the agent to use a work tree to add light/dark theme support. The agent creates a physical copy of the codebase, makes changes there, and you can merge back to master when satisfied.
- **Command Or Clicks**: Please use the work tree to add support for light and dark themes.
- **Choice Branch**: After merging, say: 'Please push all the changes to the master branch and delete the working tree.'

### Create a plugin to protect .env files
- **Timestamp**: [10:33](https://www.youtube.com/watch?v=OyuId4YQiIs&t=633)
- **Action**: Ask the agent to write a plugin that prevents reading .env files. The plugin is a simple TypeScript file. List plugins with `opencode plugin list`. Test by asking the agent to read .env; it will require permission.
- **Command Or Clicks**: Write a plugin that will prevent you from ever reading .env files.
- **Choice Branch**: Run `opencode plugin list` to see configured plugins.

### Run local models with Ollama
- **Timestamp**: [12:27](https://www.youtube.com/watch?v=OyuId4YQiIs&t=747)
- **Action**: Install Ollama from ollama.com, choose a model like qwen3:8b (requires ~16GB VRAM), pull it with `ollama pull`, then in OpenCode enable Ollama and select the model. Test with a simple query.
- **Command Or Clicks**: ollama pull qwen3:8b
- **Choice Branch**: Ask your coding agent to analyze hardware and recommend a model.

## Gotchas

### Free models may use your queries for training; for professional work, use paid services or local models.
- **Severity**: serious
- **Timestamp**: [04:34](https://www.youtube.com/watch?v=OyuId4YQiIs&t=274)

### Running OpenCode in the root directory can scatter files; always create a project folder.
- **Severity**: heads_up
- **Timestamp**: [01:59](https://www.youtube.com/watch?v=OyuId4YQiIs&t=119)

### You cannot send messages directly to subagents; you can only view their output.
- **Severity**: heads_up
- **Timestamp**: [07:16](https://www.youtube.com/watch?v=OyuId4YQiIs&t=436)

## Where to go next

Explore more OpenCode features like custom plugins and local models. Check the free course link in the description to master agent-based coding.

## Concepts surfaced

[[background-agents]] · [[code-mode]] · [[work-trees]] · [[plugins]] · [[local-models]] · [[cross-platform-sessions]]
