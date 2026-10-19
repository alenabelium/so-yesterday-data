---
video_id: I_b2QN-B1W0
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-01-08-new-1-open-source-ai-video-generator-is-here-fast-4k-audio-l.md
source_transcript: ../transcripts/2026-01-08-new-1-open-source-ai-video-generator-is-here-fast-4k-audio-l.md
source_summary_hash: sha256:d23e6eb1f0d4070ee8bff86a0101e5899ffd96895f6b743e158d51b9c206f8e0
source_transcript_hash: sha256:919313dc311529e1c38fac09f978d076e403b7321818dc0153be61b54f9f3da3
fill_id: 21a1c08d-250d-4819-bfb6-97529d435db9
published_at: '2026-10-19T21:00:55.910432'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

LTX-2 is the new top open-source video generator with native audio, 4K support, and low-VRAM capability, and this guide shows you how to set it up in ComfyUI.

## Prerequisites

### ComfyUI installed
- **Kind**: tool
- **Note**: The tutorial assumes you already have ComfyUI installed. If not, the host points to a separate installation video.

### CUDA GPU (optional)
- **Kind**: hardware
- **Note**: The official docs say 32GB VRAM, but the host shows how to run on as low as 2GB VRAM if you have enough system RAM.

### Sufficient system RAM
- **Kind**: hardware
- **Note**: To run LTX-2 with low VRAM, you need enough RAM to hold the model, upscaler, and text encoder (roughly 36GB total).

## Steps

