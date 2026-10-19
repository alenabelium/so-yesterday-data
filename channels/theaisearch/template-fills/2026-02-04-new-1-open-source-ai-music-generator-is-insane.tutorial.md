---
video_id: QzddQoCKKss
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-02-04-new-1-open-source-ai-music-generator-is-insane.md
source_transcript: ../transcripts/2026-02-04-new-1-open-source-ai-music-generator-is-insane.md
source_summary_hash: sha256:bf00f20e42772f76e6a2be1d7f08bc458f1f07408a21a703bb9f984a95bb2932
source_transcript_hash: sha256:d8c747b4fa1d8ebe8c5436df5a55cea409f798cf3b00e1673b173340b24635b3
fill_id: d0f07c9c-abaa-4a5a-875f-dc7242e85f0e
published_at: '2026-10-19T20:50:04.942730'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

AEP 1.5, an open-source AI music generator, runs locally on low VRAM or CPU and produces studio-grade tracks across genres and languages.

## Prerequisites

### Python 3.11
- **Kind**: tool
- **Note**: Recommended version for AEP 1.5; ensure it's installed before starting.

### CUDA GPU (optional)
- **Kind**: hardware
- **Note**: Recommended for faster generation, but not required; CPU works but slower.

### UV package manager
- **Kind**: tool
- **Note**: Install via terminal; handles dependencies and virtual environment.

### Git
- **Kind**: tool
- **Note**: Required to clone the repository; install from git-scm.com if missing.

### Windows PowerShell (or Mac/Linux terminal)
- **Kind**: os
- **Note**: Used for installation commands; run as administrator on Windows.

## Steps

### Install UV package manager
- **Timestamp**: [12:15](https://www.youtube.com/watch?v=QzddQoCKKss&t=735)
- **Action**: Open PowerShell as administrator (Windows) or terminal (Mac/Linux) and run the UV installer command. Wait for the success message.
- **Command Or Clicks**: Windows: `irm https://astral.sh/uv/install.ps1 | iex`; Mac/Linux: `curl -LsSf https://astral.sh/uv/install.sh | sh`

### Install Git (if not already installed)
- **Timestamp**: [13:22](https://www.youtube.com/watch?v=QzddQoCKKss&t=802)
- **Action**: Download Git for your OS from git-scm.com, run the installer, and follow the default settings.
- **Command Or Clicks**: Click 'Download for Windows' (or your OS), run the .exe, click 'Next' through defaults.
- **Choice Branch**: Skip if Git is already installed.

### Clone the AEP 1.5 repository
- **Timestamp**: [14:35](https://www.youtube.com/watch?v=QzddQoCKKss&t=875)
- **Action**: Open Command Prompt in your desired folder (e.g., Desktop) and clone the GitHub repo.
- **Command Or Clicks**: `git clone https://github.com/AEP-1.5/AEP-1.5.git`

### Install dependencies with UV sync
- **Timestamp**: [15:44](https://www.youtube.com/watch?v=QzddQoCKKss&t=944)
- **Action**: Change directory into the cloned folder and run UV sync to install all dependencies and create a virtual environment.
- **Command Or Clicks**: `cd AEP-1.5` then `uv sync`

### Run the interface
- **Timestamp**: [16:30](https://www.youtube.com/watch?v=QzddQoCKKss&t=990)
- **Action**: Double-click into the AEP folder, open Command Prompt, and run the app. Then open the local URL in your browser.
- **Command Or Clicks**: `uv run aep` then Ctrl+click the link (e.g., http://127.0.0.1:7860)

### Initialize the service
- **Timestamp**: [23:52](https://www.youtube.com/watch?v=QzddQoCKKss&t=1432)
- **Action**: In the interface, click 'Initialize service' to auto-download models. Wait for 'model initialized successfully on CUDA' message.
- **Command Or Clicks**: Click 'Initialize service'

### Generate music with text prompt
- **Timestamp**: [24:58](https://www.youtube.com/watch?v=QzddQoCKKss&t=1498)
- **Action**: Select 'text to music' task, enter a prompt (simple or custom), optionally set language, BPM, duration, and click generate.
- **Command Or Clicks**: Enter prompt, click 'Generate'
- **Choice Branch**: Choose 'simple' for auto lyrics or 'custom' for manual caption/lyrics.

### Use repaint to micro-edit a song
- **Timestamp**: [29:42](https://www.youtube.com/watch?v=QzddQoCKKss&t=1782)
- **Action**: Upload an audio file, set repaint start/end times, modify lyrics, and generate to replace that section.
- **Command Or Clicks**: Upload audio, set start/end, edit lyrics, click 'Generate'

### Create a cover song
- **Timestamp**: [31:04](https://www.youtube.com/watch?v=QzddQoCKKss&t=1864)
- **Action**: Select 'cover' task, upload source audio, enter lyrics, set a new style caption, and adjust cover strength in advanced settings.
- **Command Or Clicks**: Upload audio, set caption, adjust 'audio cover strength', click 'Generate'

## Gotchas

### If you get an error during initialization, you may need to initialize the service, exit, and restart the app before it works.
- **Severity**: heads_up
- **Timestamp**: [24:00](https://www.youtube.com/watch?v=QzddQoCKKss&t=1440)

### The language model (LM) is optional; if you have under 6GB VRAM, disable it to avoid issues.
- **Severity**: serious
- **Timestamp**: [20:19](https://www.youtube.com/watch?v=QzddQoCKKss&t=1219)

### Generated songs are not saved by default; you must click the save button to keep them.
- **Severity**: heads_up
- **Timestamp**: [28:47](https://www.youtube.com/watch?v=QzddQoCKKss&t=1727)

### The base model requires more steps and takes longer; use turbo models for speed.
- **Severity**: heads_up
- **Timestamp**: [19:30](https://www.youtube.com/watch?v=QzddQoCKKss&t=1170)

### The 'think' and 'parallel thinking' features require the language model to be initialized; otherwise they won't work.
- **Severity**: blocking
- **Timestamp**: [28:29](https://www.youtube.com/watch?v=QzddQoCKKss&t=1709)

## Where to go next

Now that you've mastered AEP 1.5, explore training your own LoRA for custom styles. Check the GitHub repo for model options and stay tuned for a dedicated LoRA tutorial.

## Concepts surfaced

[[open-source-ai]] · [[ai-music-generation]] · [[local-inference]] · [[gradio-interface]] · [[lora-fine-tuning]]
