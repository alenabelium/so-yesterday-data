---
video_id: -3DVJu72VhE
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-01-01-long-continuous-ai-video-is-here-free-open-source.md
source_transcript: ../transcripts/2026-01-01-long-continuous-ai-video-is-here-free-open-source.md
source_summary_hash: sha256:0602ff96bcf1791e6849880b7491d6bb29b95fce2e4b279a982729126e1fb14f
source_transcript_hash: sha256:db6e00171f8134848c8f545bc08074446be1e0a0c47d3af3399fd3a2324b68a0
fill_id: d299bbd5-8eb6-4da7-9e89-f02f51ed2ce7
published_at: '2026-10-19T21:01:01.137854'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Generate seamless, long AI videos offline for free using Stable Video Infinity v2 Pro and ComfyUI, even with low VRAM.

## Prerequisites

### ComfyUI
- **Kind**: tool
- **Note**: The most popular platform for running open-source image and video models. Windows portable version recommended.

### KJ Nodes
- **Kind**: tool
- **Note**: Required custom nodes for the workflow. Install via git clone or ComfyUI Manager.

### Wan 2.2 I2V Models
- **Kind**: tool
- **Note**: High and low variants of the image-to-video model, each ~15 GB (FP8) or GGUF quantized for lower VRAM.

### Light X2V LoRAs
- **Kind**: tool
- **Note**: Optional but recommended to speed up video generation by 4-5x. High and low versions needed.

### SVI v2 Pro Models
- **Kind**: tool
- **Note**: High and low versions of Stable Video Infinity v2 Pro, each ~1.23 GB.

### UMT5-XXL FP8 Text Encoder
- **Kind**: tool
- **Note**: CLIP model required for text conditioning, ~6.7 GB.

### Wan 2.1 VAE
- **Kind**: tool
- **Note**: VAE model required for decoding, can use compressed version.

### VRAM
- **Kind**: hardware
- **Note**: Works with as low as 6 GB VRAM using GGUF quantized models.

## Steps

