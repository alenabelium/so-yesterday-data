---
video_id: 54YB-hjZDR4
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-01-20-open-source-suno-is-here-free-offline-ai-music-generator.md
source_transcript: ../transcripts/2026-01-20-open-source-suno-is-here-free-offline-ai-music-generator.md
source_summary_hash: sha256:1c916e8e2d5280b0b54bd52816417f3f9156c2a73d05b920508af5ff56b1638d
source_transcript_hash: sha256:acd3cf77c80d7505378eb9bcfab372013a58bf1841875a9d79846560fca243f3
fill_id: 4c454e53-49b0-41aa-ab8a-b181199f93e5
published_at: '2026-10-19T21:00:48.690477'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Install Heart Moola, an open-source AI music generator that rivals Suno v5, and run it for free, unlimited, and offline on your computer.

## Prerequisites

### Git
- **Kind**: tool
- **Note**: Required to clone the Heart Moola repository. Install from git-scm.com if not already present.

### Miniconda
- **Kind**: tool
- **Note**: Recommended to create a Python 3.10 virtual environment. Install version 3.12 or 3.11 for compatibility.

### Python 3.10
- **Kind**: knowledge
- **Note**: Heart Moola requires Python 3.10. Use Miniconda to create a virtual environment with this version.

### 16 GB VRAM GPU
- **Kind**: hardware
- **Note**: The model files total just under 16 GB, so a GPU with at least 16 GB VRAM is recommended.

## Steps

### Install Git
- **Timestamp**: [16:28](https://www.youtube.com/watch?v=54YB-hjZDR4&t=988)
- **Action**: Download the latest Git installer for your operating system and run it, accepting the default settings.
- **Command Or Clicks**: Download from git-scm.com, run the .exe, click Next through all defaults.

### Clone the Heart Moola repository
- **Timestamp**: [17:20](https://www.youtube.com/watch?v=54YB-hjZDR4&t=1040)
- **Action**: Open a command prompt in your desired folder (e.g., Desktop) and clone the Heart Moola GitHub repository.
- **Command Or Clicks**: cd Desktop, then: git clone https://github.com/heartmoola/heartmoola.git

### Create a Python 3.10 virtual environment
- **Timestamp**: [20:59](https://www.youtube.com/watch?v=54YB-hjZDR4&t=1259)
- **Action**: Use Miniconda to create a virtual environment named 'heartmoola' with Python 3.10, then activate it.
- **Command Or Clicks**: conda create -n heartmoola python=3.10, then conda activate heartmoola

### Install build dependencies
- **Timestamp**: [22:17](https://www.youtube.com/watch?v=54YB-hjZDR4&t=1337)
- **Action**: Run the provided pip command to install all required build dependencies, including torch, torchaudio, and torchvision.
- **Command Or Clicks**: pip install -e .

### Download model checkpoints
- **Timestamp**: [23:35](https://www.youtube.com/watch?v=54YB-hjZDR4&t=1415)
- **Action**: Install the huggingface_hub package and download the model checkpoints into a 'ckpt' folder. Use the Windows-compatible commands without quotes.
- **Command Or Clicks**: pip install huggingface_hub, then: hf download heartmoola/heartmoola-genen --local-dir ./ckpt

### Install Triton
- **Timestamp**: [26:05](https://www.youtube.com/watch?v=54YB-hjZDR4&t=1565)
- **Action**: Install a pre-built Triton 2.1 wheel for Windows to avoid long compilation times. Download the wheel and install it with pip.
- **Command Or Clicks**: pip install "path/to/triton-2.1.0-cp310-cp310-win_amd64.whl"

### Generate a song
- **Timestamp**: [27:10](https://www.youtube.com/watch?v=54YB-hjZDR4&t=1630)
- **Action**: Activate the virtual environment, then run the music generation script. Edit the tags.txt and lyrics.txt files in the assets folder to customize your song.
- **Command Or Clicks**: conda activate heartmoola, then: python examples/run_music_generation.py

## Gotchas

### The model files total just under 16 GB, so you need at least 16 GB of VRAM to run it.
- **Severity**: blocking
- **Timestamp**: [14:30](https://www.youtube.com/watch?v=54YB-hjZDR4&t=870)

### Python 3.13 tends not to work well with the latest AI models; use 3.12 or 3.11.
- **Severity**: serious
- **Timestamp**: [18:30](https://www.youtube.com/watch?v=54YB-hjZDR4&t=1110)

### The provided download commands use quotes that don't work on Windows; remove the quotes when typing them.
- **Severity**: blocking
- **Timestamp**: [23:35](https://www.youtube.com/watch?v=54YB-hjZDR4&t=1415)

### Triton 3 does not work with Heart Moola; you must use version 2.1.
- **Severity**: blocking
- **Timestamp**: [27:10](https://www.youtube.com/watch?v=54YB-hjZDR4&t=1630)

### Generating a new song overwrites the existing output.mp3 file; copy or rename it to save it.
- **Severity**: heads_up
- **Timestamp**: [31:29](https://www.youtube.com/watch?v=54YB-hjZDR4&t=1889)

## Where to go next

Heart Moola is a game-changer for open-source AI music. If you run into issues, share your error messages in the comments. Stay tuned for more AI tools and news in my weekly newsletter.

## Concepts surfaced

[[open-source-ai]] · [[ai-music-generation]] · [[local-ai]]
