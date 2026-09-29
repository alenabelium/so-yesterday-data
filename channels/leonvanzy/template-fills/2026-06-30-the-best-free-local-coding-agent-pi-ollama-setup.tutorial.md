---
video_id: cUwH8wxYDx8
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-06-30-the-best-free-local-coding-agent-pi-ollama-setup.md
source_transcript: ../transcripts/2026-06-30-the-best-free-local-coding-agent-pi-ollama-setup.md
source_summary_hash: sha256:657e67f0e1859c7e7e8fb4cba004810220678e3452926170715f29f940bd556a
source_transcript_hash: sha256:ea7bafeb2392e12140b4e2abb596940b35cd43bb8bf9a6e5ddd3779f6384d22e
fill_id: bb11237c-4979-48ba-831c-c7e19b633175
published_at: '2026-09-29T11:06:28.385783'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Use the lean Pi Agent SDK with Ollama to run free local coding models without context window bloat, enabling reliable software generation.

## Prerequisites

### Pi Agent SDK
- **Kind**: tool
- **Note**: Install via npm from pi.dev to get the lean harness.

### Ollama
- **Kind**: tool
- **Note**: Download and install from ollama.com to run local models.

### Qwen 3.6 Model
- **Kind**: tool
- **Note**: Pull via Ollama; requires 16GB-24GB VRAM depending on parameter size.

### VS Code
- **Kind**: tool
- **Note**: Required to edit the models.json configuration file.

## Steps

### Install Pi Agent SDK
- **Timestamp**: [02:28](https://www.youtube.com/watch?v=cUwH8wxYDx8&t=148)
- **Action**: Navigate to pi.dev, copy the npm install command, and run it in your terminal.
- **Command Or Clicks**: npm install -g @pi-agent/sdk

### Install and Verify Ollama
- **Timestamp**: [03:15](https://www.youtube.com/watch?v=cUwH8wxYDx8&t=195)
- **Action**: Download Ollama from ollama.com, install it, and verify the installation via terminal.
- **Command Or Clicks**: ollama serve

### Download Qwen 3.6 Model
- **Timestamp**: [04:00](https://www.youtube.com/watch?v=cUwH8wxYDx8&t=240)
- **Action**: Pull the Qwen 3.6 model using Ollama and test it with a simple greeting.
- **Command Or Clicks**: ollama pull qwen3.6 && ollama run qwen3.6

### Configure Pi to Use Local Model
- **Timestamp**: [05:39](https://www.youtube.com/watch?v=cUwH8wxYDx8&t=339)
- **Action**: Create or edit the models.json file in the .pi/agent folder to register the Ollama model.
- **Command Or Clicks**: Create .pi/agent/models.json with Ollama config entry

### Set Up Project Memory and Design
- **Timestamp**: [06:30](https://www.youtube.com/watch?v=cUwH8wxYDx8&t=390)
- **Action**: Create an agents.md file for rules and a design.md file for design system details.
- **Command Or Clicks**: Create agents.md and design.md in project root

### Generate Implementation Plan
- **Timestamp**: [12:22](https://www.youtube.com/watch?v=cUwH8wxYDx8&t=742)
- **Action**: Use a cloud LLM to generate a detailed markdown implementation plan for the website.
- **Command Or Clicks**: Prompt LLM: 'Create detailed implementation plan...'

### Split Plan into Features
- **Timestamp**: [14:08](https://www.youtube.com/watch?v=cUwH8wxYDx8&t=848)
- **Action**: Ask the local agent to split the large plan file into individual feature files.
- **Command Or Clicks**: Prompt agent: 'Split this large implementation file up...'

### Implement Features Sequentially
- **Timestamp**: [15:00](https://www.youtube.com/watch?v=cUwH8wxYDx8&t=900)
- **Action**: Clear context, pull one feature file, and ask the agent to implement it.
- **Command Or Clicks**: Slash new, pull feature file, prompt agent

### Deploy to Hostinger
- **Timestamp**: [17:49](https://www.youtube.com/watch?v=cUwH8wxYDx8&t=1069)
- **Action**: Create a zip of the public_html folder and migrate it via Hostinger's dashboard.
- **Command Or Clicks**: Hostinger Dashboard > Websites > Migrate Website > Upload zip

## Gotchas

### Bloated harnesses like Claude Code consume 20k+ tokens instantly, pushing local models into the 'dumb zone' where intelligence degrades.
- **Severity**: blocking
- **Timestamp**: [00:54](https://www.youtube.com/watch?v=cUwH8wxYDx8&t=54)

### Large implementation plans will exceed the context window if pasted directly; always split them into smaller feature files first.
- **Severity**: blocking
- **Timestamp**: [14:08](https://www.youtube.com/watch?v=cUwH8wxYDx8&t=848)

### Local models lack creativity for design systems; use external tools like Google Stitch or Dribbble to generate design assets.
- **Severity**: heads_up
- **Timestamp**: [09:59](https://www.youtube.com/watch?v=cUwH8wxYDx8&t=599)

## Where to go next

Explore the Pi Agent SDK plugin marketplace to add MCP servers or web search capabilities to your lean harness.

## Concepts surfaced

[[lean-harness]] · [[local-llm]] · [[context-window-management]] · [[ollama-setup]] · [[pi-agent-sdk]] · [[static-site-deployment]]
