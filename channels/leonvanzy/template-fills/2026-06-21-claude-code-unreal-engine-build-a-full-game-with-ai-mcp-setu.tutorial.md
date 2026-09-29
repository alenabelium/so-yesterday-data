---
video_id: v-6KM2ysQYo
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-06-21-claude-code-unreal-engine-build-a-full-game-with-ai-mcp-setu.md
source_transcript: ../transcripts/2026-06-21-claude-code-unreal-engine-build-a-full-game-with-ai-mcp-setu.md
source_summary_hash: sha256:35293fb9cfe78e17fd6439c2ef48d9af360405a4a8a79d71e641c7203a5293f5
source_transcript_hash: sha256:a654901bce001c4fb6e2a14b5b453cfd7cde360a66b838ea632e95f08aaa6288
fill_id: fd132ee1-aebf-45c4-a4c0-cfa866cc066c
published_at: '2026-09-29T11:05:44.078613'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Non-developers can build GTA-style game prototypes in hours by combining Claude Code with Unreal Engine's MCP server for agentic asset management and scene editing.

## Prerequisites

### Unreal Engine 5.8+
- **Kind**: tool
- **Note**: Latest version required for MCP server compatibility.

### Claude Code
- **Kind**: tool
- **Note**: Coding agent installed via OS-specific terminal command.

### Basic Terminal Knowledge
- **Kind**: knowledge
- **Note**: Ability to run copy-pasted CLI commands for setup.

## Steps

### Install Unreal Engine and Claude Code
- **Timestamp**: [00:30](https://www.youtube.com/watch?v=v-6KM2ysQYo&t=30)
- **Action**: Download and install the Unreal Engine launcher (version 5.8+) and install Claude Code using the provided terminal command for your OS.
- **Command Or Clicks**: Copy and run the installation command from the video description for your OS (Mac/Linux/WSL/PowerShell).
- **Choice Branch**: You can use other agents like CodeEx, but Claude Code is used in this tutorial.

### Create Project and Enable MCP Plugin
- **Timestamp**: [02:15](https://www.youtube.com/watch?v=v-6KM2ysQYo&t=135)
- **Action**: Launch Unreal Engine, create a new Blank project named 'MCP test', navigate to Edit > Plugins, search for 'Unreal MCP', enable it, and restart the editor.
- **Command Or Clicks**: Edit > Plugins > Search 'Unreal MCP' > Enable > Restart Editor
- **Choice Branch**: Ensure you restart the editor after enabling the plugin.

### Configure MCP Server Settings
- **Timestamp**: [03:00](https://www.youtube.com/watch?v=v-6KM2ysQYo&t=180)
- **Action**: Go to Edit > Editor Preferences > Model Context Protocol and enable the 'Auto start MCP server' checkbox.
- **Command Or Clicks**: Edit > Editor Preferences > Model Context Protocol > Check 'Auto start MCP server'
- **Choice Branch**: None

### Initialize MCP Connection via Console
- **Timestamp**: [03:30](https://www.youtube.com/watch?v=v-6KM2ysQYo&t=210)
- **Action**: Press tilde (~) to open the console, paste the MCP initialization command provided by the documentation, and press Enter to generate the mcp.json file.
- **Command Or Clicks**: Press ~ > Paste MCP command > Enter
- **Choice Branch**: Save the project (Ctrl+S) before closing Unreal to ensure settings take effect.

### Verify MCP Status in Claude Code
- **Timestamp**: [04:45](https://www.youtube.com/watch?v=v-6KM2ysQYo&t=285)
- **Action**: Restart Unreal Engine, open a terminal, start Claude Code, set the model to opus 4.8, set effort to extra high, and run /mcp to verify the Unreal MCP connection is authenticated.
- **Command Or Clicks**: /model opus 4.8 /effort extra-high /mcp
- **Choice Branch**: Ensure the tick mark appears next to Unreal MCP.

### Enable Required Plugins for Tool Access
- **Timestamp**: [06:00](https://www.youtube.com/watch?v=v-6KM2ysQYo&t=360)
- **Action**: Enable 'Python editor script plugin', 'Python foundation packages plugin', and 'Editor Toolset Registry' in the plugins menu, then restart Unreal Engine.
- **Command Or Clicks**: Edit > Plugins > Enable Python Editor Script, Python Foundation, Editor Toolset Registry > Restart
- **Choice Branch**: This step is critical for the agent to interact with actors and blueprints.

### Refresh Tools and Test Scene Interaction
- **Timestamp**: [06:45](https://www.youtube.com/watch?v=v-6KM2ysQYo&t=405)
- **Action**: Open the console again, paste the refresh command, restart Claude Code, and ask Claude to add a cube to verify the 'scenes' tool is active.
- **Command Or Clicks**: Press ~ > Paste refresh command > Enter > Restart Claude Code
- **Choice Branch**: Use Alt+V to paste screenshots if the agent cannot see the scene correctly.

### Plan Game Mechanics in Planning Mode
- **Timestamp**: [09:15](https://www.youtube.com/watch?v=v-6KM2ysQYo&t=555)
- **Action**: Switch Claude Code to planning mode, ask it to research GTA-style mechanics, and define a vertical slice scope (e.g., getaway car, wanted levels, character switching).
- **Command Or Clicks**: Switch to Planning Mode > Prompt: 'Research GTA mechanics and create a vertical slice plan'
- **Choice Branch**: Specify 'sunset neon' mood and 'new dedicated level' for the build.

### Import Assets via Feature Packs
- **Timestamp**: [11:30](https://www.youtube.com/watch?v=v-6KM2ysQYo&t=690)
- **Action**: Open the Content Drawer, click the green Add button, select 'Add Feature or Content Pack', and add the 'Third Person' and 'Vehicle' packs bundled with the engine.
- **Command Or Clicks**: Content Drawer > Green Add Button > Add Feature or Content Pack > Third Person/Vehicle
- **Choice Branch**: Use Fab to find additional free assets like palm trees if default assets look poor.

### Execute Build and Wrap Up
- **Timestamp**: [13:30](https://www.youtube.com/watch?v=v-6KM2ysQYo&t=810)
- **Action**: Allow Claude to implement the plan, then use the 'ultra code' keyword to trigger a workflow that wraps up remaining tasks like vehicle physics and NPC AI.
- **Command Or Clicks**: Prompt: 'Use a workflow to wrap up this game' (triggering ultra code mode)
- **Choice Branch**: Monitor progress; the agent works synchronously, so patience is required.

## Gotchas

### Incompatible asset packs can crash the engine. Always check compatibility version and filter for free products in Fab.
- **Severity**: serious
- **Timestamp**: [15:00](https://www.youtube.com/watch?v=v-6KM2ysQYo&t=900)

### The MCP server is new and currently synchronous; you cannot have multiple agents edit the scene simultaneously yet.
- **Severity**: heads_up
- **Timestamp**: [16:30](https://www.youtube.com/watch?v=v-6KM2ysQYo&t=990)

### Default assets may look poor. You must manually download higher-quality free packs from Fab for better visuals.
- **Severity**: heads_up
- **Timestamp**: [15:30](https://www.youtube.com/watch?v=v-6KM2ysQYo&t=930)

## Where to go next

Explore Epic's built-in feature packs for quick prototyping. For advanced visuals, use Fab to filter free assets by compatibility. Check the community resources for the full game build and the custom song used in the trailer.

## Concepts surfaced

[[agentic-coding]] · [[unreal-engine-mcp]] · [[claude-code-setup]] · [[game-prototyping]] · [[asset-management]] · [[planning-mode-workflow]]
