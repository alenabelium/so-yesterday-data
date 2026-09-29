---
video_id: pC6KHflGye0
template_id: tech-overview
template_version: 1
source_summary: ../summaries/2026-05-24-ai-co-scientist-ai-for-dna-ai-npcs-open-source-robots-new-qw.md
source_transcript: ../transcripts/2026-05-24-ai-co-scientist-ai-for-dna-ai-npcs-open-source-robots-new-qw.md
source_summary_hash: sha256:b17f6aae72a97a14eb6ec5cb4c5029d5e1cd0f9a18da8d381f6d4d8aad6d9727
source_transcript_hash: sha256:fcf6b9b76fa9c74a424fa994dcf4d1c06c598dc5831a99d8d67d265d0d5b3ee1
fill_id: 1eacd0f9-094e-406e-9616-54c82c4c8416
published_at: '2026-05-31T00:57:15.073984'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Bite Dance's Lance ships a 3B unified model that generates and edits both video and images, while Alibaba's Qwen 3.7 Max targets agentic coding and Google DeepMind reveals a multi-agent AI co-scientist.

## Tools covered

### Lance
- **Vendor**: Bite Dance
- **Category**: multimodal
- **Timestamp**: [01:15](https://www.youtube.com/watch?v=pC6KHflGye0&t=75)
- **Why It Matters**: A 3B-parameter unified multimodal model that does text-to-video, multi-turn video editing, text-to-image, image editing, and visual understanding in one model, described as Nano Banana for video.
- **Sota Comparison**: Video quality isn't state-of-the-art, but the unified scope across video, image, and understanding is the point.
- **Sota Band**: new
- **Access Constraint**: Open code; needs 40GB+ VRAM GPU

### LTO
- **Vendor**: Apple
- **Category**: world-model
- **Timestamp**: [03:32](https://www.youtube.com/watch?v=pC6KHflGye0&t=212)
- **Why It Matters**: Surface light field tokenization renders a full 3D model from an input image and captures how the object looks from different viewpoints, not just its shape, which matters for shiny or reflective surfaces.
- **Sota Comparison**: On average more accurate and faithful than Trellis, another leading 3D model generator.
- **Sota Band**: beats
- **Access Constraint**: Open code plus training script

### Flash GRPO
- **Category**: video
- **Timestamp**: [05:18](https://www.youtube.com/watch?v=pC6KHflGye0&t=318)
- **Why It Matters**: Aligns large video models to human preferences by sampling a single time step instead of the full diffusion trajectory, cutting the hundreds of GPU-days alignment usually costs while improving detail and motion.
- **Sota Comparison**: Learns and improves faster than the Flow GRPO Fast alignment method.
- **Sota Band**: beats
- **Access Constraint**: Open GitHub repo with training code

### Reactive GWM
- **Category**: world-model
- **Timestamp**: [06:49](https://www.youtube.com/watch?v=pC6KHflGye0&t=409)
- **Why It Matters**: A reactive game world model where NPCs can be steered with high-level strategies like offense or defense, separating player button inputs from NPC behavior injected via cross attention, pointing toward controllable game simulation.
- **Sota Band**: new
- **Access Constraint**: Open GitHub; uses Wan 2.2 base, runs on mid/high GPUs

### L2P
- **Category**: image
- **Timestamp**: [07:57](https://www.youtube.com/watch?v=pC6KHflGye0&t=477)
- **Why It Matters**: An image model that removes the VAE and latent space to generate directly in pixel space, handling up to 4K resolution with 8K extrapolation and very high detail and accuracy.
- **Sota Comparison**: The most performant pixel-based diffusion model so far; quality beats open latent models like Qwen and Zimage Turbo.
- **Sota Band**: beats
- **Access Constraint**: Open code; 1K model only, ~20GB

### Carbon
- **Category**: other
- **Timestamp**: [10:09](https://www.youtube.com/watch?v=pC6KHflGye0&t=609)
- **Why It Matters**: An open-source DNA foundation model that reads the four-letter language of DNA, processing nearly 400,000 base pairs at once to continue sequences, score genetic variants, or predict protein 3D structure.
- **Sota Comparison**: Claimed fastest open DNA model, ~275x faster than medium EVO 2, though the larger EVO 2 still has the highest win rate.
- **Sota Band**: beats
- **Access Constraint**: Open code; 500M model ~1GB, plus GGUF

### LongCat Video Avatar 1.5
- **Vendor**: Meituan
- **Category**: video
- **Timestamp**: [12:00](https://www.youtube.com/watch?v=pC6KHflGye0&t=720)
- **Why It Matters**: An avatar generator that takes a reference image plus audio and makes that person speak naturally, now more stable and expressive, supporting different art styles and multi-person interaction.
- **Sota Band**: new
- **Access Constraint**: Open models; int8 version ~16GB

### Mega ASR
- **Category**: asr
- **Timestamp**: [14:55](https://www.youtube.com/watch?v=pC6KHflGye0&t=895)
- **Why It Matters**: A speech recognition model built for messy real-world audio with noise, echo, reverb, clipping, and bad microphones, trained on 2.6M samples across seven acoustic problems to transcribe where others fail.
- **Sota Comparison**: Lowest error rate vs Gemini 3 Pro and Qwen 3 ASR; claimed ~30% gains in difficult acoustics.
- **Sota Band**: beats
- **Access Constraint**: Open code plus fine-tune script; under 5GB

### HYMT2
- **Vendor**: Tencent
- **Category**: other
- **Timestamp**: [17:09](https://www.youtube.com/watch?v=pC6KHflGye0&t=1029)
- **Why It Matters**: An open multilingual translation family (30B MoE with 3B active, plus 7B and 1.8B) across 33 languages, designed to follow detailed instructions like preserving formatting, style, terminology, and delimiters.
- **Sota Comparison**: Beats larger open models like DeepSeek V4 on instruction following and specialized-domain translation.
- **Sota Band**: beats
- **Access Constraint**: Open; 1.8B ~4GB, plus FP8 and GGUF

### AI co-scientist
- **Vendor**: Google DeepMind
- **Category**: agent
- **Timestamp**: [23:46](https://www.youtube.com/watch?v=pC6KHflGye0&t=1426)
- **Why It Matters**: A multi-agent system where specialized agents debate, critique, and refine hypotheses to act as a research partner, generating ideas, reviewing evidence, and proposing experiments, with a Nature paper and drug-discovery examples.
- **Sota Band**: new
- **Access Constraint**: Published in Nature; main page linked

### Marlin 2B
- **Category**: multimodal
- **Timestamp**: [25:57](https://www.youtube.com/watch?v=pC6KHflGye0&t=1557)
- **Why It Matters**: A tiny 2B video language model based on Qwen 3.5 2B that extracts structured information from video, producing scene descriptions and timestamped events for search, moderation, editing, or dataset labeling.
- **Sota Comparison**: Strongest open video model in its weight class; on captioning it matches the much larger closed Gemini 2.5 Flash.
- **Sota Band**: beats
- **Access Constraint**: Open; under 6GB, runs on low-end GPUs

### Qwen 3.7 Max
- **Vendor**: Alibaba
- **Category**: coding
- **Timestamp**: [26:55](https://www.youtube.com/watch?v=pC6KHflGye0&t=1615)
- **Why It Matters**: Alibaba's latest Qwen variant aimed at agentic multi-step work, especially coding tasks needing planning and iteration, pluggable into Claude Code, OpenClaw, or Hermes, with vision to drive robots in real time.
- **Sota Comparison**: On par with top open models including DeepSeek V4, GLM 5.1, and Kimi K2.6 on agentic coding and reasoning.
- **Sota Band**: parity
- **Access Constraint**: API only via Alibaba Cloud Model Studio; not open

### Qwen 3.5 Live Translate
- **Vendor**: Alibaba
- **Category**: multimodal
- **Timestamp**: [29:24](https://www.youtube.com/watch?v=pC6KHflGye0&t=1764)
- **Why It Matters**: A real-time translation model that also uses visual context, so it can see what is happening to disambiguate terms like shell versus human muscle and translate product specs in e-commerce live streams more accurately.
- **Sota Band**: new
- **Access Constraint**: Free demo via online platform

### Wall-climbing industrial robot
- **Vendor**: Robot+
- **Category**: other
- **Timestamp**: [30:28](https://www.youtube.com/watch?v=pC6KHflGye0&t=1828)
- **Why It Matters**: A heavy-duty humanoid dual-arm robot using wheeled magnetic suction to grip vertical steel surfaces, switching tools for welding, grinding, inspection, and spray painting on chemical tanks and ship hulls, removing humans from hazardous work.
- **Sota Comparison**: Unlike typical lightweight inspection drones, this is a field-tested powerhouse that has serviced over 10,000 ships.
- **Sota Band**: new
- **Access Constraint**: Teleoperated via VR headset

### HuggingFace humanoid robot
- **Vendor**: HuggingFace
- **Category**: other
- **Timestamp**: [32:12](https://www.youtube.com/watch?v=pC6KHflGye0&t=1932)
- **Why It Matters**: An open-source 3D-printed humanoid platform shipping the full stack of design, parts list, assembly guide, simulation tools, training environments, and runtime software to make humanoid and sim-to-real research more accessible.
- **Sota Band**: new
- **Access Constraint**: Open docs; ~$2500 in 3D-printed parts

### Unitree G1 voice control
- **Vendor**: Unitree Robotics
- **Category**: other
- **Timestamp**: [35:17](https://www.youtube.com/watch?v=pC6KHflGye0&t=2117)
- **Why It Matters**: A demo controlling the G1 with voice commands to autonomously jump, plank, turn, exercise, and dance in real time, in one continuous uncut shot with low latency, requiring no pre-programmed actions or teleoperation.
- **Sota Band**: new

### Cog Omni Control
- **Category**: video
- **Timestamp**: [37:03](https://www.youtube.com/watch?v=pC6KHflGye0&t=2223)
- **Why It Matters**: A ControlNet-style system for video generation that combines multiple inputs like rough sketch animation, pose skeletons, or line art plus a reference image and text prompt to produce a video that follows the specified direction.
- **Sota Band**: new
- **Access Constraint**: Technical paper only; no code or models yet

### Wave Flow
- **Vendor**: Meta
- **Category**: audio
- **Timestamp**: [38:27](https://www.youtube.com/watch?v=pC6KHflGye0&t=2307)
- **Why It Matters**: Takes a silent video and adds synced audio and sound effects, generating directly in raw waveform space without a VAE or latent compression, which should make sound cleaner, though it struggled with piano.
- **Sota Comparison**: Performs competitively against leading audio competitors like MM Audio.
- **Sota Band**: parity
- **Access Constraint**: GitHub repo; full checkpoints withheld by policy

### Pano World
- **Category**: world-model
- **Timestamp**: [41:06](https://www.youtube.com/watch?v=pC6KHflGye0&t=2466)
- **Why It Matters**: A generative world model that turns a floor plan plus style reference into a connected set of furnished panoramic room views that stay consistent as you move, using a 3D shell as visual memory for VR real-estate tours.
- **Sota Comparison**: Unlike Nano Banana or Cadream, layout, furniture, and materials stay consistent across viewpoints.
- **Sota Band**: new
- **Access Constraint**: No code or models yet; coming soon

### Stable Audio 3
- **Vendor**: Stability AI
- **Category**: music
- **Timestamp**: [43:23](https://www.youtube.com/watch?v=pC6KHflGye0&t=2603)
- **Why It Matters**: An open model family for making music, soundscapes, and effects from text prompts, with audio inpainting and extension; the medium 1.4B variant generates up to 6m20s and there is a small SFX version plus LoRA training docs.
- **Sota Band**: new
- **Access Constraint**: Small/medium open; large is API only, medium ~10GB

### Fashion Chameleon
- **Vendor**: Alibaba
- **Category**: video
- **Timestamp**: [44:45](https://www.youtube.com/watch?v=pC6KHflGye0&t=2685)
- **Why It Matters**: A real-time virtual try-on for video that streams a model wearing different garments at different moments while motion stays coherent, useful for fashion and live e-commerce outfit switching.
- **Sota Comparison**: Hits ~24 fps on a single GPU, claimed 30 to 180x faster than existing baselines.
- **Sota Band**: beats
- **Access Constraint**: Code and model planned; not released yet



## Wider context

This is a single-week open-source roundup, and the throughline is the death of the VAE/latent-space detour: L2P generates images in pixel space and Wave Flow audio in raw waveform, both trading compute for fidelity. The other axis is control, where Reactive GWM steers NPCs, Cog Omni Control conditions video on sketches and poses, and Qwen 3.5 Live Translate adds vision, shifting the frontier from raw generation quality to directable, instruction-following systems.

## Read next

[[unified-multimodal-models]] · [[latent-diffusion]] · [[world-models]] · [[ai-agents]] · [[speech-recognition]] · [[humanoid-robotics]]
