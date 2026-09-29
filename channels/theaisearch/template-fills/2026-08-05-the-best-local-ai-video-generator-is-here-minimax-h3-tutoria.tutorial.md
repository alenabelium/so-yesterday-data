---
video_id: 8HutJ9W5pTg
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-08-05-the-best-local-ai-video-generator-is-here-minimax-h3-tutoria.md
source_transcript: ../transcripts/2026-08-05-the-best-local-ai-video-generator-is-here-minimax-h3-tutoria.md
source_summary_hash: sha256:83d50ae908b1462efa727ed0f7c383639ae501f426d270cd929f73d9d8bc2f67
source_transcript_hash: sha256:0ac37c2da6ba47423e8970be6b08214d2d8c0a0a588a54fec22fa2e3803c6a8b
fill_id: 6b7db66e-59f3-4758-9242-6f1d438cc92c
published_at: '2026-09-29T11:21:57.792490'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Install Minimax H3 in Comfy UI for local text, image, and audio-to-video generation with optimized VRAM usage.

## Prerequisites

### Comfy UI
- **Kind**: tool
- **Note**: Latest version installed locally. Update via the update_comfy file in the Comfy folder.

### Nvidia GPU
- **Kind**: hardware
- **Note**: VRAM requirements vary from 5GB (1-to-1 GP) to 66GB (full model). FP8/INT8 recommended for most.

### Minimax H3 Models
- **Kind**: tool
- **Note**: Download diffusion models, text encoders (Qwen 3VL32B), and VAEs from the official source.

### Python Knowledge
- **Kind**: knowledge
- **Note**: Basic CLI skills needed to check PyTorch/CUDA versions and install wheels via pip.

## Steps

### Update and launch Comfy UI
- **Timestamp**: [03:12](https://www.youtube.com/watch?v=8HutJ9W5pTg&t=192)
- **Action**: Navigate to the Comfy folder, run the update script, and start the application.
- **Command Or Clicks**: Double click update_comfy file. Run update_comfy. Start Comfy UI.
- **Choice Branch**: Use the portable version or standard installation.

### Load Minimax workflow
- **Timestamp**: [04:00](https://www.youtube.com/watch?v=8HutJ9W5pTg&t=240)
- **Action**: Search for Minimax templates in Comfy UI and select a local workflow (Text to Video, Image to Video, or Reference to Video).
- **Command Or Clicks**: Click Templates > Search 'Minimax' > Select workflow without API tag.
- **Choice Branch**: Ignore workflows with the API tag as they run cloud models.

### Download model weights
- **Timestamp**: [05:00](https://www.youtube.com/watch?v=8HutJ9W5pTg&t=300)
- **Action**: Download the appropriate diffusion model, text encoder (Qwen 3VL32B), and VAEs based on your VRAM capacity.
- **Command Or Clicks**: Download FP8 or INT8 models to models/diffusion_models, models/text_encoders, and models/vae.
- **Choice Branch**: Full model is 66GB; FP8 is 21GB; INT8 is 34GB. Choose based on hardware.

### Configure workflow nodes
- **Timestamp**: [07:00](https://www.youtube.com/watch?v=8HutJ9W5pTg&t=420)
- **Action**: Refresh the model list and select the downloaded models in the workflow dropdowns.
- **Command Or Clicks**: Press R to refresh. Select Minimax FP8 for unit, Qwen 3VL32B for clip, and appropriate VAEs.
- **Choice Branch**: Ensure red error outlines disappear from nodes.

### Generate video
- **Timestamp**: [08:00](https://www.youtube.com/watch?v=8HutJ9W5pTg&t=480)
- **Action**: Set aspect ratio, megapixels, and duration, then run the generation.
- **Command Or Clicks**: Set aspect ratio (e.g., 16:9), megapixels (0.4 for 480p), duration. Click Run.
- **Choice Branch**: Default steps (20) and sampler are usually sufficient.

### Install Sage Attention for speed
- **Timestamp**: [14:30](https://www.youtube.com/watch?v=8HutJ9W5pTg&t=870)
- **Action**: Check PyTorch/CUDA/Python versions and install the matching Sage Attention wheel.
- **Command Or Clicks**: cmd > python -c "import torch; print(torch.__version__)". pip install <path_to_wheel>.
- **Choice Branch**: Must match CUDA, PyTorch, and Python versions exactly.

### Install KJ Nodes and Comfy Spectrum
- **Timestamp**: [16:30](https://www.youtube.com/watch?v=8HutJ9W5pTg&t=990)
- **Action**: Clone KJ Nodes and Comfy Spectrum repositories into custom_nodes and install dependencies.
- **Command Or Clicks**: git clone <URL> in custom_nodes. pip install -r requirements.txt. Restart Comfy.
- **Choice Branch**: Restart Comfy UI after installing custom nodes.

### Apply optimization nodes
- **Timestamp**: [18:00](https://www.youtube.com/watch?v=8HutJ9W5pTg&t=1080)
- **Action**: Add Patch Sage Attention, Easy Cache, and Spectrum Apply nodes to the workflow to speed up generation.
- **Command Or Clicks**: Search 'Patch Sage Attention', 'Easy Cache', 'Spectrum Apply'. Connect model outputs to BasicGuider/BasicSampler.
- **Choice Branch**: Stacking these can speed up generation by 30-40%.

## Gotchas

### API-tagged workflows run cloud models, not locally. Ensure you download the correct model size for your VRAM.
- **Severity**: blocking
- **Timestamp**: [04:30](https://www.youtube.com/watch?v=8HutJ9W5pTg&t=270)

### Sage Attention wheel must exactly match your PyTorch, CUDA, and Python versions or installation will fail.
- **Severity**: blocking
- **Timestamp**: [15:00](https://www.youtube.com/watch?v=8HutJ9W5pTg&t=900)

### Users in the US, EU, UK, and Korea are excluded from the community license and must apply for a separate license to use commercially.
- **Severity**: serious
- **Timestamp**: [21:30](https://www.youtube.com/watch?v=8HutJ9W5pTg&t=1290)

## Where to go next

Check the description for links to model weights, Sage Attention wheels, and KJ Nodes. For VRAM under 12GB, explore the 1-to-1 GP platform. For character consistency, look into training LoRAs with the Orius AI toolkit.

## Concepts surfaced

[[minimax-h3]] · [[comfy-ui-tutorial]] · [[local-ai-video]] · [[sage-attention]] · [[custom-nodes]] · [[ai-licensing]]
