---
video_id: OtuoOWsnLDg
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-01-29-z-image-base-is-out-best-local-ai-image-model.md
source_transcript: ../transcripts/2026-01-29-z-image-base-is-out-best-local-ai-image-model.md
source_summary_hash: sha256:8943722a529cfc2e514f503b37966ea16fb2f155e0a7b8255fd5a1ce43ab5fd9
source_transcript_hash: sha256:26fba42bd6ecc1042b1b6f6c0c35c969e12a3edde02ab0c0cc9824ddfbefb57b
fill_id: bdcbbab0-aa66-4e18-9c49-611d4b196530
published_at: '2026-10-19T20:50:09.793790'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Learn to install and run Z-Image Base locally in Comfy UI, including low-VRAM GGUF options, image-to-image, and inpainting workflows.

## Prerequisites

### Comfy UI installed
- **Kind**: tool
- **Note**: The host assumes you already have Comfy UI installed; recommends the Windows portable version.

### Comfy UI updated
- **Kind**: tool
- **Note**: Update to the latest version via the update folder before proceeding.

### Hugging Face account
- **Kind**: account
- **Note**: Required to download model files from the official Hugging Face page.

### GPU with at least 12GB VRAM
- **Kind**: hardware
- **Note**: For the full BF-16 model; lower VRAM users can use GGUF versions.

## Steps

### Update Comfy UI
- **Timestamp**: [09:56](https://www.youtube.com/watch?v=OtuoOWsnLDg&t=596)
- **Action**: Open the update folder in your Comfy UI installation and run the update script to pull the latest changes.
- **Command Or Clicks**: Double-click 'update_comfy.bat' (or similar) and press run.
- **Choice Branch**: Choose 'update_comfy.bat' for latest or 'update_comfy_stable.bat' for stable.

### Start Comfy UI and load Z-Image template
- **Timestamp**: [10:44](https://www.youtube.com/watch?v=OtuoOWsnLDg&t=644)
- **Action**: Launch Comfy UI, click the templates button on the left sidebar, select 'image', then choose 'Zimage text to image' (not the Turbo one).
- **Command Or Clicks**: Click 'Templates' > 'Image' > 'Zimage text to image'.
- **Choice Branch**: If template missing, download workflow from linked Comfy UI page.

### Download required models
- **Timestamp**: [12:00](https://www.youtube.com/watch?v=OtuoOWsnLDg&t=720)
- **Action**: Download the Z-Image BF-16 model (12GB), the Qwen 34B text encoder (7.8GB), and the VAE (327MB) into the appropriate Comfy UI folders.
- **Command Or Clicks**: Click links in workflow; save to 'models/diffusion_models', 'models/text_encoders', 'models/vae'.
- **Choice Branch**: If you already have Qwen 34B and VAE from Turbo, skip those downloads.

### Configure model nodes
- **Timestamp**: [13:38](https://www.youtube.com/watch?v=OtuoOWsnLDg&t=818)
- **Action**: After downloading, press R to refresh model lists, then select the downloaded models in the workflow dropdowns.
- **Command Or Clicks**: Press R; select 'Zimage BF-16', 'Qwen 34B', 'AE.safetensors'.

### Set generation parameters
- **Timestamp**: [14:26](https://www.youtube.com/watch?v=OtuoOWsnLDg&t=866)
- **Action**: Adjust width, height, batch size, positive/negative prompts, seed, steps (30-50), and CFG (3-5) for optimal results.
- **Command Or Clicks**: Set steps to 30-50, CFG to 3-5, seed to randomize.

### Run generation
- **Timestamp**: [15:44](https://www.youtube.com/watch?v=OtuoOWsnLDg&t=944)
- **Action**: Press run to generate the image; results save automatically to the output folder.
- **Command Or Clicks**: Press 'Run'.

### Use GGUF for low VRAM
- **Timestamp**: [18:22](https://www.youtube.com/watch?v=OtuoOWsnLDg&t=1102)
- **Action**: Download a GGUF version (e.g., Q2K 4GB) and replace the model node with a GGUF loader node in the workflow.
- **Command Or Clicks**: Download GGUF to 'models/unet'; double-click, search 'unet loader GGUF', connect to model input.
- **Choice Branch**: If GGUF node missing, install 'ComfyUI-GGUF' via Manager.

### Set up image-to-image workflow
- **Timestamp**: [19:35](https://www.youtube.com/watch?v=OtuoOWsnLDg&t=1175)
- **Action**: Modify the text-to-image workflow to accept an input image by adding a Load Image node and a VAE Encode node, then connect to the KSampler.
- **Command Or Clicks**: Double-click, search 'load image', add 'VAE encode', connect VAE and image, set denoise to 0.5.

### Adjust denoise for image-to-image
- **Timestamp**: [22:03](https://www.youtube.com/watch?v=OtuoOWsnLDg&t=1323)
- **Action**: Tune the denoise value to control how much of the original image is retained; increase if too much is kept.
- **Command Or Clicks**: Set denoise to 0.5 initially, then increase to 0.84 if needed.

### Set up inpainting workflow
- **Timestamp**: [23:00](https://www.youtube.com/watch?v=OtuoOWsnLDg&t=1380)
- **Action**: Load an image, use the mask editor to brush over areas to edit, then add a Set Latent Noise Mask node to connect the mask to the KSampler.
- **Command Or Clicks**: Right-click Load Image > 'Open Mask Editor', brush area, save; add 'Set Latent Noise Mask' node.

### Run inpainting generation
- **Timestamp**: [24:24](https://www.youtube.com/watch?v=OtuoOWsnLDg&t=1464)
- **Action**: Enter a prompt describing the desired edit and run the workflow; adjust denoise if you want to retain parts of the original.
- **Command Or Clicks**: Enter prompt, press 'Run'.

### Add LoRA to workflow
- **Timestamp**: [25:20](https://www.youtube.com/watch?v=OtuoOWsnLDg&t=1520)
- **Action**: Once Z-Image Base LoRAs are available, add a 'LoRA Loader Model Only' node after the diffusion model and connect it.
- **Command Or Clicks**: Double-click, search 'LoRA loader model only', connect model and output.

## Gotchas

### Z-Image Turbo LoRAs do not work with Z-Image Base; don't waste time trying to add them.
- **Severity**: blocking
- **Timestamp**: [25:20](https://www.youtube.com/watch?v=OtuoOWsnLDg&t=1520)

### The BF-16 model is 12GB; you'll need at least 12GB VRAM plus offloading to run it.
- **Severity**: serious
- **Timestamp**: [12:00](https://www.youtube.com/watch?v=OtuoOWsnLDg&t=720)

### Z-Image Base is slower than Turbo (about 1.5 minutes vs 7 seconds on the host's GPU).
- **Severity**: heads_up
- **Timestamp**: [16:46](https://www.youtube.com/watch?v=OtuoOWsnLDg&t=1006)

### Negative prompts only work with CFG 3-5; Turbo uses CFG 0-1 so negative prompts don't work there.
- **Severity**: heads_up
- **Timestamp**: [15:44](https://www.youtube.com/watch?v=OtuoOWsnLDg&t=944)

## Where to go next

Check the linked resources for training LoRAs with AI Toolkit or the quick Z-Image Image-to-LoRA method. Subscribe to the weekly newsletter for more AI tools and tutorials.

## Concepts surfaced

[[comfy-ui]] · [[gguf-quantization]] · [[lora-fine-tuning]] · [[image-to-image]] · [[inpainting]] · [[negative-prompts]]