### Update ComfyUI to the latest version
- **Timestamp**: [04:01](https://www.youtube.com/watch?v=I_b2QN-B1W0&t=241)
- **Action**: Before opening ComfyUI, update it to the latest version to ensure compatibility with LTX-2 workflows. Use the update script in the ComfyUI folder.
- **Command Or Clicks**: Double-click 'update_comfyui.bat' or 'update_comfyui_stable.bat' in the ComfyUI folder.
- **Choice Branch**: Try 'update_comfyui_stable.bat' first for safety.

### Install the ComfyUI LTX Video custom nodes
- **Timestamp**: [05:06](https://www.youtube.com/watch?v=I_b2QN-B1W0&t=306)
- **Action**: Open ComfyUI, go to the Manager, search for 'LTX video', and install the 'ComfyUI LTX video' custom nodes. If already installed, update to the latest version.
- **Command Or Clicks**: Click 'Manager' > search 'LTX video' > install 'ComfyUI LTX video'.

### Download the LTX-2 model files
- **Timestamp**: [07:46](https://www.youtube.com/watch?v=I_b2QN-B1W0&t=466)
- **Action**: Download the LTX-2 model checkpoints from the official Hugging Face repo. For the full workflow, you can use the full, FP8, or FP4 versions. For the distilled workflow, download the distilled FP8 checkpoint.
- **Command Or Clicks**: Download 'ltx2-8b-distilled-fp8.safetensors' (27GB) and place it in 'ComfyUI/models/checkpoints'.
- **Choice Branch**: Choose the distilled FP8 model for faster generation with lower VRAM.

### Download the video upscaler model
- **Timestamp**: [10:14](https://www.youtube.com/watch?v=I_b2QN-B1W0&t=614)
- **Action**: Download the spatial upscaler model from the provided link. This is used in the second pass of video generation to enhance resolution.
- **Command Or Clicks**: Download the upscaler (~1GB) and place it in 'ComfyUI/models/upscale_models'.

### Install a quantized Gemma 3 text encoder
- **Timestamp**: [12:11](https://www.youtube.com/watch?v=I_b2QN-B1W0&t=731)
- **Action**: To save VRAM, install a 4-bit quantized version of Gemma 3 (by Unsloth) instead of the full 24GB model. Clone the repo into the text encoders folder.
- **Command Or Clicks**: In 'ComfyUI/models/text_encoders', run: git clone <URL>
- **Choice Branch**: Use the quantized Gemma 3 (7.8GB) to reduce memory usage.

### Configure the text-to-video workflow
- **Timestamp**: [13:00](https://www.youtube.com/watch?v=I_b2QN-B1W0&t=780)
- **Action**: Load the 'LTX text to video distilled' workflow. Set the model paths, select the Gemma 3 quantized model, and adjust width, height, and frame count.
- **Command Or Clicks**: In the workflow, set 'LTXV path' to 'distilled_fp8', select 'Gemma 3' model, set width 1280, height 720, frames 121.

### Run text-to-video generation
- **Timestamp**: [13:49](https://www.youtube.com/watch?v=I_b2QN-B1W0&t=829)
- **Action**: Enter a positive prompt and click 'Run' to generate the video. The output is automatically saved in the output folder.
- **Command Or Clicks**: Click 'Run' in ComfyUI.

### Optimize for low VRAM
- **Timestamp**: [16:14](https://www.youtube.com/watch?v=I_b2QN-B1W0&t=974)
- **Action**: Edit the ComfyUI source file to reduce VRAM usage, and add startup parameters to reserve or offload VRAM.
- **Command Or Clicks**: Edit 'ComfyUI/comfy/ldm/modules/embeddings_connector.py' and replace the line with the provided code. Edit 'run_nvidia_gpu.bat' to add '--reserve-vram 4' or '--lowvram'.
- **Choice Branch**: Use '--reserve-vram 4' for VRAM under 8GB, or '--lowvram' for under 4GB.

### Add LoRA to text-to-video workflow
- **Timestamp**: [19:45](https://www.youtube.com/watch?v=I_b2QN-B1W0&t=1185)
- **Action**: Download a LoRA (e.g., dolly left) and load it into the workflow. You need to load the LoRA twice: once for the first pass and once for the second pass.
- **Command Or Clicks**: Download 'ltx2-lora-dolly-left.safetensors' and place in 'ComfyUI/models/loras'. In the workflow, select the LoRA for both the first and second pass nodes.

### Run image-to-video generation
- **Timestamp**: [20:46](https://www.youtube.com/watch?v=I_b2QN-B1W0&t=1246)
- **Action**: Load the 'LTX image to video distilled' workflow. Upload a starting image, set the prompt, and adjust length. Optionally bypass the enhancer node for speed.
- **Command Or Clicks**: Upload an image, set prompt, set frames (e.g., 121), click 'Run'.

### Use ControlNet for pose-to-video
- **Timestamp**: [25:40](https://www.youtube.com/watch?v=I_b2QN-B1W0&t=1540)
- **Action**: Load the 'LTX ControlNet' workflow. Upload a reference video, select pose extraction, and set the prompt. Install the required pose LoRA and controlnet auxiliary nodes.
- **Command Or Clicks**: Upload reference video, select 'pose', download 'ltx2-lora-pose.safetensors' (654MB) and place in 'ComfyUI/models/loras'. Install 'comfyui_controlnet_aux' via Manager.

### Use ControlNet for canny-to-video
- **Timestamp**: [31:21](https://www.youtube.com/watch?v=I_b2QN-B1W0&t=1881)
- **Action**: In the same ControlNet workflow, switch to canny extraction. Download the canny LoRA and replace the missing canny node with the one from the auxiliary pack.
- **Command Or Clicks**: Download 'ltx2-lora-canny.safetensors' (654MB) and place in 'ComfyUI/models/loras'. Replace the missing 'Canny' node with 'Canny Edge Detector'.

### Use the video upscaler workflow
- **Timestamp**: [35:10](https://www.youtube.com/watch?v=I_b2QN-B1W0&t=2110)
- **Action**: Load the 'V2V Detailer' workflow. Upload a low-resolution video, download the full model (FP4) and detailer LoRA, and run to upscale.
- **Command Or Clicks**: Download 'ltx2-8b-fp4.safetensors' (20GB) and 'ltx2-lora-detailer.safetensors' (2.6GB). Place in respective folders. Set 'largest side' to 1920.

## Gotchas

### The official docs say you need 32GB VRAM, but that's not true. You can run with as low as 2GB VRAM if you have enough system RAM.
- **Severity**: heads_up
- **Timestamp**: [04:01](https://www.youtube.com/watch?v=I_b2QN-B1W0&t=241)

### The default Gemma 3 text encoder is 24GB, which is too large. Use the quantized 4-bit version (7.8GB) to save VRAM.
- **Severity**: serious
- **Timestamp**: [12:11](https://www.youtube.com/watch?v=I_b2QN-B1W0&t=731)

### If you have low VRAM, you must add '--reserve-vram 4' or '--lowvram' to the startup command, otherwise Windows may fight for VRAM and cause errors.
- **Severity**: blocking
- **Timestamp**: [17:29](https://www.youtube.com/watch?v=I_b2QN-B1W0&t=1049)

### In the ControlNet workflow, the 'enhancer' node may be missing and you can't find it. Delete it or bypass it to avoid errors.
- **Severity**: heads_up
- **Timestamp**: [28:26](https://www.youtube.com/watch?v=I_b2QN-B1W0&t=1706)

### The canny workflow has a missing 'Canny' node. You need to replace it with the 'Canny Edge Detector' from the controlnet auxiliary pack.
- **Severity**: blocking
- **Timestamp**: [34:02](https://www.youtube.com/watch?v=I_b2QN-B1W0&t=2042)

### The built-in upscaler is not great; there are better dedicated upscalers, but this is an option.
- **Severity**: heads_up
- **Timestamp**: [37:03](https://www.youtube.com/watch?v=I_b2QN-B1W0&t=2223)

## Where to go next

LTX-2 is a game-changer for open-source video generation. If you run into errors, share the exact error message in the comments for help. Also, subscribe to the free weekly newsletter for the latest AI tools and news.

## Concepts surfaced

[[ltx2]] · [[comfyui]] · [[text-to-video]] · [[image-to-video]] · [[controlnet]] · [[lora]]
