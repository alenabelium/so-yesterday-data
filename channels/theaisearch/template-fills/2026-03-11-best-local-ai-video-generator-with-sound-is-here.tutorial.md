---
video_id: KaQbt6NYrzY
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-03-11-best-local-ai-video-generator-with-sound-is-here.md
source_transcript: ../transcripts/2026-03-11-best-local-ai-video-generator-with-sound-is-here.md
source_summary_hash: sha256:05800ee1c67d70c4d97433177c3895b1591adad7ec6e684eeafd9e86c0db4b8b
source_transcript_hash: sha256:ed2a464c2cb75742398d5f788a8783c96224493c49125361aac865f2bc112007
fill_id: f93d0b63-6fd6-46a6-9983-77953994fea2
published_at: '2026-10-19T20:36:47.831422'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Run LTX 2.3 locally with sound, even on 6GB VRAM, using the one-click WanToGP installer.

## Prerequisites

### Git
- **Kind**: tool
- **Note**: Required for cloning the WanToGP repository; install from the official Git installer.

### Miniconda
- **Kind**: tool
- **Note**: Barebones Anaconda for creating the Python 3.11 virtual environment; saves disk space.

### Windows 11
- **Kind**: os
- **Note**: Host's setup; instructions assume Windows command prompt and environment variables.

### NVIDIA GPU with 6GB VRAM
- **Kind**: hardware
- **Note**: Minimum VRAM for LTX 2.3; more RAM helps if VRAM is low.

## Steps

### Install Git
- **Timestamp**: [15:00](https://www.youtube.com/watch?v=KaQbt6NYrzY&t=900)
- **Action**: Download and install Git from the official installer page, accepting default settings.
- **Command Or Clicks**: Download Git for Windows (64-bit) → Run .exe → Click Next through all defaults.

### Clone WanToGP repository
- **Timestamp**: [16:00](https://www.youtube.com/watch?v=KaQbt6NYrzY&t=960)
- **Action**: Open Command Prompt in your chosen folder (e.g., Desktop) and clone the WanToGP GitHub repository.
- **Command Or Clicks**: cd Desktop → git clone https://github.com/WanToGP/WanToGP.git

### Install Miniconda
- **Timestamp**: [17:30](https://www.youtube.com/watch?v=KaQbt6NYrzY&t=1050)
- **Action**: Download and install Miniconda, the lightweight Anaconda distribution, to manage Python environments.
- **Command Or Clicks**: Download Miniconda installer → Run .exe → Accept defaults → Check 'Clear package cache'.

### Add Miniconda to PATH
- **Timestamp**: [19:00](https://www.youtube.com/watch?v=KaQbt6NYrzY&t=1140)
- **Action**: Add the Miniconda Scripts folder to the system PATH so 'conda' works in Command Prompt.
- **Command Or Clicks**: Search 'Edit the system environment variables' → Environment Variables → Path → New → Paste path to Miniconda Scripts.

### Create and activate virtual environment
- **Timestamp**: [20:00](https://www.youtube.com/watch?v=KaQbt6NYrzY&t=1200)
- **Action**: Create a Python 3.11 virtual environment named 'wantogp' and activate it.
- **Command Or Clicks**: conda create -n wantogp python=3.11 → conda activate wantogp

### Install PyTorch and requirements
- **Timestamp**: [21:00](https://www.youtube.com/watch?v=KaQbt6NYrzY&t=1260)
- **Action**: Install PyTorch (torch, torchvision, torchaudio) and then the rest of the WanToGP requirements via pip.
- **Command Or Clicks**: pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118 → pip install -r requirements.txt

### Launch WanToGP interface
- **Timestamp**: [22:30](https://www.youtube.com/watch?v=KaQbt6NYrzY&t=1350)
- **Action**: Start the WanToGP web interface by running the Python script, then open the provided link in your browser.
- **Command Or Clicks**: python wgp.py → Ctrl+Click the localhost link

### Select LTX 2.3 model
- **Timestamp**: [23:00](https://www.youtube.com/watch?v=KaQbt6NYrzY&t=1380)
- **Action**: In the WanToGP interface, choose LTX2 as the generator and then select version 2.3, choosing between dev and distilled.
- **Command Or Clicks**: Select 'LTX2' → Select '2.3' → Choose 'distilled' for speed or 'dev' for quality.

### Configure performance profile
- **Timestamp**: [23:30](https://www.youtube.com/watch?v=KaQbt6NYrzY&t=1410)
- **Action**: Set the memory profile in Configuration > Performance to match your hardware (e.g., high RAM, low VRAM).
- **Command Or Clicks**: Configuration → Performance → Default memory profile for video → Choose profile 2 or 3.

### Generate text-to-video
- **Timestamp**: [24:30](https://www.youtube.com/watch?v=KaQbt6NYrzY&t=1470)
- **Action**: Enter a text prompt, set resolution, aspect ratio, and frame count, then click Generate.
- **Command Or Clicks**: Enter prompt → Set resolution (up to 1080p) → Set aspect ratio (vertical supported) → Set frames (e.g., 100) → Generate

### Use first-frame image
- **Timestamp**: [27:00](https://www.youtube.com/watch?v=KaQbt6NYrzY&t=1620)
- **Action**: Upload an image to use as the first frame, adjust influence strength, and generate.
- **Command Or Clicks**: Click image upload → Drag & drop image → Set strength (default 1) → Enter prompt → Generate

### Use first and last frame images
- **Timestamp**: [28:00](https://www.youtube.com/watch?v=KaQbt6NYrzY&t=1680)
- **Action**: Upload both a start and end frame image, describe the transition, and generate.
- **Command Or Clicks**: Upload start frame → Check 'Add end frame' → Upload end frame → Enter prompt → Generate

### Use control video for motion transfer
- **Timestamp**: [29:00](https://www.youtube.com/watch?v=KaQbt6NYrzY&t=1740)
- **Action**: Upload a reference video and choose to transfer pose, depth, or edge to your new video.
- **Command Or Clicks**: Select 'Transfer human motion' → Upload reference video → Set influence (default 1) → Enter prompt → Generate

## Gotchas

### First/last frame transitions fail if the two images are too different; it results in a hard cut instead of a seamless transition.
- **Severity**: heads_up
- **Timestamp**: [11:30](https://www.youtube.com/watch?v=KaQbt6NYrzY&t=690)

### Text rendering in videos is still unreliable; use a reference image to guide it.
- **Severity**: heads_up
- **Timestamp**: [10:30](https://www.youtube.com/watch?v=KaQbt6NYrzY&t=630)

### The control video feature can produce noticeable distortions in faces and limbs.
- **Severity**: heads_up
- **Timestamp**: [29:50](https://www.youtube.com/watch?v=KaQbt6NYrzY&t=1790)

### First run downloads many large models (20GB+ total); ensure enough disk space.
- **Severity**: serious
- **Timestamp**: [25:20](https://www.youtube.com/watch?v=KaQbt6NYrzY&t=1520)

### Miniconda must be added to PATH manually; otherwise 'conda' is not recognized.
- **Severity**: blocking
- **Timestamp**: [19:00](https://www.youtube.com/watch?v=KaQbt6NYrzY&t=1140)

## Where to go next

Explore more LTX 2.3 features like vertical video and control video. For troubleshooting, paste your exact error in the comments. Subscribe to the weekly newsletter for more AI tools.

## Concepts surfaced

[[open-source-ai]] · [[local-ai]] · [[video-generation]] · [[text-to-video]] · [[image-to-video]] · [[low-vram]]
