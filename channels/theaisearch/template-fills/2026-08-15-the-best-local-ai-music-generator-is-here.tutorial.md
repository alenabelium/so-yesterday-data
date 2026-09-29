---
video_id: aUcDyeZgz_k
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-08-15-the-best-local-ai-music-generator-is-here.md
source_transcript: ../transcripts/2026-08-15-the-best-local-ai-music-generator-is-here.md
source_summary_hash: sha256:a284a9bdcb4151d8818ff5a3c4c48323f1076b11066da61a72c39522a9eb8a64
source_transcript_hash: sha256:b96a41f4f07f07a59d808f3a7df01de7a6ce44f4f0b9a8182ea145ea5ac0d91f
fill_id: 7f6b8b8c-1b7b-41c6-a3f0-753f3676468e
published_at: '2026-09-29T11:22:35.910253'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Install Miniax Music in Comfy UI for unlimited, offline AI song generation with detailed prompt structuring.

## Prerequisites

### Comfy UI
- **Kind**: tool
- **Note**: Latest version installed and updated via update_comfy.bat.

### Consumer GPU
- **Kind**: hardware
- **Note**: Must support VRAM for models ranging from 2.5GB to 9.8GB.

### Miniax Models
- **Kind**: tool
- **Note**: Diffusion model, text encoder, and VAE downloaded from Hugging Face.

## Steps

### Update Comfy UI
- **Timestamp**: [11:22](https://www.youtube.com/watch?v=aUcDyeZgz_k&t=682)
- **Action**: Navigate to the Comfy folder, open the update folder, and run the batch file to update to the latest version.
- **Command Or Clicks**: Click update_comfy.bat

### Load Miniax Workflow
- **Timestamp**: [11:22](https://www.youtube.com/watch?v=aUcDyeZgz_k&t=682)
- **Action**: Open Comfy UI, go to Templates, search for 'music', and select the Miniax text to music workflow.
- **Command Or Clicks**: Templates > Search 'music' > Miniax text to music

### Download Diffusion Model
- **Timestamp**: [12:53](https://www.youtube.com/watch?v=aUcDyeZgz_k&t=773)
- **Action**: Download the diffusion model (e.g., FP16 9.8GB or int8 2.5GB) and save it to the diffusion_models folder.
- **Command Or Clicks**: Save to Comfy UI/models/diffusion_models

### Download Text Encoder
- **Timestamp**: [12:53](https://www.youtube.com/watch?v=aUcDyeZgz_k&t=773)
- **Action**: Download the text encoder (e.g., 9.2GB) and save it to the text_encoders folder.
- **Command Or Clicks**: Save to Comfy UI/models/text_encoders

### Download VAE
- **Timestamp**: [12:53](https://www.youtube.com/watch?v=aUcDyeZgz_k&t=773)
- **Action**: Download the VAE (217MB) and save it to the VAE folder.
- **Command Or Clicks**: Save to Comfy UI/models/VAE

### Refresh and Select Models
- **Timestamp**: [12:53](https://www.youtube.com/watch?v=aUcDyeZgz_k&t=773)
- **Action**: Press R to refresh the model list in Comfy UI and select the downloaded models from the dropdowns.
- **Command Or Clicks**: Press R > Select models from dropdowns

### Configure Prompt and Lyrics
- **Timestamp**: [13:39](https://www.youtube.com/watch?v=aUcDyeZgz_k&t=819)
- **Action**: Enter song description (genre, feel, pace), vocal details, and arrangements in the prompt field. Add lyrics with metatags like [intro] or [verse].
- **Command Or Clicks**: Input text into prompt and lyrics fields

### Set Duration and Seed
- **Timestamp**: [13:39](https://www.youtube.com/watch?v=aUcDyeZgz_k&t=819)
- **Action**: Set the maximum duration in seconds (up to 300) and choose a seed for reproducibility.
- **Command Or Clicks**: Set duration slider > Enter seed value

### Adjust VRAM Settings
- **Timestamp**: [15:10](https://www.youtube.com/watch?v=aUcDyeZgz_k&t=910)
- **Action**: Disable tiled encode if you have high VRAM (16GB+) for better quality, or enable it for low VRAM systems.
- **Command Or Clicks**: Toggle tiled encode off

### Generate Song
- **Timestamp**: [15:57](https://www.youtube.com/watch?v=aUcDyeZgz_k&t=957)
- **Action**: Click run to generate the song. Adjust step count and CFG for quality vs. speed trade-offs.
- **Command Or Clicks**: Click run

## Gotchas

### Miniax currently only supports text-to-music; you cannot create covers or music-to-music directly yet.
- **Severity**: heads_up
- **Timestamp**: [13:39](https://www.youtube.com/watch?v=aUcDyeZgz_k&t=819)

### Tiled encode reduces VRAM usage; disable it if you have 16GB+ VRAM for faster, higher quality results.
- **Severity**: serious
- **Timestamp**: [15:10](https://www.youtube.com/watch?v=aUcDyeZgz_k&t=910)

### Sunno now limits paid users to 20 downloads/month and adds watermarks, making local tools like Miniax critical.
- **Severity**: serious
- **Timestamp**: [16:55](https://www.youtube.com/watch?v=aUcDyeZgz_k&t=1015)

## Where to go next

Use AEP 1.5 XL for inpainting and Muse Scriptor for MIDI extraction to extend Miniax Music's capabilities.

## Concepts surfaced

[[miniax-music]] · [[comfy-ui]] · [[local-ai-music]] · [[open-source-generative-ai]] · [[music-generation-tutorial]]