### Install KJ Nodes
- **Timestamp**: [01:50](https://www.youtube.com/watch?v=-3DVJu72VhE&t=110)
- **Action**: Open the custom nodes folder in ComfyUI via command prompt and clone the KJ Nodes repository. If already installed, skip this step.
- **Command Or Clicks**: cd ComfyUI/custom_nodes && git clone <KJ-Nodes-URL>

### Install KJ Nodes Dependencies
- **Timestamp**: [04:57](https://www.youtube.com/watch?v=-3DVJu72VhE&t=297)
- **Action**: In the root ComfyUI folder, open command prompt and run the requirements installation command for KJ Nodes.
- **Command Or Clicks**: pip install -r ComfyUI/custom_nodes/KJNodes/requirements.txt

### Update ComfyUI
- **Timestamp**: [05:30](https://www.youtube.com/watch?v=-3DVJu72VhE&t=330)
- **Action**: Open ComfyUI, click on Manager, then Update ComfyUI, and restart to ensure the latest version.
- **Command Or Clicks**: Manager > Update ComfyUI > Restart

### Download and Load the SVI v2 Pro Workflow
- **Timestamp**: [06:01](https://www.youtube.com/watch?v=-3DVJu72VhE&t=361)
- **Action**: Download the workflow JSON file from the provided link and drag-and-drop it onto the ComfyUI canvas to load the pre-built workflow.
- **Command Or Clicks**: Download workflow JSON > Drag & drop onto canvas

### Download Wan 2.2 I2V Models (High & Low)
- **Timestamp**: [07:27](https://www.youtube.com/watch?v=-3DVJu72VhE&t=447)
- **Action**: Download both the high and low variants of the Wan 2.2 image-to-video model (FP8 versions) and place them in the diffusion_models folder.
- **Command Or Clicks**: Download Wan2.2-I2V-High-FP8 and Wan2.2-I2V-Low-FP8 > Save to ComfyUI/models/diffusion_models

### Download Light X2V LoRAs (High & Low)
- **Timestamp**: [08:25](https://www.youtube.com/watch?v=-3DVJu72VhE&t=505)
- **Action**: Download the high and low versions of the Light X2V LoRA to speed up generation, and place them in the Loras folder.
- **Command Or Clicks**: Download LightX2V-High and LightX2V-Low > Save to ComfyUI/models/loras

### Download SVI v2 Pro Models (High & Low)
- **Timestamp**: [09:11](https://www.youtube.com/watch?v=-3DVJu72VhE&t=551)
- **Action**: Download both the high and low versions of the Stable Video Infinity v2 Pro models and place them in the Loras folder.
- **Command Or Clicks**: Download SVI-v2-Pro-High and SVI-v2-Pro-Low > Save to ComfyUI/models/loras

### Download CLIP and VAE Models
- **Timestamp**: [10:00](https://www.youtube.com/watch?v=-3DVJu72VhE&t=600)
- **Action**: Download the UMT5-XXL FP8 text encoder and the Wan 2.1 VAE, placing them in the text_encoders and VAE folders respectively.
- **Command Or Clicks**: Download UMT5-XXL-FP8 > Save to ComfyUI/models/text_encoders; Download Wan2.1-VAE > Save to ComfyUI/models/vae

### Configure Model Selections in Workflow
- **Timestamp**: [11:00](https://www.youtube.com/watch?v=-3DVJu72VhE&t=660)
- **Action**: Refresh the model list and select the downloaded models in the workflow: Wan 2.2 I2V high/low, Light X2V high/low, SVI v2 Pro high/low, CLIP, and VAE.
- **Command Or Clicks**: Press R to refresh > Select models in dropdowns

### Run the Workflow with an Initial Image
- **Timestamp**: [13:05](https://www.youtube.com/watch?v=-3DVJu72VhE&t=785)
- **Action**: Upload an initial image as the first frame, set the width/height and crop settings, then enter prompts for each clip. Press Run to generate the video.
- **Command Or Clicks**: Upload image > Set dimensions > Enter prompts > Click Run

### Add More Clips to Extend Video Length
- **Timestamp**: [16:56](https://www.youtube.com/watch?v=-3DVJu72VhE&t=1016)
- **Action**: Duplicate the clip generation blocks by selecting them and pressing Ctrl+C/Ctrl+V, then connect the samples and extended images outputs to the new blocks. Finally, connect the last extended images output to the video combine node.
- **Command Or Clicks**: Select blocks > Ctrl+C > Ctrl+V > Connect outputs > Connect to Video Combine

### Use GGUF Quantized Models for Low VRAM
- **Timestamp**: [21:00](https://www.youtube.com/watch?v=-3DVJu72VhE&t=1260)
- **Action**: Download GGUF quantized versions of Wan 2.2 (e.g., Q6 for 12 GB VRAM) and use the Unet Loader node to replace the standard model loaders.
- **Command Or Clicks**: Download GGUF models > Install ComfyUI-GGUF node > Add Unet Loader > Select GGUF models

## Gotchas

### If you see errors about Sage Attention or Triton, set the Sage Attention setting to 'disabled' in both high and low nodes.
- **Severity**: blocking
- **Timestamp**: [17:30](https://www.youtube.com/watch?v=-3DVJu72VhE&t=1050)

### Missing 'Wan ImageToVideo SVI Pro' node indicates KJ Nodes not installed or outdated. Update via ComfyUI Manager.
- **Severity**: blocking
- **Timestamp**: [16:56](https://www.youtube.com/watch?v=-3DVJu72VhE&t=1016)

### If PyTorch 2.7.1 is not installed, set the FP16 accumulation setting to 'false' in both high and low nodes to avoid errors.
- **Severity**: serious
- **Timestamp**: [19:05](https://www.youtube.com/watch?v=-3DVJu72VhE&t=1145)

### The default workflow crops the image to 640x640; to keep original dimensions, enter the original width and height in the settings.
- **Severity**: heads_up
- **Timestamp**: [15:30](https://www.youtube.com/watch?v=-3DVJu72VhE&t=930)

## Where to go next

Explore the ecosystem of Wan 2.2 LoRAs on CivitAI to add custom styles, camera motions, and effects. For lower VRAM, try GGUF quantized models. Stay tuned for more AI tools and tutorials.

## Concepts surfaced

[[stable-video-infinity]] · [[wan-2-2]] · [[comfyui]] · [[gguf-quantization]] · [[lora]] · [[video-generation]]
