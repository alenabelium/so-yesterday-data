---
video_id: N7Hkqznvc7I
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-08-31-qwen-38-deepseek-harness-is-my-new-free-claude-code.md
source_transcript: ../transcripts/2026-08-31-qwen-38-deepseek-harness-is-my-new-free-claude-code.md
source_summary_hash: sha256:7ab0528020d64719e8be19dd7fac684ab753aa13b9945efafe0a3dcd23db59c9
source_transcript_hash: sha256:bfad5c53676aed932d27fe1887b47944dfb58b80c1c1a6daba0214d0e20a8f89
fill_id: 43592365-469d-4d74-bf3f-7e45a94ca6d5
published_at: '2026-09-29T11:23:31.674144'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Set up DeepSeek Harness, connect local models via Ollama, and build custom plugins for a free Claude Code alternative.

## Prerequisites

### Node.js Environment
- **Kind**: tool
- **Note**: Required to run the npx installer command.

### Ollama or LM Studio
- **Kind**: tool
- **Note**: Needed to host local LLMs like Qwen 3.8 for offline use.

### 16GB VRAM
- **Kind**: hardware
- **Note**: Minimum hardware requirement to run the Qwen 3.8 model locally.

## Steps

### Install DeepSeek Harness
- **Timestamp**: [01:22](https://www.youtube.com/watch?v=N7Hkqznvc7I&t=82)
- **Action**: Copy the npx command from the GitHub repository run section and paste it into your terminal to install the harness.
- **Command Or Clicks**: npx deepseek-harness@latest
- **Choice Branch**: If npx fails, use npm install -g deepseek-harness@latest.

### Launch and Configure API Key
- **Timestamp**: [02:29](https://www.youtube.com/watch?v=N7Hkqznvc7I&t=149)
- **Action**: Run the web command to start the UI. If using DeepSeek's cloud model, create an API key on their platform and paste it into the prompt.
- **Command Or Clicks**: dsh web
- **Choice Branch**: API key is optional if using other providers or local models.

### Create Local Model Preset
- **Timestamp**: [09:29](https://www.youtube.com/watch?v=N7Hkqznvc7I&t=569)
- **Action**: Use Creator Mode to ask the agent to create a preset that disables heavy tools like sub-agents and RALF loop for local model efficiency.
- **Command Or Clicks**: Please create a new agent preset called local models. For this preset disable the Ralph plugin and the sub aents plugins.
- **Choice Branch**: Use Creator Mode to bypass standard capabilities.

### Install Ollama and Model
- **Timestamp**: [10:24](https://www.youtube.com/watch?v=N7Hkqznvc7I&t=624)
- **Action**: Download Ollama, then pull the Qwen 3.8 model using the command line.
- **Command Or Clicks**: ollama pull qwen3.8
- **Choice Branch**: Ensure you have ~16GB VRAM for this model.

### Add Ollama as Provider
- **Timestamp**: [11:16](https://www.youtube.com/watch?v=N7Hkqznvc7I&t=676)
- **Action**: In Settings > Models, add a custom provider named 'Llama' with base URL localhost:11434/v1 and API key 'ollama'.
- **Command Or Clicks**: Base URL: http://localhost:11434/v1 | API Key: ollama
- **Choice Branch**: Select OpenAI completions protocol.

### Install External Plugin
- **Timestamp**: [12:35](https://www.youtube.com/watch?v=N7Hkqznvc7I&t=755)
- **Action**: Navigate to the plugin folder in terminal and run the profile command to install a downloaded plugin.
- **Command Or Clicks**: deepseek harness plugin profile web add <plugin-name>
- **Choice Branch**: Restart DSH web after installation.

### Create Dynamic Plugin
- **Timestamp**: [14:29](https://www.youtube.com/watch?v=N7Hkqznvc7I&t=869)
- **Action**: In Creator Mode, ask the agent to create a plugin (e.g., confetti effect) and approve the installation prompt.
- **Command Or Clicks**: Please create a new plug-in that will shoot confetti all over the screen whenever the user clicks the new session button.
- **Choice Branch**: Test in the 'cordis plugin' sidebar before finalizing.

### Finalize and Distribute Plugin
- **Timestamp**: [15:34](https://www.youtube.com/watch?v=N7Hkqznvc7I&t=934)
- **Action**: Ask the agent to create a permanent plugin file, then share the resulting folder with others for installation.
- **Command Or Clicks**: Please create a permanent plugin that I can distribute using the [installation command].
- **Choice Branch**: Share the folder contents for others to install.

## Gotchas

### Dynamic plugins created in memory are lost if you close DeepSeek Harness. You must ask the agent to create a permanent plugin file.
- **Severity**: blocking
- **Timestamp**: [15:34](https://www.youtube.com/watch?v=N7Hkqznvc7I&t=934)

### Local models struggle with complex tools like sub-agents and RALF loops. Disable these in your preset to avoid context bloat.
- **Severity**: serious
- **Timestamp**: [09:29](https://www.youtube.com/watch?v=N7Hkqznvc7I&t=569)

## Where to go next

Explore the [deepseek-harness] GitHub repo for more plugins and presets. Check out the [cordis] framework docs to understand the underlying plugin architecture.

## Concepts surfaced

[[deepseek-harness]] · [[ollama]] · [[local-llm]] · [[plugin-architecture]] · [[cordis-framework]] · [[agent-presets]]
