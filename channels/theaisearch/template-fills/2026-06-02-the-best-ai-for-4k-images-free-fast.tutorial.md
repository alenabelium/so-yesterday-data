---
video_id: DlvhlQOBHBw
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-06-02-the-best-ai-for-4k-images-free-fast.md
source_transcript: ../transcripts/2026-06-02-the-best-ai-for-4k-images-free-fast.md
source_summary_hash: sha256:4c8dc4dc94b45a672f3aabbc942b45925e4ab1fe1afe98f1cb56936dc8c04cd7
source_transcript_hash: sha256:a9a3d5dfff1091dbe99910d344ec917692af179a100a629eeed31828588ab7b6
fill_id: 2661bf4c-eef0-411f-8dd3-b88c702605c7
published_at: '2026-06-04T21:14:19.110182'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Install Nvidia's Pixel Diffusion in Comfy UI to upscale images to 4K resolution for free, offline, and in under 10 seconds.

## Prerequisites

### Comfy UI
- **Kind**: tool
- **Note**: Latest version installed locally. Use update Comfy.bat to ensure workflow compatibility.

### Nvidia GPU
- **Kind**: hardware
- **Note**: Required for inference. Blackwell architecture or 50 series needed for MXFP8 variants.

### Gemma 2 2B
- **Kind**: tool
- **Note**: Text encoder model required for Pixel Diffusion workflows. Download FP8 for speed.

### Pixel Diffusion Model
- **Kind**: tool
- **Note**: Upscaler model. Select variant matching your base generator (e.g., Flux 1 for Z Image).

## Steps

### Update Comfy UI
- **Timestamp**: [04:27](https://www.youtube.com/watch?v=DlvhlQOBHBw&t=267)
- **Action**: Ensure Comfy UI is updated to the latest version to prevent workflow errors. Run the portable update script.
- **Command Or Clicks**: Click update Comfy.bat in the Comfy folder. Wait for 'press any key to continue'.
- **Choice Branch**: Use the portable version's update script rather than manual pip updates.

### Download Workflow and Gemma 2B
- **Timestamp**: [07:23](https://www.youtube.com/watch?v=DlvhlQOBHBw&t=443)
- **Action**: Download the O2 upscaling workflow JSON and the Gemma 2 2B text encoder (FP8 recommended).
- **Command Or Clicks**: Save Gemma 2B to Comfy UI/models/text_encoders. Drag workflow JSON onto Comfy UI interface.
- **Choice Branch**: Choose FP8 for speed or FP16 for quality. FP8 is smaller and faster.

### Install Pixel Diffusion Model
- **Timestamp**: [08:33](https://www.youtube.com/watch?v=DlvhlQOBHBw&t=513)
- **Action**: Download the correct Pixel Diffusion upscaler model variant based on your base generator (e.g., Flux 1 for Z Image).
- **Command Or Clicks**: Save model to Comfy UI/models/diffusion_models. Press R to refresh model list.
- **Choice Branch**: Use BF16 for compatibility or MXFP8 for smaller size (requires Blackwell/50 series GPU).

### Configure Upscaling Settings
- **Timestamp**: [10:32](https://www.youtube.com/watch?v=DlvhlQOBHBw&t=632)
- **Action**: Set dimensions to 4096x2732 for 4K output, select the VAE (AE.safe tensors), and input a matching text prompt.
- **Command Or Clicks**: Set width to 4096. Select AE.safe tensors in VAE dropdown. Enter prompt matching image content.
- **Choice Branch**: Ensure input image longest side is 1024 for the 1K-to-4K model variant.

### Run Upscale and Compare
- **Timestamp**: [12:34](https://www.youtube.com/watch?v=DlvhlQOBHBw&t=754)
- **Action**: Execute the workflow and use the compare node to view the before/after difference.
- **Command Or Clicks**: Press Run. Double click canvas, type 'compare', and connect input/output nodes.
- **Choice Branch**: Use the compare node to verify detail retention in the upscaled output.

### Setup Z Image + Pixel Diffusion
- **Timestamp**: [14:29](https://www.youtube.com/watch?v=DlvhlQOBHBw&t=869)
- **Action**: Download the O3 workflow and install Z Image Turbo (FP4) and Qwen 34B text encoder.
- **Command Or Clicks**: Save Z Image Turbo to diffusion_models. Save Qwen 34B to text_encoders. Press R to refresh.
- **Choice Branch**: Use FP4 for Z Image Turbo if on newer CUDA GPUs for efficiency.

### Generate and Upscale with Z Image
- **Timestamp**: [17:20](https://www.youtube.com/watch?v=DlvhlQOBHBw&t=1040)
- **Action**: Configure Z Image settings (7-9 steps, CFG 1) and run the workflow to generate and upscale simultaneously.
- **Command Or Clicks**: Set steps to 7-9. CFG to 1. Sampler to euler. Press Run.
- **Choice Branch**: Keep longest side at 1024 for the input image before upscaling.

### Optional: Direct Text-to-Image
- **Timestamp**: [20:40](https://www.youtube.com/watch?v=DlvhlQOBHBw&t=1240)
- **Action**: Download the O1 workflow and the tiny Pixel Diffusion text-to-image model for direct generation.
- **Command Or Clicks**: Save BF16 text-to-image model to diffusion_models. Select Gemma 2B as clip encoder.
- **Choice Branch**: Note: This workflow only generates 1K resolution and is less impressive than Z Image.

## Gotchas

### Workflow will fail if Comfy UI is not updated to the latest version. Always run update Comfy.bat first.
- **Severity**: blocking
- **Timestamp**: [04:27](https://www.youtube.com/watch?v=DlvhlQOBHBw&t=267)

### MXFP8 model variants only work on Blackwell architecture or Nvidia 50 series GPUs. Older GPUs like 3090 may fail.
- **Severity**: blocking
- **Timestamp**: [09:29](https://www.youtube.com/watch?v=DlvhlQOBHBw&t=569)

### Ensure the input image's longest side is 1024 when using the 1K-to-4K upscaling model for best results.
- **Severity**: serious
- **Timestamp**: [10:32](https://www.youtube.com/watch?v=DlvhlQOBHBw&t=632)

## Where to go next

Explore Z Image Turbo for generation or Flux 2 for alternative base models. Check the description for all workflow links and model downloads.

## Concepts surfaced

[[pixel-diffusion]] · [[comfy-ui-tutorial]] · [[image-upscaling]] · [[nvidia-ai]] · [[z-image]] · [[flux-model]]
