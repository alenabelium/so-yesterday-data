---
video_id: 6Il0CJx9yU8
template_id: tech-overview
template_version: 1
source_summary: ../summaries/2026-03-29-robot-waifus-rip-sora-glm-51-ai-brain-scans-google-realtime.md
source_transcript: ../transcripts/2026-03-29-robot-waifus-rip-sora-glm-51-ai-brain-scans-google-realtime.md
source_summary_hash: sha256:a84eb48960552341d7be167b2255ea0f3b856e7e03e5aa1e59243844f4dd1eaf
source_transcript_hash: sha256:571086491f4ee15e8376808246cb98019864e5b73c625da822c86e32215a6ddb
fill_id: 50178f73-7258-49a9-9077-cf96e4a7536a
published_at: '2026-10-19T20:27:21.687716'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

OpenAI shuts down Sora while open-source tools like Real-ESRGAN and DaVinci Magi Human surge ahead.

## Tools covered

### Real-ESRGAN
- **Vendor**: Unknown
- **Category**: image
- **Timestamp**: [01:02](https://www.youtube.com/watch?v=6Il0CJx9yU8&t=62)
- **Why It Matters**: Restores damaged photos, removing noise, scratches, and reflections, matching closed models on benchmarks.
- **Sota Comparison**: On par with NanoBanana Pro and GPT-4 Image 1.5, beats Qwen Image Edit and LongCat Image Edit.
- **Sota Band**: parity
- **Access Constraint**: Open-source, 42 GB

### Matrix Game 3.0
- **Vendor**: Skywork AI
- **Category**: world-model
- **Timestamp**: [03:22](https://www.youtube.com/watch?v=6Il0CJx9yU8&t=202)
- **Why It Matters**: Generates interactive 720p worlds in real-time with memory for long-term consistency.
- **Sota Comparison**: New approach with memory, real-time generation at 40 FPS.
- **Sota Band**: new
- **Access Constraint**: Open-source, 5B params

### DaVinci Magi Human
- **Vendor**: Unknown
- **Category**: video
- **Timestamp**: [04:55](https://www.youtube.com/watch?v=6Il0CJx9yU8&t=295)
- **Why It Matters**: Open-source video generator with native audio, supporting multiple languages.
- **Sota Comparison**: Higher win rate than LTEX 2.3 in blind tests.
- **Sota Band**: beats
- **Access Constraint**: Open-source, 61 GB distilled

### Prism Audio
- **Vendor**: Unknown
- **Category**: audio
- **Timestamp**: [07:39](https://www.youtube.com/watch?v=6Il0CJx9yU8&t=459)
- **Why It Matters**: Generates perfectly timed sound effects for silent videos, outperforming larger models.
- **Sota Comparison**: Highest benchmark scores, fastest, smallest at 518M params.
- **Sota Band**: beats
- **Access Constraint**: Open-source, 6 GB

### Retime GS
- **Vendor**: Unknown
- **Category**: video
- **Timestamp**: [09:49](https://www.youtube.com/watch?v=6Il0CJx9yU8&t=589)
- **Why It Matters**: Creates smooth 4D animations from choppy videos, filling missing frames.
- **Sota Comparison**: Only tool producing coherent animations vs competitors.
- **Sota Band**: beats
- **Access Constraint**: Paper only, data coming soon

### Tribe V2
- **Vendor**: Meta
- **Category**: other
- **Timestamp**: [11:54](https://www.youtube.com/watch?v=6Il0CJx9yU8&t=714)
- **Why It Matters**: Predicts brain activity from video, generalizing to new people and content.
- **Sota Comparison**: More accurate than actual fMRI scans.
- **Sota Band**: beats
- **Access Constraint**: Open-source

### ComfyUI Dynamic VRAM
- **Vendor**: ComfyUI
- **Category**: tool
- **Timestamp**: [14:29](https://www.youtube.com/watch?v=6Il0CJx9yU8&t=869)
- **Why It Matters**: Manages VRAM efficiently, enabling larger models and faster generation on low-VRAM GPUs.
- **Sota Comparison**: Significantly faster execution times.
- **Sota Band**: new
- **Access Constraint**: Nvidia GPUs, Windows/Linux

### Action Plan
- **Vendor**: Unknown
- **Category**: agent
- **Timestamp**: [15:32](https://www.youtube.com/watch?v=6Il0CJx9yU8&t=932)
- **Why It Matters**: Generates real-time human motion from text, applicable to humanoid robots.
- **Sota Comparison**: Runs up to 9x faster with smooth motion.
- **Sota Band**: new
- **Access Constraint**: Open-source

### World Agents
- **Vendor**: Unknown
- **Category**: world-model
- **Timestamp**: [17:38](https://www.youtube.com/watch?v=6Il0CJx9yU8&t=1058)
- **Why It Matters**: Uses 2D image models to build consistent 3D worlds via agentic loop.
- **Sota Comparison**: New approach, no additional training.
- **Sota Band**: new
- **Access Constraint**: Paper only

### World Reconstruction from Inconsistent Views
- **Vendor**: Unknown
- **Category**: world-model
- **Timestamp**: [18:53](https://www.youtube.com/watch?v=6Il0CJx9yU8&t=1133)
- **Why It Matters**: Stitches AI-generated videos into consistent 3D worlds, model-agnostic.
- **Sota Comparison**: More consistent than other generators.
- **Sota Band**: beats
- **Access Constraint**: Open-source

### Lumos X
- **Vendor**: Unknown
- **Category**: video
- **Timestamp**: [20:42](https://www.youtube.com/watch?v=6Il0CJx9yU8&t=1242)
- **Why It Matters**: Creates consistent deepfakes with multiple reference images.
- **Sota Comparison**: More consistent than competitors.
- **Sota Band**: beats
- **Access Constraint**: Open-source, 35 GB

### Turbo Quant
- **Vendor**: Google Research
- **Category**: tool
- **Timestamp**: [24:28](https://www.youtube.com/watch?v=6Il0CJx9yU8&t=1468)
- **Why It Matters**: Compresses AI models to use 6x less memory and 8x faster retrieval.
- **Sota Comparison**: New compression method.
- **Sota Band**: new
- **Access Constraint**: Technical paper

### GLM 5.1
- **Vendor**: ZAI
- **Category**: coding
- **Timestamp**: [25:51](https://www.youtube.com/watch?v=6Il0CJx9yU8&t=1551)
- **Why It Matters**: Agentic coding model approaching Opus 4.6, faster and cheaper.
- **Sota Comparison**: Close to Opus 4.6 on agentic coding.
- **Sota Band**: parity
- **Access Constraint**: API, open-source planned

### Arc-AGI 3
- **Vendor**: Unknown
- **Category**: reasoning
- **Timestamp**: [26:56](https://www.youtube.com/watch?v=6Il0CJx9yU8&t=1616)
- **Why It Matters**: Benchmark showing frontier models score <0.5% on learning new environments.
- **Sota Comparison**: Humans solve 100%, models under 0.5%.
- **Sota Band**: inferred
- **Access Constraint**: Benchmark

### Real Master
- **Vendor**: Meta
- **Category**: video
- **Timestamp**: [29:56](https://www.youtube.com/watch?v=6Il0CJx9yU8&t=1796)
- **Why It Matters**: Turns game renders into photorealistic video, preserving geometry.
- **Sota Comparison**: Keeps consistency better than other editors.
- **Sota Band**: beats
- **Access Constraint**: Not released

### Sora
- **Vendor**: OpenAI
- **Category**: video
- **Timestamp**: [31:28](https://www.youtube.com/watch?v=6Il0CJx9yU8&t=1888)
- **Why It Matters**: OpenAI shuts down Sora app to focus on robotics and real-world tasks.
- **Sota Comparison**: Sora 2 model still available in ChatGPT.
- **Sota Band**: inferred
- **Access Constraint**: Shutting down

### Co-here Transcribe
- **Vendor**: Cohere
- **Category**: asr
- **Timestamp**: [33:28](https://www.youtube.com/watch?v=6Il0CJx9yU8&t=2008)
- **Why It Matters**: State-of-the-art open-source transcription, efficient and accurate.
- **Sota Comparison**: Wins most benchmarks vs ElevenLabs, Whisper, etc.
- **Sota Band**: beats
- **Access Constraint**: Open-source, Apache 2.0

### Origin F1
- **Vendor**: A Head Form
- **Category**: other
- **Timestamp**: [35:27](https://www.youtube.com/watch?v=6Il0CJx9yU8&t=2127)
- **Why It Matters**: Hyperrealistic humanoid robot head with swappable skin and microexpressions.
- **Sota Comparison**: Most realistic humanoid robot seen.
- **Sota Band**: new
- **Access Constraint**: Not yet available

### Logger NVS
- **Vendor**: Unknown
- **Category**: image
- **Timestamp**: [36:27](https://www.youtube.com/watch?v=6Il0CJx9yU8&t=2187)
- **Why It Matters**: Generates new views from few images, creating full 3D scenes.
- **Sota Comparison**: New approach without dense input.
- **Sota Band**: new
- **Access Constraint**: Open-source

### Pulse of Motion
- **Vendor**: Unknown
- **Category**: video
- **Timestamp**: [37:36](https://www.youtube.com/watch?v=6Il0CJx9yU8&t=2256)
- **Why It Matters**: Fixes timing in AI videos, making motion realistic.
- **Sota Comparison**: Addresses chronometric hallucination.
- **Sota Band**: new
- **Access Constraint**: Open-source, <2 GB

### Mega Flow
- **Vendor**: Unknown
- **Category**: video
- **Timestamp**: [40:42](https://www.youtube.com/watch?v=6Il0CJx9yU8&t=2442)
- **Why It Matters**: State-of-the-art optical flow for large displacements.
- **Sota Comparison**: Achieves SOTA pixel tracking accuracy.
- **Sota Band**: beats
- **Access Constraint**: Open-source, <4 GB

### CUA Suite
- **Vendor**: Unknown
- **Category**: agent
- **Timestamp**: [41:29](https://www.youtube.com/watch?v=6Il0CJx9yU8&t=2489)
- **Why It Matters**: Massive dataset for training computer-use agents.
- **Sota Comparison**: 2.5x larger than current largest.
- **Sota Band**: new
- **Access Constraint**: Open-source

### Gemini 3.1 Flash Live
- **Vendor**: Google
- **Category**: multimodal
- **Timestamp**: [43:29](https://www.youtube.com/watch?v=6Il0CJx9yU8&t=2609)
- **Why It Matters**: Real-time voice that feels natural, integrates with apps.
- **Sota Comparison**: New real-time voice model.
- **Sota Band**: new
- **Access Constraint**: API, AI Studio



## Wider context

OpenAI's pivot from consumer video to robotics signals a broader industry shift toward real-world AI. Meanwhile, open-source tools are closing the gap on closed models, with Real-ESRGAN matching top editors and DaVinci beating LTEX. The Arc-AGI 3 benchmark reveals a critical weakness: even frontier models struggle with learning in unfamiliar environments, highlighting the next frontier for AI research.

## Read next

[[open-source-ai]] · [[world-models]] · [[real-time-ai]] · [[ai-agents]] · [[video-generation]]
