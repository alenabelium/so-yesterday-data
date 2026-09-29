---
video_id: vr_iCHPY8yI
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-09-16-i-let-ai-take-over-blender.md
source_transcript: ../transcripts/2026-09-16-i-let-ai-take-over-blender.md
source_summary_hash: sha256:145b51356c148a28574c75de7b8a95d86a9d365c502d93a9c8192559dfc23f62
source_transcript_hash: sha256:d2d369818c8be1676e12f3b432447e5b37cd0cf746247919c66695a1eab08685
fill_id: a3ac6542-e792-44d5-8e25-fd7fff23674c
published_at: '2026-09-29T11:24:42.174455'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Connect AI agents to Blender via MCP to autonomously create, animate, and export interactive 3D assets.

## Prerequisites

### AI Assistant with Computer Use
- **Kind**: account
- **Note**: ChatGPT desktop app (GPT-6 Astra) or Claude desktop app (Claude 5.1) with 'Computer Use' enabled in settings.

### Blender
- **Kind**: tool
- **Note**: Latest version installed from blender.org to support the official MCP server protocol.

## Steps

### Enable Computer Use in AI App
- **Timestamp**: [02:23](https://www.youtube.com/watch?v=vr_iCHPY8yI&t=143)
- **Action**: Open your AI assistant's profile settings, navigate to the 'Computer Use' section, and ensure the toggle is enabled so the agent can control Blender.
- **Command Or Clicks**: Profile Settings > Computer Use > Enable Toggle
- **Choice Branch**: Ensure you are using a model with strong 3D spatial understanding like GPT-6 Astra.

### Configure Blender MCP Server
- **Timestamp**: [02:55](https://www.youtube.com/watch?v=vr_iCHPY8yI&t=175)
- **Action**: Ask the AI agent to set up the Blender MCP server by providing it with the official setup article URL. The agent will read the instructions and configure the connection automatically.
- **Command Or Clicks**: Chat Input: 'Please set up the blender MCP server as per this [URL] and connect it to the chat GPT app using computer use'
- **Choice Branch**: Wait for the agent to complete the setup; you may need to restart the desktop app if the plugin doesn't appear immediately.

### Verify Plugin Connection
- **Timestamp**: [03:58](https://www.youtube.com/watch?v=vr_iCHPY8yI&t=238)
- **Action**: Check the AI app's settings under Plugins > MCP to confirm the Blender plugin is listed and enabled. Create a new chat session if necessary.
- **Command Or Clicks**: Settings > Plugins > MCP > Verify Blender Plugin Status
- **Choice Branch**: If the plugin isn't visible, restart the desktop app or create a new chat window.

### Generate 3D Asset via Prompt
- **Timestamp**: [06:42](https://www.youtube.com/watch?v=vr_iCHPY8yI&t=402)
- **Action**: Instruct the agent to create a specific 3D model using the Blender MCP tools. The agent will open Blender and generate the geometry based on your description.
- **Command Or Clicks**: Chat Input: 'Use the Blender MCP to create a 3D donut with pink frosting and sprinkles'
- **Choice Branch**: Allow a few minutes for the agent to process the request and render the initial model.

### Request Animations and Sound
- **Timestamp**: [08:05](https://www.youtube.com/watch?v=vr_iCHPY8yI&t=485)
- **Action**: Ask the agent to animate the asset, specifying physics behaviors like dropping or wobbling. The agent can also find and sync audio files for sound effects.
- **Command Or Clicks**: Chat Input: 'Create an animation for the donut. Drop it onto the plate with a wobble effect.'
- **Choice Branch**: The agent may take screenshots to test the animation loop before finalizing.

### Export Interactive Web Experience
- **Timestamp**: [09:54](https://www.youtube.com/watch?v=vr_iCHPY8yI&t=594)
- **Action**: Ask the agent to generate an index.html file that embeds the 3D asset, allowing users to rotate, zoom, and play animations in a browser.
- **Command Or Clicks**: Chat Input: 'Create an index.html file with this 3D asset. Users should be able to interact with it like rotate the scene.'
- **Choice Branch**: The agent will test the export in its integrated browser and self-correct alignment issues automatically.

## Gotchas

### You must use the latest version of Blender to ensure compatibility with the official MCP server protocol.
- **Severity**: blocking
- **Timestamp**: [02:23](https://www.youtube.com/watch?v=vr_iCHPY8yI&t=143)

### Standard web versions of ChatGPT or Claude lack 'Computer Use' capabilities; you must use the desktop apps to control Blender locally.
- **Severity**: serious
- **Timestamp**: [00:57](https://www.youtube.com/watch?v=vr_iCHPY8yI&t=57)

### The AI agent may not see the plugin immediately after setup; restarting the app or creating a new chat is often required.
- **Severity**: heads_up
- **Timestamp**: [03:58](https://www.youtube.com/watch?v=vr_iCHPY8yI&t=238)

## Where to go next

Explore Agentic Labs for coding agent fundamentals, including payment integration and user authentication tutorials. Try the Crisp voice isolation tool for cleaner audio inputs in future AI projects.

## Concepts surfaced

[[blender-mcp-server]] · [[ai-computer-use]] · [[autonomous-3d-modeling]] · [[interactive-web-assets]]
