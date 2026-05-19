---
video_id: UAlLD5fS7-c
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-04-10-the-best-local-ai-music-generator-is-here-free-unlimited.md
source_transcript: ../transcripts/2026-04-10-the-best-local-ai-music-generator-is-here-free-unlimited.md
source_summary_hash: sha256:a8278d9c2ca23f610be5737659f6335beb3f6ca043eaece868bdc54717c9c815
source_transcript_hash: sha256:0cae791b734acaf8b958fceeb29c75cd38fecd0a8673d383200dd215ae0fb450
fill_id: 5eeffd40-fc91-464b-b475-89be6711cb9e
published_at: '2026-05-19T08:14:16.645336'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Install and run ACE Studio's AEP 1.5 XL locally for free, unlimited, high-quality music generation with full vocal and instrumental support.

## Prerequisites

### Consumer GPU
- **Kind**: hardware
- **Note**: Minimum 12 GB VRAM with offloading; 20 GB recommended for full GPU fit.

### Python Environment
- **Kind**: tool
- **Note**: UV installer and Git must be installed on your OS.

### HuggingFace Account
- **Kind**: account
- **Note**: Required to download the model weights via CLI.

## Steps

### Install UV and Git
- **Timestamp**: [13:00](https://www.youtube.com/watch?v=UAlLD5fS7-c&t=780)
- **Action**: Open PowerShell as admin and paste the UV installation line. Then download and run the Git installer for your OS.
- **Command Or Clicks**: PowerShell: [Paste UV install line] + Enter. Git: Download .exe, click Next through defaults.
- **Choice Branch**: Skip Git install if already present.

### Clone Repository
- **Timestamp**: [14:23](https://www.youtube.com/watch?v=UAlLD5fS7-c&t=863)
- **Action**: Open Command Prompt in your desired folder and clone the AEP 1.5 repo.
- **Command Or Clicks**: cmd: [Paste git clone line] + Enter.
- **Choice Branch**: None

### Install Dependencies
- **Timestamp**: [15:27](https://www.youtube.com/watch?v=UAlLD5fS7-c&t=927)
- **Action**: Navigate to the repo folder and use UV to sync the virtual environment and install packages.
- **Command Or Clicks**: cd aep-1.5 && uv sync
- **Choice Branch**: None

### Download Model
- **Timestamp**: [17:25](https://www.youtube.com/watch?v=UAlLD5fS7-c&t=1045)
- **Action**: Open cmd in the repo folder and use the HuggingFace CLI to download the Turbo XL model.
- **Command Or Clicks**: huggingface-cli download [Turbo XL repo path]
- **Choice Branch**: Choose SFT for quality or Turbo for speed.

### Launch Interface
- **Timestamp**: [18:27](https://www.youtube.com/watch?v=UAlLD5fS7-c&t=1107)
- **Action**: Open cmd in the repo folder and run the AEP interface command.
- **Command Or Clicks**: uv run aep
- **Choice Branch**: None

### Configure Settings
- **Timestamp**: [19:00](https://www.youtube.com/watch?v=UAlLD5fS7-c&t=1140)
- **Action**: In the UI, select language, device, and enable CPU offload/int8 quantization if VRAM is low. Click Initialize Service.
- **Command Or Clicks**: UI: Check 'Offload to CPU', check 'Int8 Quantization', click 'Initialize Service'.
- **Choice Branch**: Enable Flash Attention if installed.

### Generate Music
- **Timestamp**: [21:53](https://www.youtube.com/watch?v=UAlLD5fS7-c&t=1313)
- **Action**: Enter style prompt and lyrics in the generation tab, set steps (4-8 for Turbo), and click Generate.
- **Command Or Clicks**: UI: Input prompt/lyrics, set steps=6, click 'Generate Music'.
- **Choice Branch**: Add optional BPM/key tags.

## Gotchas

### VRAM requirements are high; 12GB is minimum with offloading, 20GB recommended for full GPU fit.
- **Severity**: blocking
- **Timestamp**: [10:27](https://www.youtube.com/watch?v=UAlLD5fS7-c&t=627)

### Int8 quantization and CPU offload may slightly reduce quality but are necessary for lower VRAM.
- **Severity**: heads_up
- **Timestamp**: [10:27](https://www.youtube.com/watch?v=UAlLD5fS7-c&t=627)

### First generation takes longer due to model compilation; subsequent runs are faster.
- **Severity**: heads_up
- **Timestamp**: [19:00](https://www.youtube.com/watch?v=UAlLD5fS7-c&t=1140)

## Where to go next

Check the linked GitHub repo for detailed documentation. Explore the previous AEP 1.5 tutorial for advanced features like inpainting and reference audio style copying.

## Concepts surfaced

[[local-ai-music]] · [[ace-studio]] · [[aep-1-5-xl]] · [[open-source-ai]] · [[gpu-offloading]] · [[huggingface-cli]]
