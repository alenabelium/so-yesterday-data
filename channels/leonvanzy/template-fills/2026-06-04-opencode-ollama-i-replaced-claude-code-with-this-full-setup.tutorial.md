---
video_id: 4r80bMX_kGg
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-06-04-opencode-ollama-i-replaced-claude-code-with-this-full-setup.md
source_transcript: ../transcripts/2026-06-04-opencode-ollama-i-replaced-claude-code-with-this-full-setup.md
source_summary_hash: sha256:d1749276a4f4ad13b3873caaa22865d817f53b965cc1548782cdb29ef2e73ffe
source_transcript_hash: sha256:cd6d01551af56238a5fa9c0d157aca984eac7d421ef81f3a7d63ef5b03c7deba
fill_id: 319bc3cc-cd00-4d6a-be00-b0c545c52619
published_at: '2026-06-10T10:45:26.469818'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Replace Claude Code with OpenCode and Ollama to run local models without system prompt overhead.

## Prerequisites

### Node.js
- **Kind**: tool
- **Note**: Required to install OpenCode via npm.

### Ollama
- **Kind**: tool
- **Note**: Local model runner installed from ollama.com.

### Compatible GPU
- **Kind**: hardware
- **Note**: 8GB+ VRAM recommended for local model inference.

## Steps

### Install OpenCode via npm
- **Timestamp**: [02:24](https://www.youtube.com/watch?v=4r80bMX_kGg&t=144)
- **Action**: Copy the npm install command from the NPM website and run it in your terminal to install OpenCode globally.
- **Command Or Clicks**: npm install -g open-code

### Install Ollama
- **Timestamp**: [01:45](https://www.youtube.com/watch?v=4r80bMX_kGg&t=105)
- **Action**: Navigate to the Ollama website, download the installer, and run it to enable local model hosting.
- **Command Or Clicks**: Download from ollama.com

### Pull a Local Model
- **Timestamp**: [02:24](https://www.youtube.com/watch?v=4r80bMX_kGg&t=144)
- **Action**: Select a model based on your VRAM (e.g., Code Llama 3.6 for 24GB+) and pull it using the terminal.
- **Command Or Clicks**: ollama pull codellama:3.6b
- **Choice Branch**: Use Gemma 4 for 8-12GB VRAM or Code Llama 3.6 for 24GB+.

### Connect OpenCode to Ollama
- **Timestamp**: [03:24](https://www.youtube.com/watch?v=4r80bMX_kGg&t=204)
- **Action**: Run the connect command in OpenCode, search for Ollama, and use 'Ollama' as the API key.
- **Command Or Clicks**: connect
- **Choice Branch**: If the model doesn't appear, edit the OpenCode config file in your user folder.

### Launch OpenCode with Model
- **Timestamp**: [04:13](https://www.youtube.com/watch?v=4r80bMX_kGg&t=253)
- **Action**: Start OpenCode in your project directory, explicitly specifying the local model to use.
- **Command Or Clicks**: open-code --model codellama:3.6b

### Scaffold Project and Plan
- **Timestamp**: [05:00](https://www.youtube.com/watch?v=4r80bMX_kGg&t=300)
- **Action**: Use OpenCode to scaffold a Next.js project, then switch to planning mode to generate a detailed implementation plan.
- **Command Or Clicks**: Please scaffold a Next.js project in this directory.
- **Choice Branch**: Hold Shift+Tab to switch between build and plan modes.

### Split Plan into Phases
- **Timestamp**: [06:00](https://www.youtube.com/watch?v=4r80bMX_kGg&t=360)
- **Action**: Interrupt the agent and ask it to split the plan into separate files in a tasks subfolder with actionable tasks.
- **Command Or Clicks**: Please split this plan into separate files in a tasks subfolder.
- **Choice Branch**: Keep instructions small and focused to avoid overwhelming the context window.

### Implement Phases Iteratively
- **Timestamp**: [07:05](https://www.youtube.com/watch?v=4r80bMX_kGg&t=425)
- **Action**: Create new sessions for each phase, pulling in the main file and the specific phase file to implement only that part.
- **Command Or Clicks**: Please go ahead and implement phase one only.
- **Choice Branch**: Implement phases sequentially to maintain context clarity.

### Debug with Browser Skill
- **Timestamp**: [09:12](https://www.youtube.com/watch?v=4r80bMX_kGg&t=552)
- **Action**: Install the agent browser skill to let the agent test the app and fix bugs autonomously.
- **Command Or Clicks**: Install agent browser skill and run skills command
- **Choice Branch**: Use headed mode to visualize the browser actions.

## Gotchas

### Claude Code uses ~30,000 tokens for system prompts, overwhelming local models. OpenCode has minimal overhead.
- **Severity**: serious
- **Timestamp**: [00:30](https://www.youtube.com/watch?v=4r80bMX_kGg&t=30)

### Avoid giving massive prompts or files to local agents; they may ignore instructions or hallucinate.
- **Severity**: blocking
- **Timestamp**: [06:30](https://www.youtube.com/watch?v=4r80bMX_kGg&t=390)

### Ensure your model is added to the OpenCode config file if it doesn't appear in the provider list.
- **Severity**: heads_up
- **Timestamp**: [03:50](https://www.youtube.com/watch?v=4r80bMX_kGg&t=230)

## Where to go next

Explore other open-weight models like Gemma 4 for lower VRAM setups. Check out the agent browser skill for autonomous debugging workflows.

## Concepts surfaced

[[local-ai]] · [[ollama]] · [[open-code]] · [[coding-agents]] · [[context-window-management]] · [[browser-automation]]
