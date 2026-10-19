---
video_id: UAlLD5fS7-c
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-04-10-the-best-local-ai-music-generator-is-here-free-unlimited.md
source_transcript: ../transcripts/2026-04-10-the-best-local-ai-music-generator-is-here-free-unlimited.md
source_summary_hash: sha256:93326574b2bfa9258c450574e43c5f5e75078e211b92dfec12573979d2904ea6
source_transcript_hash: sha256:0cae791b734acaf8b958fceeb29c75cd38fecd0a8673d383200dd215ae0fb450
fill_id: b7aff963-c21e-4710-be48-fcadd699b993
published_at: '2026-10-19T20:27:17.346392'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Install ACE Studio's AEP 1.5 XL locally for free, unlimited, high-quality AI music generation on consumer GPUs, even AMD and Apple Silicon.

## Prerequisites

### Git
- **Kind**: tool
- **Note**: Required to clone the AEP 1.5 repository. Install from git-scm.com if not already present.

### UV
- **Kind**: tool
- **Note**: Python package manager used for one-click installation of AEP and its dependencies.

### GPU with at least 12GB VRAM
- **Kind**: hardware
- **Note**: Minimum for AEP 1.5 XL with CPU offload and int8 quantization. 20GB recommended for full model in GPU.

### Python
- **Kind**: knowledge
- **Note**: Familiarity with command line and virtual environments helps, though UV simplifies setup.

## Steps

### Install UV via PowerShell
- **Timestamp**: [12:30](https://www.youtube.com/watch?v=UAlLD5fS7-c&t=750)
- **Action**: Open PowerShell as administrator and run the UV installer command. This installs the UV package manager needed for the AEP installation.
- **Command Or Clicks**: powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"

### Install Git
- **Timestamp**: [14:23](https://www.youtube.com/watch?v=UAlLD5fS7-c&t=863)
- **Action**: If Git is not already installed, download the installer from git-scm.com, select your OS (Windows 64-bit here), run the .exe, and accept default settings through the wizard.
- **Command Or Clicks**: Download from git-scm.com, run installer, click Next through defaults.
- **Choice Branch**: Skip if Git is already installed.

### Clone the AEP 1.5 repository
- **Timestamp**: [14:30](https://www.youtube.com/watch?v=UAlLD5fS7-c&t=870)
- **Action**: Open a command prompt in your desired installation folder (e.g., Desktop) and clone the official AEP 1.5 GitHub repository into a new folder.
- **Command Or Clicks**: git clone https://github.com/ACE-Studio/ACE-Step.git

### Install dependencies with UV
- **Timestamp**: [15:30](https://www.youtube.com/watch?v=UAlLD5fS7-c&t=930)
- **Action**: Change directory into the cloned AEP 1.5 folder and run 'uv sync' to create a virtual environment and install all required packages, including PyTorch (about 3GB).
- **Command Or Clicks**: cd ACE-Step
uv sync

### Download the XL Turbo model
- **Timestamp**: [16:30](https://www.youtube.com/watch?v=UAlLD5fS7-c&t=990)
- **Action**: In the AEP 1.5 folder, open a command prompt and use the HuggingFace CLI to download the Turbo XL model (about 20GB). Choose Turbo for speed or SFT for higher quality.
- **Command Or Clicks**: huggingface-cli download ACE-Studio/ACE-Step-XL-Turbo --local-dir checkpoints/ACE-Step-XL-Turbo
- **Choice Branch**: Use SFT model if you prefer better quality over speed.

### Launch the AEP interface
- **Timestamp**: [18:00](https://www.youtube.com/watch?v=UAlLD5fS7-c&t=1080)
- **Action**: Double-click into the AEP 1.5 folder, open a command prompt there, and run 'uv run aep'. The interface will auto-detect your GPU and enable CPU offload if needed. Then click the local URL to open the web UI.
- **Command Or Clicks**: uv run aep

### Configure and initialize the service
- **Timestamp**: [18:27](https://www.youtube.com/watch?v=UAlLD5fS7-c&t=1107)
- **Action**: In the interface, set UI language to English, confirm the checkpoint folder points to the downloaded model, and optionally enable CPU offload, int8 quantization, and compile model for faster generation. Then click 'Initialize Service'.
- **Command Or Clicks**: Click 'Initialize Service' after configuring settings.
- **Choice Branch**: Enable language model for better quality (requires more VRAM) or disable for speed.

### Generate a song
- **Timestamp**: [22:30](https://www.youtube.com/watch?v=UAlLD5fS7-c&t=1350)
- **Action**: In the generation tab, enter a prompt describing the style and lyrics with tags like [verse], [chorus]. Optionally set BPM, key, and time signature. Click 'Generate Music' and wait for the output.
- **Command Or Clicks**: Enter prompt and lyrics, click 'Generate Music'.

## Gotchas

### The Turbo model requires only 4-8 steps, while the SFT model needs 30-50 steps. Using too many steps with Turbo wastes time without quality gain.
- **Severity**: heads_up
- **Timestamp**: [21:30](https://www.youtube.com/watch?v=UAlLD5fS7-c&t=1290)

### If you enable the language model for 'think mode', it uses several more GB of VRAM and slows generation. Ensure your hardware can handle it.
- **Severity**: serious
- **Timestamp**: [18:27](https://www.youtube.com/watch?v=UAlLD5fS7-c&t=1107)

### CPU offload and int8 quantization reduce quality slightly, though the host notes the difference is barely audible.
- **Severity**: heads_up
- **Timestamp**: [10:00](https://www.youtube.com/watch?v=UAlLD5fS7-c&t=600)

### The first generation after enabling 'compile model' takes longer because it compiles the model, but subsequent generations are 10-20% faster.
- **Severity**: heads_up
- **Timestamp**: [21:53](https://www.youtube.com/watch?v=UAlLD5fS7-c&t=1313)

## Where to go next

Check out the previous AEP 1.5 tutorial for a thorough overview of all interface settings, including reference audio, inpainting, and remixing features.

## Concepts surfaced

[[open-source-ai]] · [[local-ai]] · [[music-generation]] · [[consumer-gpu]] · [[cpu-offload]] · [[int8-quantization]]
