---
video_id: CMuwP0u-Sjg
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-03-20-finally-ai-for-music-production-free-open-source.md
source_transcript: ../transcripts/2026-03-20-finally-ai-for-music-production-free-open-source.md
source_summary_hash: sha256:301d428d558211651a7c6bf425a0af733d73eaadffc541a3b69d28b40da29382
source_transcript_hash: sha256:2d1a46364b7137b8478c401e0f88a0d62850a6293cf832ae2067ef3dd1b1ca70
fill_id: 9c2833ba-9713-443f-83c0-9a50073c54ab
published_at: '2026-10-19T20:36:40.506583'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Generate musically coherent stems that follow BPM, key, and bar count, then layer them in a DAW to build a full song.

## Prerequisites

### Git
- **Kind**: tool
- **Note**: Required to clone the RC Stable Audio Tools repository. Install from git-scm.com if not already present.

### Miniconda
- **Kind**: tool
- **Note**: Recommended for creating a Python 3.10 virtual environment. Lightweight alternative to Anaconda.

### Python 3.10
- **Kind**: knowledge
- **Note**: Use Python 3.10 specifically; newer versions can fail dependency resolution.

### CUDA GPU with 8GB+ VRAM
- **Kind**: hardware
- **Note**: Official version requires at least 8GB VRAM; 16GB VRAM generates a track in about 15 seconds.

## Steps

### Install Git
- **Timestamp**: [16:39](https://www.youtube.com/watch?v=CMuwP0u-Sjg&t=999)
- **Action**: Download and install Git from the official site, selecting the appropriate version for your operating system. Follow the installer defaults.
- **Command Or Clicks**: Download Git for Windows (64-bit) and run the .exe, clicking Next through the default options.

### Clone the RC Stable Audio Tools repository
- **Timestamp**: [17:19](https://www.youtube.com/watch?v=CMuwP0u-Sjg&t=1039)
- **Action**: Open Command Prompt in your desired directory (e.g., Desktop) and clone the repository using Git.
- **Command Or Clicks**: cd Desktop
cmd
git clone https://github.com/RC-Studio/RC-Stable-Audio-Tools.git

### Install Miniconda
- **Timestamp**: [19:29](https://www.youtube.com/watch?v=CMuwP0u-Sjg&t=1169)
- **Action**: Download and install Miniconda from the official site, then add it to your system PATH.
- **Command Or Clicks**: Download Miniconda installer, run it, then add the Scripts folder to PATH via Environment Variables.

### Create and activate a Python 3.10 virtual environment
- **Timestamp**: [21:21](https://www.youtube.com/watch?v=CMuwP0u-Sjg&t=1281)
- **Action**: Use Conda to create a virtual environment named 'stable-audio' with Python 3.10, then activate it.
- **Command Or Clicks**: conda create -n stable-audio python=3.10
conda activate stable-audio

### Install PyTorch with CUDA support
- **Timestamp**: [22:50](https://www.youtube.com/watch?v=CMuwP0u-Sjg&t=1370)
- **Action**: Install the CUDA version of PyTorch before other dependencies to ensure GPU acceleration.
- **Command Or Clicks**: pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118

### Install stable-audio-tools and dependencies
- **Timestamp**: [23:21](https://www.youtube.com/watch?v=CMuwP0u-Sjg&t=1401)
- **Action**: Install the stable-audio-tools package and all required dependencies from the repository's requirements.
- **Command Or Clicks**: pip install -r requirements.txt

### Launch the Gradio interface
- **Timestamp**: [24:47](https://www.youtube.com/watch?v=CMuwP0u-Sjg&t=1487)
- **Action**: Start the Gradio interface by running the provided Python script, then open the local URL in your browser.
- **Command Or Clicks**: python run_gradio.py

### Download the Foundation One model
- **Timestamp**: [25:38](https://www.youtube.com/watch?v=CMuwP0u-Sjg&t=1538)
- **Action**: In the interface, select the Foundation One model and click Download. After completion, restart the interface.
- **Command Or Clicks**: Select Foundation 1 model, click Download, then restart the interface.

### Generate your first audio clip
- **Timestamp**: [27:33](https://www.youtube.com/watch?v=CMuwP0u-Sjg&t=1653)
- **Action**: Enter a prompt, set the number of bars, BPM, and key, then click Generate. Adjust sampler parameters if desired.
- **Command Or Clicks**: Enter prompt, set bars=8, BPM=128, key=F minor, click Generate.

### Download MIDI and use style transfer
- **Timestamp**: [28:48](https://www.youtube.com/watch?v=CMuwP0u-Sjg&t=1728)
- **Action**: Download the MIDI file to use with other instruments, or upload a reference clip for style transfer to modify or replace instruments.
- **Command Or Clicks**: Click Download MIDI, or upload a clip, set influence, and click Generate.

## Gotchas

### Use Python 3.10 specifically; newer versions like 3.11 or beyond can fail dependency resolution.
- **Severity**: blocking
- **Timestamp**: [21:21](https://www.youtube.com/watch?v=CMuwP0u-Sjg&t=1281)

### The official version requires at least 8 GB of VRAM; lower VRAM may not work without quantized versions.
- **Severity**: blocking
- **Timestamp**: [15:30](https://www.youtube.com/watch?v=CMuwP0u-Sjg&t=930)

### Percussion and drum sounds are outside the scope of Foundation One; you'll need to add them manually.
- **Severity**: heads_up
- **Timestamp**: [10:14](https://www.youtube.com/watch?v=CMuwP0u-Sjg&t=614)

### The model only works with specific BPMs; you cannot use faster or slower tempos.
- **Severity**: heads_up
- **Timestamp**: [14:49](https://www.youtube.com/watch?v=CMuwP0u-Sjg&t=889)

### The Comfy UI node does not include style transfer; use the Gradio interface for that feature.
- **Severity**: heads_up
- **Timestamp**: [31:30](https://www.youtube.com/watch?v=CMuwP0u-Sjg&t=1890)

## Where to go next

Check out other music generators like AEP 1.5 and Heart Moola on this channel, and subscribe to the weekly newsletter for the latest AI tools.

## Concepts surfaced

[[open-source-ai]] · [[music-generation]] · [[stable-audio]] · [[gradio-interface]] · [[midi-export]] · [[style-transfer]]
