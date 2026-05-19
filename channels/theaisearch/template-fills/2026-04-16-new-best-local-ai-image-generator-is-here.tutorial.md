---
video_id: A_nAU8h9YOY
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-04-16-new-best-local-ai-image-generator-is-here.md
source_transcript: ../transcripts/2026-04-16-new-best-local-ai-image-generator-is-here.md
source_summary_hash: sha256:01fe45c4bcbaa7929fb905abf0da694f569c9b923e538135bdc32633dc06a1bc
source_transcript_hash: sha256:e9ed65d8fddd8917a588fbf0567abdb0cd835153dcf6b40969ffc45ca50255a3
fill_id: 2a0746d1-47c3-476e-b79a-de9d1f630daa
published_at: '2026-05-19T04:50:23.124774'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Install Ernie Image, a top-tier open-source AI image generator, locally using ComfyUI for free, unlimited offline use with superior prompt adherence and text rendering.

## Prerequisites

### ComfyUI
- **Kind**: tool
- **Note**: Popular interface for running open-source image generators. Must be installed and updated to the latest version before proceeding.

### GPU with 20GB VRAM
- **Kind**: hardware
- **Note**: Required for standard operation. The base model and turbo model are ~16GB each, plus text encoder and VAE totaling ~20GB.

### Python Environment
- **Kind**: tool
- **Note**: Implicitly required to run the ComfyUI update and run batch files on Windows.

## Steps

### Update ComfyUI
- **Timestamp**: [15:06](https://www.youtube.com/watch?v=A_nAU8h9YOY&t=906)
- **Action**: Navigate to the ComfyUI installation folder, open the update directory, and run the update script to ensure you have the latest version.
- **Command Or Clicks**: Double click update Comfy.bat

### Launch ComfyUI
- **Timestamp**: [15:45](https://www.youtube.com/watch?v=A_nAU8h9YOY&t=945)
- **Action**: Start the ComfyUI application to access the web interface.
- **Command Or Clicks**: Double click run.bat

### Load Ernie Image Turbo Workflow
- **Timestamp**: [16:08](https://www.youtube.com/watch?v=A_nAU8h9YOY&t=968)
- **Action**: In the ComfyUI sidebar, click Templates, search for 'Ernie', and select the Ernie Image Turbo workflow for faster generation.
- **Command Or Clicks**: Click Templates > Search 'Ernie' > Select Ernie Image Turbo

### Download Required Models
- **Timestamp**: [16:30](https://www.youtube.com/watch?v=A_nAU8h9YOY&t=990)
- **Action**: Download the Ernie Image Turbo diffusion model, Minestral 3B text encoder, and Flux 2 VAE. Place them in the correct ComfyUI subdirectories.
- **Command Or Clicks**: Click download buttons in UI or manually place files: Ernie Turbo in comfy/models/diffusion_models, Minestral 3B in comfy/models/text_encoders, Flux 2 VAE in comfy/models/vae

### Configure Workflow Nodes
- **Timestamp**: [17:30](https://www.youtube.com/watch?v=A_nAU8h9YOY&t=1050)
- **Action**: Refresh the model list, then select Ernie Image Turbo as the model, Minestral 3B as the clip name, and Flux 2 VAE as the VAE in the respective nodes.
- **Command Or Clicks**: Press R to refresh > Select Ernie Image Turbo > Select Minestral 3B > Select Flux 2 VAE

### Adjust Generation Settings
- **Timestamp**: [18:09](https://www.youtube.com/watch?v=A_nAU8h9YOY&t=1089)
- **Action**: Set the K sampler steps to 8 for the turbo model. Leave CFG at 1.0 for optimal balance. Turn off Prompt Enhancement to save VRAM and time.
- **Command Or Clicks**: Set Steps to 8 > Set CFG to 1 > Toggle Prompt Enhancement OFF

### Generate Image
- **Timestamp**: [19:15](https://www.youtube.com/watch?v=A_nAU8h9YOY&t=1155)
- **Action**: Enter your prompt and click the queue button to generate the image. The result will be saved in the Comfy output folder.
- **Command Or Clicks**: Enter prompt > Click Queue Prompt

### Install GGUF Support for Low VRAM
- **Timestamp**: [21:00](https://www.youtube.com/watch?v=A_nAU8h9YOY&t=1260)
- **Action**: For users with less VRAM, install the ComfyUI GGUF extension by City96 to load compressed models.
- **Command Or Clicks**: Click Extensions > Search 'GGUF' > Install 'ComfyUI GGUF by city96' > Apply and Restart

### Load Compressed GGUF Model
- **Timestamp**: [21:34](https://www.youtube.com/watch?v=A_nAU8h9YOY&t=1294)
- **Action**: Replace the standard diffusion loader with a GGUF loader node, connect it to the K sampler, and select the downloaded Q2K or other GGUF variant.
- **Command Or Clicks**: Double click canvas > Type 'gguf' > Select 'GGUF Loader GGUF' > Connect to K Sampler Model Input > Select Ernie Image Turbo Q2 GGUF

## Gotchas

### Ernie Image struggles with human anatomy, particularly complex poses like yoga or floating figures, often resulting in grotesque or physically impossible limbs.
- **Severity**: serious
- **Timestamp**: [11:44](https://www.youtube.com/watch?v=A_nAU8h9YOY&t=704)

### Prompt Enhancement significantly increases VRAM usage and generation time. Disable it if you have limited hardware resources.
- **Severity**: serious
- **Timestamp**: [18:09](https://www.youtube.com/watch?v=A_nAU8h9YOY&t=1089)

### Compressed GGUF models (like Q2K) sacrifice quality for lower VRAM usage. The smallest versions may produce noticeably lower fidelity images.
- **Severity**: heads_up
- **Timestamp**: [20:45](https://www.youtube.com/watch?v=A_nAU8h9YOY&t=1245)

### Both Ernie and Zage failed to accurately render specific text '11:15' on a clock face and filling a wine glass to the top in the final test.
- **Severity**: heads_up
- **Timestamp**: [11:15](https://www.youtube.com/watch?v=A_nAU8h9YOY&t=675)

## Where to go next

Check the description for links to the GGUF compressed models and the Unsloth page. Subscribe to the weekly newsletter for more AI tool updates.

## Concepts surfaced

[[ernie-image]] · [[comfyui-tutorial]] · [[local-ai-generation]] · [[gguf-compression]] · [[open-source-image-models]]
