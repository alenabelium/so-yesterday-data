---
video_id: A_nAU8h9YOY
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-04-16-new-best-local-ai-image-generator-is-here.md
source_transcript: ../transcripts/2026-04-16-new-best-local-ai-image-generator-is-here.md
source_summary_hash: sha256:203a13ed4d5529068a9a42e3ac71c0ee48a103603c1b02b74c6b2fb69bf5eb02
source_transcript_hash: sha256:e9ed65d8fddd8917a588fbf0567abdb0cd835153dcf6b40969ffc45ca50255a3
fill_id: 1a343cfa-1414-43c2-8d6a-85f519f4bf1b
published_at: '2026-10-19T20:15:50.118775'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Ernie Image is a new open-source AI image generator that beats Zage in prompt adherence and text rendering, and you can run it locally for free via ComfyUI.

## Prerequisites

### ComfyUI
- **Kind**: tool
- **Note**: The most popular interface for running open-source image and video generators on your computer. Must be installed and updated to the latest version.

### GPU with ~20GB VRAM (or lower with GGUF)
- **Kind**: hardware
- **Note**: Original models need around 20GB total (16GB model + text encoder + VAE). Compressed GGUF versions can run on as low as 3.18GB.

## Steps

### Update ComfyUI to the latest version
- **Timestamp**: [15:06](https://www.youtube.com/watch?v=A_nAU8h9YOY&t=906)
- **Action**: Open your ComfyUI folder, double-click the update folder, then run update_comfyui.bat to update to the latest version.
- **Command Or Clicks**: Double-click update folder → update_comfyui.bat

### Launch ComfyUI and load the Ernie Image workflow
- **Timestamp**: [15:06](https://www.youtube.com/watch?v=A_nAU8h9YOY&t=906)
- **Action**: Run ComfyUI by double-clicking run.bat. In the left sidebar, click 'templates', search for 'Ernie', and select either the Ernie Image or Ernie Image Turbo workflow. The Turbo version requires fewer steps.
- **Command Or Clicks**: run.bat → Templates → search 'Ernie' → select Ernie Image Turbo
- **Choice Branch**: Choose Ernie Image Turbo for speed; Ernie Image base for slightly better quality but 3-5x slower.

### Download missing models via ComfyUI error prompt
- **Timestamp**: [16:08](https://www.youtube.com/watch?v=A_nAU8h9YOY&t=968)
- **Action**: Click 'see errors' to see missing models. Click the download button next to the Ernie Image Turbo model to auto-download it. If the sidebar is missing, manually download the model from the node's link.
- **Command Or Clicks**: See errors → Download button

### Download text encoder and VAE
- **Timestamp**: [16:08](https://www.youtube.com/watch?v=A_nAU8h9YOY&t=968)
- **Action**: Ensure you have the Minestral 3B text encoder (7.5GB) and Flux 2 VAE (300MB). Click the links in the nodes to download them to the correct folders.
- **Command Or Clicks**: Click links → save to ComfyUI/models/text_encoders and ComfyUI/models/vae

### Refresh and select models in the workflow
- **Timestamp**: [17:00](https://www.youtube.com/watch?v=A_nAU8h9YOY&t=1020)
- **Action**: Press R to refresh the model list. In the workflow, select the Ernie Image Turbo model, Minestral 3B for clip, and Flux 2 VAE for VAE. Refresh the page to clear the red outline.
- **Command Or Clicks**: Press R → select model, clip, VAE → refresh page

### Configure prompt and generation settings
- **Timestamp**: [18:09](https://www.youtube.com/watch?v=A_nAU8h9YOY&t=1089)
- **Action**: Enter your prompt in the prompt node. Adjust width and height. Optionally enable prompt enhancement (uses more VRAM/time). In the K sampler, set steps to 8 for turbo, keep CFG at 1, and leave sampler default.
- **Command Or Clicks**: Enter prompt → set steps=8 → CFG=1
- **Choice Branch**: Enable prompt enhancement for better prompts but more VRAM/time; disable for speed.

### Run the generation
- **Timestamp**: [19:15](https://www.youtube.com/watch?v=A_nAU8h9YOY&t=1155)
- **Action**: Click 'Run' to generate the image. ComfyUI dynamically allocates memory, so it can run even with limited VRAM. The image saves automatically to the output folder.
- **Command Or Clicks**: Click Run

### Install GGUF loader for low VRAM
- **Timestamp**: [20:45](https://www.youtube.com/watch?v=A_nAU8h9YOY&t=1245)
- **Action**: If you have less than 20GB VRAM, download a compressed GGUF version from Unsloth's page. In ComfyUI, install the 'ComfyUI GGUF' extension by city96, then replace the diffusion model loader with a GGUF loader.
- **Command Or Clicks**: Extensions → search 'GGUF' → install ComfyUI GGUF by city96
- **Choice Branch**: Choose a GGUF size that fits your VRAM, e.g., Q6_1 for 8GB.

### Replace model loader with GGUF loader
- **Timestamp**: [21:34](https://www.youtube.com/watch?v=A_nAU8h9YOY&t=1294)
- **Action**: After restarting ComfyUI, double-click on canvas, search 'unet', and add the 'UNET Loader (GGUF)' node. Connect it to the KSampler's model input, bypass the old loader with Ctrl+B, and select your GGUF file.
- **Command Or Clicks**: Double-click canvas → search 'unet' → add UNET Loader (GGUF) → connect to KSampler → Ctrl+B to bypass old loader

## Gotchas

### The original Ernie Image models require ~20GB VRAM total (16GB model + text encoder + VAE). If you have less, use a compressed GGUF version.
- **Severity**: blocking
- **Timestamp**: [15:06](https://www.youtube.com/watch?v=A_nAU8h9YOY&t=906)

### Smaller GGUF versions sacrifice quality; the Q2K version produces noticeably lower-quality images.
- **Severity**: heads_up
- **Timestamp**: [20:45](https://www.youtube.com/watch?v=A_nAU8h9YOY&t=1245)

### Ernie Image struggles with human anatomy, especially complex poses like the king pigeon yoga pose.
- **Severity**: heads_up
- **Timestamp**: [11:44](https://www.youtube.com/watch?v=A_nAU8h9YOY&t=704)

### Prompt enhancement uses more VRAM and time; disable it if you want faster generation.
- **Severity**: heads_up
- **Timestamp**: [18:09](https://www.youtube.com/watch?v=A_nAU8h9YOY&t=1089)

## Where to go next

If you run into errors, copy the exact error message into the comments for troubleshooting. Also, subscribe to the free weekly newsletter for the latest AI news and tools.

## Concepts surfaced

[[open-source-ai]] · [[local-image-generation]] · [[comfyui]] · [[gguf-quantization]] · [[prompt-adherence]]
