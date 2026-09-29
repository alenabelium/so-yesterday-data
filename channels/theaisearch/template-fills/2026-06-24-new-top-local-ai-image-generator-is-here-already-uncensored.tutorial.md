---
video_id: 1U8dJ94QFNc
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-06-24-new-top-local-ai-image-generator-is-here-already-uncensored.md
source_transcript: ../transcripts/2026-06-24-new-top-local-ai-image-generator-is-here-already-uncensored.md
source_summary_hash: sha256:251797ff750d25e29e86849480e8235de352712f95ad6b7aa88e3586858c3189
source_transcript_hash: sha256:1d5fd7095f0755c14b1b07e16e1650461edac138f5202274109725b089fef32d
fill_id: 4d9379e6-539a-477b-b6e4-90a85e4d0376
published_at: '2026-09-29T11:05:58.206809'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Install and run the uncensored Crea 2 local AI image generator in Comfy UI with low VRAM requirements.

## Prerequisites

### Comfy UI
- **Kind**: tool
- **Note**: Latest version installed on Windows portable or other OS.

### Consumer GPU
- **Kind**: hardware
- **Note**: Minimum 8 GB VRAM recommended for running the model.

### HuggingFace Account
- **Kind**: account
- **Note**: Needed to download the Crea 2 model files and LoRAs.

## Steps

### Update Comfy UI
- **Timestamp**: [02:01](https://www.youtube.com/watch?v=1U8dJ94QFNc&t=121)
- **Action**: Open the Comfy UI root folder and run the update script to ensure you have the latest version.
- **Command Or Clicks**: Double click on update Comfy.bat
- **Choice Branch**: Wait for 'press any key to continue' then press any key.

### Load Crea 2 Workflow
- **Timestamp**: [03:30](https://www.youtube.com/watch?v=1U8dJ94QFNc&t=210)
- **Action**: Open Comfy UI, navigate to templates, and load the offline Korea text to image workflow.
- **Command Or Clicks**: Sidebar > Templates > Search 'Korea' > Click 'Korea text to image' (offline)
- **Choice Branch**: Ensure you select the offline version, not the API version.

### Download Crea 2 Model
- **Timestamp**: [04:00](https://www.youtube.com/watch?v=1U8dJ94QFNc&t=240)
- **Action**: Download the Crea 2 Turbo FP8 model file and place it in the correct directory.
- **Command Or Clicks**: Download link > Save to Comfy UI/models/diffusion_models
- **Choice Branch**: Choose FP8 for lower VRAM usage or BF16 for full quality.

### Download Text Encoder
- **Timestamp**: [04:40](https://www.youtube.com/watch?v=1U8dJ94QFNc&t=280)
- **Action**: Download the Qwen2VL text encoder and place it in the text encoders folder.
- **Command Or Clicks**: Download link > Save to Comfy UI/models/text_encoders
- **Choice Branch**: File size is approximately 4.8 GB.

### Download VAE
- **Timestamp**: [05:00](https://www.youtube.com/watch?v=1U8dJ94QFNc&t=300)
- **Action**: Download the VAE file and place it in the VAE folder.
- **Command Or Clicks**: Download link > Save to Comfy UI/models/VAE
- **Choice Branch**: File size is approximately 250 MB.

### Configure Workflow Nodes
- **Timestamp**: [05:16](https://www.youtube.com/watch?v=1U8dJ94QFNc&t=316)
- **Action**: Refresh the model list and select the downloaded models in the workflow dropdowns.
- **Command Or Clicks**: Press 'R' to refresh > Select Crea 2 model, Qwen2VL4B clip, Quinn image VAE
- **Choice Branch**: Set 'enable lora' to false initially.

### Generate Image
- **Timestamp**: [06:13](https://www.youtube.com/watch?v=1U8dJ94QFNc&t=373)
- **Action**: Enter a prompt and run the generation to test the setup.
- **Command Or Clicks**: Enter prompt > Click 'Run'
- **Choice Branch**: Use 8 steps for turbo models; adjust CFG for creativity vs literalism.

### Install Uncensored Node
- **Timestamp**: [12:00](https://www.youtube.com/watch?v=1U8dJ94QFNc&t=720)
- **Action**: Clone the custom conditioning node to enable uncensored generation capabilities.
- **Command Or Clicks**: cmd > cd custom_nodes > git clone [link]
- **Choice Branch**: Restart Comfy UI after cloning.

### Connect Rebalance Node
- **Timestamp**: [13:30](https://www.youtube.com/watch?v=1U8dJ94QFNc&t=810)
- **Action**: Add the Conditioning Crea 2 Rebalance node between the prompt and K sampler.
- **Command Or Clicks**: Search 'create 2' > Drag node > Connect prompt to positive input
- **Choice Branch**: This tweak is required for robust uncensored output.

## Gotchas

### Using the API template instead of the offline one will prevent local execution.
- **Severity**: blocking
- **Timestamp**: [03:30](https://www.youtube.com/watch?v=1U8dJ94QFNc&t=210)

### Synthetic data in training biases the model and reduces aesthetic quality.
- **Severity**: serious
- **Timestamp**: [17:18](https://www.youtube.com/watch?v=1U8dJ94QFNc&t=1038)

### LoRAs require specific trigger words in the prompt to activate correctly.
- **Severity**: heads_up
- **Timestamp**: [12:55](https://www.youtube.com/watch?v=1U8dJ94QFNc&t=775)

## Where to go next

Explore the official Comfy UI Crea 2 folder on HuggingFace for community LoRAs and technical reports on training methodology.

## Concepts surfaced

[[local-ai-generation]] · [[comfy-ui-workflow]] · [[uncensored-ai-models]] · [[low-vram-optimization]] · [[synthetic-data-bias]] · [[community-loras]]
