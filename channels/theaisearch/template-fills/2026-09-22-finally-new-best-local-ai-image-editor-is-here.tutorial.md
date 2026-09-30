---
video_id: BaE6UBfNdQk
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-09-22-finally-new-best-local-ai-image-editor-is-here.md
source_transcript: ../transcripts/2026-09-22-finally-new-best-local-ai-image-editor-is-here.md
source_summary_hash: sha256:91e735ebc578a28065c8108d669b1c4b93b371d5043c735bfa16e07d7fd03698
source_transcript_hash: sha256:b1cf7df4e892fc2e5b3b75fce4a8ccec76373f83611023289acfe954e509951b
fill_id: c8cb2b05-fb34-434e-830b-ce1a6569a688
published_at: '2026-09-30T13:57:23.577667'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Install Qwen Image 2.1 locally with Comfy UI and run it on low VRAM using quantized GGUF models.

## Prerequisites

### Comfy UI installed
- **Kind**: tool
- **Note**: Comfy UI is the platform used to run Qwen Image 2.1 locally. If not installed, watch the linked tutorial first.

### GPU with at least 4GB VRAM
- **Kind**: hardware
- **Note**: For low VRAM, use GGUF quantized models; the smallest is 3.19 GB.

## Steps

### Update Comfy UI to the latest version
- **Timestamp**: [03:30](https://www.youtube.com/watch?v=BaE6UBfNdQk&t=210)
- **Action**: Double-click the update folder and run the update script to ensure Comfy UI is up to date.
- **Command Or Clicks**: Double-click 'update_ComfyUI.bat' in the update folder.

### Open the Qwen Image 2.1 text-to-image workflow
- **Timestamp**: [04:10](https://www.youtube.com/watch?v=BaE6UBfNdQk&t=250)
- **Action**: In Comfy UI, click 'templates' in the left sidebar, search for 'Qwen Image 2.1', and select the 'Text to Image' workflow. If missing, download workflow files and drag them onto the interface.
- **Command Or Clicks**: Click 'templates' > search 'Qwen Image 2.1' > select 'Text to Image'.
- **Choice Branch**: If workflows not visible, download from linked page and drag-drop onto Comfy UI.

### Download the diffusion model
- **Timestamp**: [04:50](https://www.youtube.com/watch?v=BaE6UBfNdQk&t=290)
- **Action**: From the linked model page, download the diffusion model. Choose the INT8 quantized version (7.2 GB) for 8GB VRAM or the full BF-16 (14.2 GB). Save to the diffusion_models folder.
- **Command Or Clicks**: Download 'qwen_image_2.1_int8.safetensors' to 'ComfyUI/models/diffusion_models'.
- **Choice Branch**: For 4GB VRAM, skip this and use GGUF models later.

### Download the text encoder
- **Timestamp**: [05:30](https://www.youtube.com/watch?v=BaE6UBfNdQk&t=330)
- **Action**: Download the smallest text encoder (W4A8, 6.3 GB) for low VRAM. Avoid the optional prompt-enhancer models (9.5 GB each) if VRAM is limited.
- **Command Or Clicks**: Download 'qwen_3_vl_w4a8.safetensors' to 'ComfyUI/models/text_encoders'.
- **Choice Branch**: If VRAM is ample, you may also download the prompt enhancer models.

### Download the VAE
- **Timestamp**: [06:06](https://www.youtube.com/watch?v=BaE6UBfNdQk&t=366)
- **Action**: Download the VAE file (676 MB) and save it to the VAE folder.
- **Command Or Clicks**: Download 'qwen_image_2.1_vae.safetensors' to 'ComfyUI/models/vae'.

### Select models in the workflow
- **Timestamp**: [06:30](https://www.youtube.com/watch?v=BaE6UBfNdQk&t=390)
- **Action**: Press R to refresh the model list, then select the downloaded models for the UNet, CLIP, and VAE nodes.
- **Command Or Clicks**: Press R, then select 'qwen_image_2.1_int8.safetensors' for UNet, 'qwen_3_vl_w4a8.safetensors' for CLIP, and the VAE file.

### Configure generation settings and run
- **Timestamp**: [07:00](https://www.youtube.com/watch?v=BaE6UBfNdQk&t=420)
- **Action**: Set aspect ratio, megapixels, prompt, CFG, steps, and seed. Click 'Run' to generate.
- **Command Or Clicks**: Adjust settings, then click 'Run'.
- **Choice Branch**: Increase CFG for stricter prompt adherence; decrease for more creativity. CFG=1 disables negative prompt.

### Use the image editing workflow
- **Timestamp**: [08:20](https://www.youtube.com/watch?v=BaE6UBfNdQk&t=500)
- **Action**: Open the 'Image Edit' workflow from templates. Load models, upload reference images (up to 10), set prompt, and run.
- **Command Or Clicks**: Click 'templates' > 'Image Edit', load models, upload image, set prompt, click 'Run'.
- **Choice Branch**: Use custom size toggle to override input image dimensions.

### Use the remove background workflow
- **Timestamp**: [11:30](https://www.youtube.com/watch?v=BaE6UBfNdQk&t=690)
- **Action**: Open the 'Remove Background' workflow, load models, upload an image, set prompt to remove background, and run.
- **Command Or Clicks**: Click 'templates' > 'Remove Background', load models, upload image, prompt 'remove the background, keep only the woman, output PNG', click 'Run'.
- **Choice Branch**: Set custom size to false to keep original resolution.

### Load a LoRA for character consistency
- **Timestamp**: [13:32](https://www.youtube.com/watch?v=BaE6UBfNdQk&t=812)
- **Action**: Download a LoRA (e.g., Qwen 2.1 anime consistency) and place it in the LoRA folder. In the image edit workflow, add a Load LoRA node between the model and the next node, select the LoRA, set strength, and connect.
- **Command Or Clicks**: Download LoRA to 'ComfyUI/models/loras'. Double-click to add 'Load LoRA' node, select LoRA, set strength, connect.
- **Choice Branch**: Stack multiple LoRAs by copying the node or using a LoRA stacker.

### Run with GGUF models for low VRAM
- **Timestamp**: [15:45](https://www.youtube.com/watch?v=BaE6UBfNdQk&t=945)
- **Action**: Download a GGUF quantized model (e.g., Q3, 3.19 GB) and save to the unet folder. In the workflow, replace the diffusion model loader with a UNET Loader (GGUF) node, select the GGUF, and run.
- **Command Or Clicks**: Download GGUF to 'ComfyUI/models/unet'. Add 'UNET Loader (GGUF)' node, connect, select GGUF, click 'Run'.
- **Choice Branch**: Install the Comfy GGUF extension if the node is missing.

## Gotchas

### The optional prompt-enhancer text encoders are ~9.5 GB each; avoid them if VRAM is low. Write good prompts manually instead.
- **Severity**: heads_up
- **Timestamp**: [05:30](https://www.youtube.com/watch?v=BaE6UBfNdQk&t=330)

### Setting CFG to 1 disables the negative prompt; increase CFG slightly for it to take effect.
- **Severity**: heads_up
- **Timestamp**: [07:00](https://www.youtube.com/watch?v=BaE6UBfNdQk&t=420)

### The official license prohibits commercial use without a separate license, but Qwen confirmed outputs are not licensed materials, so you retain rights to your generations.
- **Severity**: serious
- **Timestamp**: [17:57](https://www.youtube.com/watch?v=BaE6UBfNdQk&t=1077)

## Where to go next

Check the linked Comfy UI installation tutorial if you're new, and explore more Qwen Image 2.1 workflows and LoRAs as the community releases them.

## Concepts surfaced

[[comfy-ui]] · [[qwen-image-2-1]] · [[gguf-quantization]] · [[lora-fine-tuning]] · [[transparent-background]] · [[image-editing]]
