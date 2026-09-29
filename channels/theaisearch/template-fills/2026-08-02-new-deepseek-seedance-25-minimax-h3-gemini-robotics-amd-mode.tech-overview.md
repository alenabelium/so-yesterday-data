---
video_id: OrcBSpADCGk
template_id: tech-overview
template_version: 1
source_summary: ../summaries/2026-08-02-new-deepseek-seedance-25-minimax-h3-gemini-robotics-amd-mode.md
source_transcript: ../transcripts/2026-08-02-new-deepseek-seedance-25-minimax-h3-gemini-robotics-amd-mode.md
source_summary_hash: sha256:a9247965c1c2d34ddd3acdcee856aa20a635bd20f289e4dbc06c97062fda75d9
source_transcript_hash: sha256:2480b6221e1578db4693275568e242d7a861b12ee8472a8584e78af48b67f7a0
fill_id: 112dbdbf-dfbf-40a0-8389-3dd83115a284
published_at: '2026-09-29T11:21:41.431472'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Seedance 2.5 and Minimax H3 lead video generation, while Deepseek V4 Flash delivers frontier performance at 100x lower cost.

## Tools covered

### IDV
- **Vendor**: Netflix
- **Category**: video
- **Timestamp**: [00:00](https://www.youtube.com/watch?v=OrcBSpADCGk&t=0)
- **Why It Matters**: Open-source tool that changes video scene style while preserving character identity and movement via keyframe editing.
- **Sota Comparison**: Open-source style transfer for video that maintains character consistency.
- **Sota Band**: new
- **Access Constraint**: Open-source

### Crisper Whisper 2
- **Vendor**: Crisper
- **Category**: asr
- **Timestamp**: [01:18](https://www.youtube.com/watch?v=OrcBSpADCGk&t=78)
- **Why It Matters**: Open-source transcription tool offering verbatim and intended modes with precise word-level timing.
- **Sota Comparison**: Outperforms 11 Labs and others in transcription accuracy and word-level timestamp precision.
- **Sota Band**: beats
- **Access Constraint**: Open-source

### Deepseek V4 Flash
- **Vendor**: Deepseek
- **Category**: reasoning
- **Timestamp**: [04:14](https://www.youtube.com/watch?v=OrcBSpADCGk&t=254)
- **Why It Matters**: Frontier-level coding and reasoning model that is 100x cheaper than Claude Opus and 70% smaller than GLM 5.2.
- **Sota Comparison**: Matches GLM 5.2 and Opus 4.8 on benchmarks while being significantly cheaper and smaller.
- **Sota Band**: parity
- **Access Constraint**: Open-source

### Redesign
- **Vendor**: Redesign
- **Category**: image
- **Timestamp**: [06:04](https://www.youtube.com/watch?v=OrcBSpADCGk&t=364)
- **Why It Matters**: Converts flat images into editable layers using OCR, segmentation, and image layering AI tools.
- **Sota Comparison**: Outperforms other image-to-layer generators like Image Layered in benchmarks.
- **Sota Band**: beats
- **Access Constraint**: Open-source

### Kimi K3
- **Vendor**: Moonshot AI
- **Category**: reasoning
- **Timestamp**: [08:11](https://www.youtube.com/watch?v=OrcBSpADCGk&t=491)
- **Why It Matters**: Massive 2.8T parameter MoE model with native vision, now open-source with full weights released.
- **Sota Comparison**: Most powerful open-source model available, though requires significant hardware resources.
- **Sota Band**: new
- **Access Constraint**: Open-source

### Instellae
- **Vendor**: AMD
- **Category**: reasoning
- **Timestamp**: [09:03](https://www.youtube.com/watch?v=OrcBSpADCGk&t=543)
- **Why It Matters**: First fully open-source model trained entirely on AMD Instinct hardware and ROCm software stack.
- **Sota Comparison**: Beats similarly sized models like Gemma 4 and a smaller version of Cohere 3.5.
- **Sota Band**: beats
- **Access Constraint**: Open-source

### Inkling Small
- **Vendor**: Thinking Machines AI
- **Category**: multimodal
- **Timestamp**: [12:22](https://www.youtube.com/watch?v=OrcBSpADCGk&t=742)
- **Why It Matters**: Smaller omnimodal model with strong audio capabilities, offering cost efficiency over the full Inkling model.
- **Sota Comparison**: Holds up well against DeepSeek V4 Flash and Gemini 3.5 Flash Light, especially in audio tasks.
- **Sota Band**: parity
- **Access Constraint**: Open-source

### Prism
- **Vendor**: Thinking Machines AI
- **Category**: agent
- **Timestamp**: [16:05](https://www.youtube.com/watch?v=OrcBSpADCGk&t=965)
- **Why It Matters**: Robotics system that improves physical contact reaction and movement control using multi-sensor inputs.
- **Sota Comparison**: Shows higher success rates and lower error rates than similar robotics algorithms.
- **Sota Band**: beats
- **Access Constraint**: Open-source

### Seedance 2.5
- **Vendor**: ByteDance
- **Category**: video
- **Timestamp**: [16:05](https://www.youtube.com/watch?v=OrcBSpADCGk&t=965)
- **Why It Matters**: Top-tier video model capable of 30-second clips with high action and character consistency.
- **Sota Comparison**: Best video model for high-action scenes, surpassing previous versions and competitors.
- **Sota Band**: beats
- **Access Constraint**: Paid API

### Minimax H3
- **Vendor**: Minimax
- **Category**: video
- **Timestamp**: [18:30](https://www.youtube.com/watch?v=OrcBSpADCGk&t=1110)
- **Why It Matters**: Powerful multimodal video generator supporting 2K resolution and complex multi-input references.
- **Sota Comparison**: Significantly cheaper than Seedance 2.5 while offering high-quality video generation.
- **Sota Band**: parity
- **Access Constraint**: Paid API

### Gemini Robotics 2
- **Vendor**: Google DeepMind
- **Category**: agent
- **Timestamp**: [22:10](https://www.youtube.com/watch?v=OrcBSpADCGk&t=1330)
- **Why It Matters**: Robotics model family enabling full-body control, reasoning, and offline operation for humanoid robots.
- **Sota Comparison**: Advances over previous Gemini Robotics models with better hand control and reasoning.
- **Sota Band**: beats
- **Access Constraint**: Trusted Tester

### Wonder
- **Vendor**: Adobe
- **Category**: world-model
- **Timestamp**: [24:00](https://www.youtube.com/watch?v=OrcBSpADCGk&t=1440)
- **Why It Matters**: Interactive video world model allowing real-time exploration and navigation within generated scenes.
- **Sota Comparison**: Novel approach to interactive world modeling, though currently noisy and inconsistent.
- **Sota Band**: new
- **Access Constraint**: Coming Soon

### Fi0
- **Vendor**: Fi0
- **Category**: world-model
- **Timestamp**: [26:33](https://www.youtube.com/watch?v=OrcBSpADCGk&t=1593)
- **Why It Matters**: Video world model using 'physical language' to reason about movement before rendering frames.
- **Sota Comparison**: Outperforms other world models in physical coherence and understanding benchmarks.
- **Sota Band**: beats
- **Access Constraint**: Coming Soon

### Seedance 2.5
- **Timestamp**: [16:05](https://www.youtube.com/watch?v=OrcBSpADCGk&t=965)
- **One Liner**: Host calls it the best video model out there for high-action scenes and character consistency.
- **Sota Band**: beats

### Deepseek V4 Flash
- **Timestamp**: [04:14](https://www.youtube.com/watch?v=OrcBSpADCGk&t=254)
- **One Liner**: Host highlights its incredible efficiency and cost-effectiveness compared to frontier models.
- **Sota Band**: beats

## Wider context

The week marks a shift in AI accessibility and efficiency. Deepseek V4 Flash and AMD's Instellae demonstrate that frontier performance and hardware independence are no longer exclusive to Nvidia/CUDA ecosystems. In video generation, Seedance 2.5 and Minimax H3 push the boundaries of length and multimodal control, while open-source models like Kimi K3 and Inkling Small close the gap on proprietary leaders, forcing a re-evaluation of cost-performance trade-offs across the industry.

## Read next

[[open-source-ai]] · [[video-generation]] · [[large-language-models]] · [[robotics]] · [[hardware-independence]] · [[cost-efficiency]]
