---
video_id: CMuwP0u-Sjg
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-03-20-finally-ai-for-music-production-free-open-source.md
source_transcript: ../transcripts/2026-03-20-finally-ai-for-music-production-free-open-source.md
source_summary_hash: sha256:4bcf0d3f02b07fc5c2a30696fdccf8a5c6bdbe2ffd01f8c63a272552090a5fa0
source_transcript_hash: sha256:2d1a46364b7137b8478c401e0f88a0d62850a6293cf832ae2067ef3dd1b1ca70
fill_id: 8484fad7-3701-4914-9a19-0bb64f2c2415
published_at: '2026-05-19T04:50:03.628835'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Install and use Foundation One, a free open-source AI model for generating musically coherent stems and MIDI files for music production.

## Prerequisites

### GPU with 8GB+ VRAM
- **Kind**: hardware
- **Note**: Minimum 8 GB VRAM required; 16 GB recommended for speed.

### Git
- **Kind**: tool
- **Note**: Required to clone the repository; install via OS-specific installer.

### Miniconda
- **Kind**: tool
- **Note**: Recommended over Anaconda for virtual environment management and space efficiency.

### Python 3.10
- **Kind**: tool
- **Note**: Specific version required; newer versions may fail dependency resolution.

### CUDA GPU
- **Kind**: hardware
- **Note**: NVIDIA GPU required to install CUDA-specific PyTorch dependencies.

## Steps

### Install Git
- **Timestamp**: [16:39](https://www.youtube.com/watch?v=CMuwP0u-Sjg&t=999)
- **Action**: Download and install Git for your operating system to enable repository cloning.
- **Command Or Clicks**: Download .exe for Windows or equivalent for your OS, run installer, click Next through defaults.

### Clone Repository
- **Timestamp**: [17:45](https://www.youtube.com/watch?v=CMuwP0u-Sjg&t=1065)
- **Action**: Open command prompt in your desired directory and clone the RC Stable Audio Tools repository.
- **Command Or Clicks**: cmd
git clone <repository_url>

### Navigate to Folder
- **Timestamp**: [18:15](https://www.youtube.com/watch?v=CMuwP0u-Sjg&t=1095)
- **Action**: Change directory into the newly cloned RC stable audio tools folder.
- **Command Or Clicks**: cd <rc-stable-audio-tools-folder>

### Install Miniconda
- **Timestamp**: [19:29](https://www.youtube.com/watch?v=CMuwP0u-Sjg&t=1169)
- **Action**: Download and install Miniconda, then add it to your system PATH to enable conda commands.
- **Command Or Clicks**: Download installer, run exe, agree to terms, set for all users, add to PATH via System Environment Variables.

### Create Virtual Environment
- **Timestamp**: [21:21](https://www.youtube.com/watch?v=CMuwP0u-Sjg&t=1281)
- **Action**: Create a new virtual environment named 'stable-audio' using Python 3.10.
- **Command Or Clicks**: conda create -n stable-audio python=3.10

### Activate Environment
- **Timestamp**: [22:05](https://www.youtube.com/watch?v=CMuwP0u-Sjg&t=1325)
- **Action**: Activate the newly created virtual environment.
- **Command Or Clicks**: conda activate stable-audio

### Install CUDA PyTorch
- **Timestamp**: [22:45](https://www.youtube.com/watch?v=CMuwP0u-Sjg&t=1365)
- **Action**: Install PyTorch, TorchVision, and TorchAudio for CUDA if you have an NVIDIA GPU.
- **Command Or Clicks**: pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118

### Install Stable Audio Tools
- **Timestamp**: [23:05](https://www.youtube.com/watch?v=CMuwP0u-Sjg&t=1385)
- **Action**: Install the stable audio tools package and its dependencies.
- **Command Or Clicks**: pip install stable-audio-tools

### Install Additional Dependencies
- **Timestamp**: [23:30](https://www.youtube.com/watch?v=CMuwP0u-Sjg&t=1410)
- **Action**: Install remaining dependencies required by RC Stable Audio.
- **Command Or Clicks**: pip install <additional_dependencies>

### Launch Gradio Interface
- **Timestamp**: [24:15](https://www.youtube.com/watch?v=CMuwP0u-Sjg&t=1455)
- **Action**: Start the Gradio interface by running the Python script.
- **Command Or Clicks**: python run_gradio.py

### Download Model
- **Timestamp**: [25:00](https://www.youtube.com/watch?v=CMuwP0u-Sjg&t=1500)
- **Action**: Open the local Gradio link in a browser and download the Foundation One model.
- **Command Or Clicks**: Click link in terminal, click 'Download' for Foundation One model.

### Restart Interface
- **Timestamp**: [25:30](https://www.youtube.com/watch?v=CMuwP0u-Sjg&t=1530)
- **Action**: Exit the terminal, reactivate the environment, and restart the Gradio interface.
- **Command Or Clicks**: python run_gradio.py

### Generate Audio
- **Timestamp**: [26:30](https://www.youtube.com/watch?v=CMuwP0u-Sjg&t=1590)
- **Action**: Enter a prompt, set bars/BPM/key, and generate audio clips.
- **Command Or Clicks**: Enter prompt in text box, adjust settings, click Generate.

### Use Style Transfer
- **Timestamp**: [29:00](https://www.youtube.com/watch?v=CMuwP0u-Sjg&t=1740)
- **Action**: Upload a reference clip to apply its style to a new generation.
- **Command Or Clicks**: Upload audio file, check 'Use for style transfer', adjust influence slider, enter new prompt.

## Gotchas

### Newer Python versions (3.11+) may fail dependency resolution; use Python 3.10.
- **Severity**: blocking
- **Timestamp**: [21:21](https://www.youtube.com/watch?v=CMuwP0u-Sjg&t=1281)

### Percussion and drum sounds are outside the scope of this AI model.
- **Severity**: serious
- **Timestamp**: [10:14](https://www.youtube.com/watch?v=CMuwP0u-Sjg&t=614)

### Only specific BPMs are supported; you cannot use faster or slower tempos than listed.
- **Severity**: serious
- **Timestamp**: [14:49](https://www.youtube.com/watch?v=CMuwP0u-Sjg&t=889)

### Instruments not in the training list may not generate good samples.
- **Severity**: heads_up
- **Timestamp**: [14:49](https://www.youtube.com/watch?v=CMuwP0u-Sjg&t=889)

## Where to go next

Check out other music generators like AEP 1.5 and Heart Moola on the channel. Subscribe to the free weekly newsletter for AI updates.

## Concepts surfaced

[[foundation-one]] · [[open-source-ai]] · [[music-production]] · [[gradio-interface]] · [[virtual-environment]] · [[midi-generation]]
