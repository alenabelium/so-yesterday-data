---
video_id: -D7o3E0eBf4
template_id: tech-overview
template_version: 1
source_summary: ../summaries/2026-02-08-opus-46-gpt-53-codex-stepfun-qwen3-coder-new-deepfake-ais-ne.md
source_transcript: ../transcripts/2026-02-08-opus-46-gpt-53-codex-stepfun-qwen3-coder-new-deepfake-ais-ne.md
source_summary_hash: sha256:16c268bfc09961163c6e1274e4f1193658303e83602a9b83e0a7f236f11ef54e
source_transcript_hash: sha256:789e11f757ef26ccacdf43e226221ef6e44e130ed1bc2150c3c4352a88c3d38b
fill_id: 132c45df-4d79-4bef-ad6e-b557a7502a74
published_at: '2026-10-19T20:50:02.476498'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Anthropic's Opus 4.6 tops independent leaderboards, but OpenAI's GPT 5.3 Codex, which helped create itself, dominates agentic coding benchmarks.

## Tools covered

### GLM OCR
- **Vendor**: ZAI
- **Category**: multimodal
- **Timestamp**: [01:01](https://www.youtube.com/watch?v=-D7o3E0eBf4&t=61)
- **Why It Matters**: A tiny 2.6GB OCR model that outperforms all open and closed source competitors on parsing text, tables, and handwriting from images, and is faster than alternatives.
- **Sota Comparison**: Outperforms open-source (PaddleOCR, DeepSeek OCR 2) and closed-source (Gemini 3 Pro, GPT 5.2) models across benchmarks.
- **Sota Band**: beats
- **External Link**: [https://huggingface.co](https://huggingface.co)
- **Access Constraint**: Open-source, 2.6GB

### Interact Avatar
- **Vendor**: Tencent
- **Category**: video
- **Timestamp**: [03:52](https://www.youtube.com/watch?v=-D7o3E0eBf4&t=232)
- **Why It Matters**: Generates talking avatars that can interact with objects (pick up, hold, gesture) based on text prompts, with precise timing control, unlike competitors that only animate speech.
- **Sota Comparison**: Only model that can manipulate objects; others like OmniAvatar only move and talk.
- **Sota Band**: new
- **External Link**: [https://github.com](https://github.com)
- **Access Constraint**: Open-source, uses 1.2 as base model

### Claude Opus 4.6
- **Vendor**: Anthropic
- **Category**: reasoning
- **Timestamp**: [05:55](https://www.youtube.com/watch?v=-D7o3E0eBf4&t=355)
- **Why It Matters**: Anthropic's smartest model, ranking #1 on LM Arena and Artificial Analysis, with a 68.8% score on ARC-AGI-2, far above competitors, but slower and pricier.
- **Sota Comparison**: Outperforms GPT 5.2 and Gemini 3 Pro on independent leaderboards, but scores lower on SWE-Bench Verified than Opus 4.5.
- **Sota Band**: beats
- **External Link**: [https://www.anthropic.com](https://www.anthropic.com)
- **Access Constraint**: Paid plans and API

### GPT 5.3 Codex
- **Vendor**: OpenAI
- **Category**: coding
- **Timestamp**: [09:43](https://www.youtube.com/watch?v=-D7o3E0eBf4&t=583)
- **Why It Matters**: OpenAI's most capable agentic coding model, the first to be instrumental in creating itself via recursive self-improvement, dominating SWE-Bench Pro and Terminal Bench 2.
- **Sota Comparison**: Outperforms Opus 4.6 on Terminal Bench 2 and Opus 4.5 on SWE-Bench Pro (56.8% vs 45.89%).
- **Sota Band**: beats
- **External Link**: [https://openai.com](https://openai.com)
- **Access Constraint**: Paid ChatGPT plans, API soon

### Step 3.5 Flash
- **Vendor**: StepFun
- **Category**: reasoning
- **Timestamp**: [13:27](https://www.youtube.com/watch?v=-D7o3E0eBf4&t=807)
- **Why It Matters**: A 196B MoE model (11B active) matching top closed models in intelligence and deep research, with 100-300 tokens/sec throughput, at a fraction of the cost.
- **Sota Comparison**: On par with Gemini 3 Pro, Opus 4.5, and GPT 5.2 in reasoning; outperforms Gemini and OpenAI Deep Research in deep research.
- **Sota Band**: parity
- **External Link**: [https://huggingface.co](https://huggingface.co)
- **Access Constraint**: Open-weight, 399GB, needs multiple GPUs

### MiniCPM-o4.5
- **Vendor**: ModelBest
- **Category**: multimodal
- **Timestamp**: [16:50](https://www.youtube.com/watch?v=-D7o3E0eBf4&t=1010)
- **Why It Matters**: A 9B omnimodal model supporting text, voice, image, and video interaction in real-time, including voice cloning and visual puzzles, outperforming other omni models.
- **Sota Comparison**: Outperforms other omni models on visual understanding, live streaming, and speech conversation benchmarks.
- **Sota Band**: beats
- **External Link**: [https://huggingface.co](https://huggingface.co)
- **Access Constraint**: Open-source, 23.4GB, fits in 4090

### Intern S1 Pro
- **Vendor**: Shanghai AI Lab
- **Category**: reasoning
- **Timestamp**: [23:59](https://www.youtube.com/watch?v=-D7o3E0eBf4&t=1439)
- **Why It Matters**: A trillion-parameter MoE model (22B active) with state-of-the-art scientific reasoning, outperforming Gemini 3 Pro and Kimi K2.5 on science benchmarks.
- **Sota Comparison**: Outperforms Kimi K2.5 and Gemini 3 Pro on average across science tasks.
- **Sota Band**: beats
- **External Link**: [https://github.com](https://github.com)
- **Access Constraint**: Open-source, 919GB, needs data farm

### Qwen 3 Coder Next
- **Vendor**: Alibaba
- **Category**: coding
- **Timestamp**: [24:56](https://www.youtube.com/watch?v=-D7o3E0eBf4&t=1496)
- **Why It Matters**: An 80B MoE coding agent (3B active) matching much larger models on SWE-Bench, with autonomous troubleshooting and integration with OpenClaw.
- **Sota Comparison**: On par with Claude 4.5 and other top open-source models despite being far smaller.
- **Sota Band**: parity
- **External Link**: [https://github.com](https://github.com)
- **Access Constraint**: Open-source, 150GB+ (FP8 80GB)

### Skin Tokens
- **Vendor**: Unknown
- **Category**: video
- **Timestamp**: [21:20](https://www.youtube.com/watch?v=-D7o3E0eBf4&t=1280)
- **Why It Matters**: Estimates rigs/skeletons for 3D models, enabling animation of humans, animals, and fictional characters, outperforming other rig prediction systems.
- **Sota Comparison**: Most accurate on average compared to other rig prediction systems.
- **Sota Band**: beats
- **External Link**: [https://github.com](https://github.com)
- **Access Constraint**: Technical paper only, code not yet released

### Context Forcing
- **Vendor**: Unknown
- **Category**: video
- **Timestamp**: [30:40](https://www.youtube.com/watch?v=-D7o3E0eBf4&t=1840)
- **Why It Matters**: A framework that generates videos 2-10x longer than other methods with minimal inconsistencies, maintaining character and background coherence over a minute.
- **Sota Comparison**: Retains memory longer than LongLive, avoiding inconsistencies in background and character.
- **Sota Band**: beats
- **External Link**: [https://github.com](https://github.com)
- **Access Constraint**: Code and checkpoints to be open-sourced

### Paper Banana
- **Vendor**: Google
- **Category**: image
- **Timestamp**: [31:59](https://www.youtube.com/watch?v=-D7o3E0eBf4&t=1919)
- **Why It Matters**: Automates generation of accurate illustrations and diagrams for academic papers using a multi-agent framework, outperforming humans in readability and aesthetics.
- **Sota Comparison**: Outperforms Paper2Any and even humans in conciseness, readability, and aesthetics.
- **Sota Band**: beats
- **External Link**: [https://github.com](https://github.com)
- **Access Constraint**: Code and dataset to be released in 2 weeks

### FS Video
- **Vendor**: ByteDance
- **Category**: video
- **Timestamp**: [34:19](https://www.youtube.com/watch?v=-D7o3E0eBf4&t=2059)
- **Why It Matters**: A blazing-fast video generator producing 720p videos in 18 seconds on two H100s, with quality on par with top models, but only a technical paper so far.
- **Sota Comparison**: Visual quality on par with top video models.
- **Sota Band**: parity
- **External Link**: [https://github.com](https://github.com)
- **Access Constraint**: Technical paper only

### Omnimat Zero
- **Vendor**: Unknown
- **Category**: video
- **Timestamp**: [36:19](https://www.youtube.com/watch?v=-D7o3E0eBf4&t=2179)
- **Why It Matters**: Removes objects from videos, including reflections and shadows, and can separate foreground into a transparent layer for background replacement.
- **Sota Comparison**: Performs better than other object removal tools, uniquely handling complex scenes like removing a background figure while keeping a foreground pole.
- **Sota Band**: beats
- **External Link**: [https://github.com](https://github.com)
- **Access Constraint**: Open-source

### 3D Move
- **Vendor**: Kling
- **Category**: video
- **Timestamp**: [37:43](https://www.youtube.com/watch?v=-D7o3E0eBf4&t=2263)
- **Why It Matters**: Transfers motion from a reference video to a new character while also allowing camera control, a unique combination not offered by other animator tools.
- **Sota Comparison**: Only model that combines motion transfer with camera control; others like OneAnimate or Scale do one or the other.
- **Sota Band**: new
- **External Link**: [https://github.com](https://github.com)
- **Access Constraint**: Technical paper only

### Inter Prior
- **Vendor**: Unknown
- **Category**: agent
- **Timestamp**: [39:48](https://www.youtube.com/watch?v=-D7o3E0eBf4&t=2388)
- **Why It Matters**: Trains robots in physically correct virtual environments to interact with objects naturally, enabling emergent behaviors like isolating an object before picking it up.
- **Sota Comparison**: Enables emergent behaviors not in training data, improving robustness in unstable real-world conditions.
- **Sota Band**: new
- **External Link**: [https://github.com](https://github.com)
- **Access Constraint**: Technical paper only

### Fast VMT
- **Vendor**: Unknown
- **Category**: video
- **Timestamp**: [41:46](https://www.youtube.com/watch?v=-D7o3E0eBf4&t=2506)
- **Why It Matters**: Transfers motion from one video to another, changing objects or backgrounds while preserving movement and camera motion, generating videos 3.43x faster.
- **Sota Comparison**: Generates videos 3.43x faster than existing methods.
- **Sota Band**: beats
- **External Link**: [https://github.com](https://github.com)
- **Access Constraint**: No code released yet

### Edit Yourself
- **Vendor**: Unknown
- **Category**: video
- **Timestamp**: [43:31](https://www.youtube.com/watch?v=-D7o3E0eBf4&t=2611)
- **Why It Matters**: Edits talking-head videos to change dialogue, remove stutters, or add sentences with seamless lip-sync, raising deepfake concerns.
- **Sota Comparison**: Seamlessly stitches edits without hard cuts, unlike manual editing.
- **Sota Band**: new
- **External Link**: [https://foul.ai](https://foul.ai)
- **Access Constraint**: Available on foul.ai and Pipio; GitHub not yet released



## Wider context

This week marks a turning point where open-source models (Step 3.5 Flash, Qwen 3 Coder) achieve parity with closed giants, while GPT 5.3 Codex's recursive self-improvement hints at a new paradigm in AI development. The rapid release of deepfake tools like Edit Yourself underscores the urgent need for robust detection and ethical guidelines.

## Read next
