---
video_id: L_AMm7fD7tQ
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-05-06-no-claude-code-no-codex-just-local-ai-agents.md
source_transcript: ../transcripts/2026-05-06-no-claude-code-no-codex-just-local-ai-agents.md
source_summary_hash: sha256:48468c00664ce2a20a90699af44925a4b3c2018bfecfabb9ba74664a4dcd3f17
source_transcript_hash: sha256:a16b003ffd76b57ae2e88814afc7022a8e8eebbb6ae0b200d664d59e46385cfd
fill_id: fadb27b1-7038-4775-8c6b-4d938962e32b
published_at: '2026-05-31T07:55:27.533556'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Build autonomous coding agents locally with free open-source models like Qwen 3.6 and LM Studio, eliminating expensive frontier model costs.

## Prerequisites

### LM Studio
- **Kind**: tool
- **Note**: Download and install from lmstudio.ai for model inference.

### Qwen 3.6 35B
- **Kind**: tool
- **Note**: Recommended 35B parameter model for tool calling and coding.

### Node.js
- **Kind**: tool
- **Note**: Required dependency for running Local Forge.

### Git
- **Kind**: tool
- **Note**: Needed to clone the Local Forge repository.

### RTX 4070 GPU
- **Kind**: hardware
- **Note**: Tested hardware; consumer-grade GPU required for performance.

## Steps

### Download and load Qwen 3.6 in LM Studio
- **Timestamp**: [04:17](https://www.youtube.com/watch?v=L_AMm7fD7tQ&t=257)
- **Action**: Install LM Studio, search for Qwen 3.6 35B, download it, and increase the context length to at least 64,000 tokens.
- **Command Or Clicks**: Click model search, type 'qwen 3.6', click download, go to settings, set context length to 128,000, click load model.
- **Choice Branch**: Use LM Studio instead of Llama CLI to avoid CPU-only bugs.

### Install Local Forge dependencies
- **Timestamp**: [06:30](https://www.youtube.com/watch?v=L_AMm7fD7tQ&t=390)
- **Action**: Clone the Local Forge repository and install Node.js.
- **Command Or Clicks**: git clone <repo-url> && npm install
- **Choice Branch**: Download zip file if Git is not available.

### Start Local Forge server
- **Timestamp**: [07:00](https://www.youtube.com/watch?v=L_AMm7fD7tQ&t=420)
- **Action**: Run the start script to launch the Local Forge interface.
- **Command Or Clicks**: start.bat (Windows) or start.sh (Linux/Mac)
- **Choice Branch**: Wait for dependencies to install before accessing the URL.

### Configure Local Forge settings
- **Timestamp**: [07:19](https://www.youtube.com/watch?v=L_AMm7fD7tQ&t=439)
- **Action**: Set LM Studio as the provider, select Qwen 3.6, and enable Playwright for browser testing.
- **Command Or Clicks**: Click settings cog, select provider 'LM Studio', select model 'Qwen 3.6', enable Playwright, set headed mode.
- **Choice Branch**: Set concurrency to 1 agent to manage hardware load.

### Create project via AI description
- **Timestamp**: [11:00](https://www.youtube.com/watch?v=L_AMm7fD7tQ&t=660)
- **Action**: Use the 'Describe your project to AI' feature to generate a detailed feature backlog.
- **Command Or Clicks**: Click 'describe your project to AI', type prompt, click 'create', click 'generate feature list'.
- **Choice Branch**: Manually add features if AI planning is insufficient.

### Run the coding queue
- **Timestamp**: [15:28](https://www.youtube.com/watch?v=L_AMm7fD7tQ&t=928)
- **Action**: Execute the queue to start the autonomous agent implementing the features.
- **Command Or Clicks**: Click 'run queue'.
- **Choice Branch**: Pause the model in LM Studio to stop execution.

## Gotchas

### Gemma 4 26B and smaller models are not good enough at tool calling; use the 31B+ version.
- **Severity**: blocking
- **Timestamp**: [02:10](https://www.youtube.com/watch?v=L_AMm7fD7tQ&t=130)

### LM Studio default context length is too small for coding models; increase to at least 64,000 tokens.
- **Severity**: blocking
- **Timestamp**: [05:29](https://www.youtube.com/watch?v=L_AMm7fD7tQ&t=329)

### Llama CLI may run models on CPU instead of GPU, causing slow performance.
- **Severity**: serious
- **Timestamp**: [04:17](https://www.youtube.com/watch?v=L_AMm7fD7tQ&t=257)

### Free models produce less detailed feature plans; consider using a paid model for planning only.
- **Severity**: heads_up
- **Timestamp**: [13:14](https://www.youtube.com/watch?v=L_AMm7fD7tQ&t=794)

## Where to go next

Explore the Local Forge GitHub repository for more configuration options and community contributions. Consider the presenter's agentic coding masterclass for advanced agent workflows.

## Concepts surfaced

[[local-ai-agents]] · [[open-source-models]] · [[lm-studio-setup]] · [[autonomous-coding]] · [[feature-backlog-generation]] · [[playwright-testing]]
