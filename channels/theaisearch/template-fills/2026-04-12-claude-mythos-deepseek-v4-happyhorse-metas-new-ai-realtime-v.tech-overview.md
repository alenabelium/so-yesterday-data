---
video_id: 1_5sSJK2rU0
template_id: tech-overview
template_version: 1
source_summary: ../summaries/2026-04-12-claude-mythos-deepseek-v4-happyhorse-metas-new-ai-realtime-v.md
source_transcript: ../transcripts/2026-04-12-claude-mythos-deepseek-v4-happyhorse-metas-new-ai-realtime-v.md
source_summary_hash: sha256:93fe566c7b37aa1589123d29f56e6d28021daa2ebf8133c7cae4a71892023623
source_transcript_hash: sha256:f46b6a11fad059597e03c118aefba70518cf644e5fa23af3283138fcb83f51b2
fill_id: 86191c54-98a6-4889-8761-f40cb3c9e19e
published_at: '2026-10-19T20:27:14.180284'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Anthropic withholds Claude Mythos Preview over cyber-risk while ZAI open-sources GLM 5.1, the new best open model.

## Tools covered

### Claude Mythos Preview
- **Vendor**: Anthropic
- **Category**: reasoning
- **Timestamp**: [00:00](https://www.youtube.com/watch?v=1_5sSJK2rU0&t=0)
- **Why It Matters**: A frontier model so capable at finding software vulnerabilities that Anthropic refuses to release it publicly, citing national-security risks. It autonomously discovered thousands of high-severity exploits across major OSes and browsers, including a 27-year-old OpenBSD bug.
- **Sota Comparison**: Shows a 14% improvement over Opus 4.6 on SWE-Bench Pro, but critics note smaller open-weight models can replicate some findings when given isolated code.
- **Sota Band**: beats
- **Access Constraint**: Not released; Project Glasswing for defenders

### GLM 5.1
- **Vendor**: ZAI
- **Category**: reasoning
- **Timestamp**: [11:17](https://www.youtube.com/watch?v=1_5sSJK2rU0&t=677)
- **Why It Matters**: Open-sourced weights make this the best open-source model for agentic coding, beating closed models like GPT 5.4 and Opus 4.6 on SWE-Bench Pro. Demonstrates autonomous 8-hour coding sessions that build a full Linux desktop with 50+ working apps.
- **Sota Comparison**: State-of-the-art among open models and competitive with leading closed models on agentic benchmarks.
- **Sota Band**: beats
- **Access Constraint**: Open-source; 1.5 TB weights

### InSpatial World
- **Vendor**: Unknown
- **Category**: world-model
- **Timestamp**: [13:29](https://www.youtube.com/watch?v=1_5sSJK2rU0&t=809)
- **Why It Matters**: Turns a regular video into a persistent 3D world you can explore in real time, with consistent physics and motion. Runs at 24 FPS on an H-series GPU and 10 FPS on a single RTX 4090, enabling new camera angles and interactive replay.
- **Sota Comparison**: Achieves one of the highest scores on the WorldScore dynamic benchmark with far fewer parameters than competitors.
- **Sota Band**: beats
- **Access Constraint**: Code released

### DeepSeek Expert Mode
- **Vendor**: DeepSeek
- **Category**: reasoning
- **Timestamp**: [16:18](https://www.youtube.com/watch?v=1_5sSJK2rU0&t=978)
- **Why It Matters**: A new mode on the DeepSeek platform that shows noticeably stronger reasoning on logic, math, and coding. Users speculate it's a preview of V4 Light, hinting at an April release for the full V4.
- **Sota Comparison**: Perceived as a step up from V3, but not a full V4.
- **Sota Band**: inferred
- **Access Constraint**: Free to use

### Happy Horse 1.0
- **Vendor**: Alibaba
- **Category**: video
- **Timestamp**: [16:18](https://www.youtube.com/watch?v=1_5sSJK2rU0&t=978)
- **Why It Matters**: A new video generator from Alibaba's ATTH AI Innovation Unit that tops the Artificial Analysis leaderboard, outperforming most competitors. Signals China's continued dominance in AI video generation.
- **Sota Comparison**: Outperforms most models on the leaderboard; unclear if it beats Seedance 2.0.
- **Sota Band**: beats
- **Access Constraint**: Not yet released; expected April 30

### Waypoint 1.5
- **Vendor**: Overworld
- **Category**: world-model
- **Timestamp**: [18:13](https://www.youtube.com/watch?v=1_5sSJK2rU0&t=1093)
- **Why It Matters**: A real-time interactive world model that runs on consumer GPUs (RTX 3070 minimum), generating worlds at up to 720p/60 FPS. Open-source, making real-time world generation accessible to hobbyists.
- **Sota Comparison**: Trade-off in quality for real-time performance, but unique in running on consumer hardware.
- **Sota Band**: new
- **Access Constraint**: Open-source; requires RTX 3070+

### Muse Spark
- **Vendor**: Meta
- **Category**: reasoning
- **Timestamp**: [19:25](https://www.youtube.com/watch?v=1_5sSJK2rU0&t=1165)
- **Why It Matters**: Meta's first model from its rebuilt AI lab, powering Meta AI across its apps and smart glasses. Multimodal and strong on chart reasoning, but not state-of-the-art overall.
- **Sota Comparison**: Ranks fourth on Artificial Analysis, tied with Sonnet 4.6 and just above GLM 5.1; trails Gemini 3.1 Pro and GPT 5.4.
- **Sota Band**: behind
- **Access Constraint**: Closed source

### AEP 1.5 XL
- **Vendor**: Unknown
- **Category**: music
- **Timestamp**: [23:19](https://www.youtube.com/watch?v=1_5sSJK2rU0&t=1399)
- **Why It Matters**: An open-source music generator that produces full songs from a prompt and lyrics, running on consumer devices in under a minute. Benchmarks claim it beats closed models like Udio and Suno.
- **Sota Comparison**: Roughly matches Udio v4, close to v5, per host's tests.
- **Sota Band**: parity
- **Access Constraint**: Open-source

### Numina
- **Vendor**: Unknown
- **Category**: video
- **Timestamp**: [24:56](https://www.youtube.com/watch?v=1_5sSJK2rU0&t=1496)
- **Why It Matters**: A model-agnostic tool that fixes object-count errors in video generation, a common failure even in top models like Veo 3.1. Works with open-source models like Wan 2.1 and 2.2.
- **Sota Comparison**: Improves object-count accuracy over base models; outperforms Veo 3.1 and Grok Imagine on this specific task.
- **Sota Band**: beats
- **Access Constraint**: Code released

### RollerQuant
- **Vendor**: Unknown
- **Category**: tool
- **Timestamp**: [26:17](https://www.youtube.com/watch?v=1_5sSJK2rU0&t=1577)
- **Why It Matters**: An open-source KV-cache compression algorithm that beats Google's TurboQuant on speed, quality, and parameter count. Uses Clifford rotators to cut operations per vector from 16,000 to ~200, enabling 10x memory compression and 5.3x faster prefill.
- **Sota Comparison**: Beats Google's TurboQuant on every axis.
- **Sota Band**: beats
- **Access Constraint**: Open-source

### MMFiz Video
- **Vendor**: Unknown
- **Category**: video
- **Timestamp**: [27:17](https://www.youtube.com/watch?v=1_5sSJK2rU0&t=1637)
- **Why It Matters**: A framework that trains video models with physical understanding (motion, geometry, interaction) rather than just pixels, producing more physically consistent videos. Addresses the warping and weird physics common in pixel-based generators.
- **Sota Comparison**: Shows improved physical consistency over models like Wan 2.1.
- **Sota Band**: beats
- **Access Constraint**: Code and dataset coming soon

### Vanast
- **Vendor**: Unknown
- **Category**: video
- **Timestamp**: [28:41](https://www.youtube.com/watch?v=1_5sSJK2rU0&t=1721)
- **Why It Matters**: A virtual try-on tool that animates a person wearing new clothing, retaining facial features and body shape. Supports upper/lower body and dress transfer with pose control.
- **Sota Comparison**: No direct comparison provided.
- **Sota Band**: inferred
- **Access Constraint**: Code coming soon

### Anima v3 Preview
- **Vendor**: Unknown
- **Category**: image
- **Timestamp**: [30:34](https://www.youtube.com/watch?v=1_5sSJK2rU0&t=1834)
- **Why It Matters**: A lightweight 2B-parameter model that generates high-quality anime images, trained on millions of anime and non-anime art images. Understands Danbooru and quality tags, works smoothly in ComfyUI.
- **Sota Comparison**: State-of-the-art for anime image generation in its size class.
- **Sota Band**: beats
- **Access Constraint**: Open-source; available on CivitAI and ModelScope

### Komodo
- **Vendor**: Nvidia
- **Category**: tool
- **Timestamp**: [32:25](https://www.youtube.com/watch?v=1_5sSJK2rU0&t=1945)
- **Why It Matters**: Generates 3D human and robot motions from text prompts, with proper physics and balance. Can be used to synthetically train robots in simulation before real-world deployment, reducing the need for manual demonstrations.
- **Sota Comparison**: No direct comparison provided.
- **Sota Band**: new
- **Access Constraint**: Open-source; v1.1 released

### Spatial Edit
- **Vendor**: Unknown
- **Category**: image
- **Timestamp**: [34:02](https://www.youtube.com/watch?v=1_5sSJK2rU0&t=2042)
- **Why It Matters**: Allows precise movement of objects and camera angle changes in photos, with controls for yaw, pitch, and zoom. Outperforms other models like Nano Banana and CRaEdit on object and camera placement benchmarks.
- **Sota Comparison**: Only model that handled the task on average across benchmarks.
- **Sota Band**: beats
- **Access Constraint**: Fully open-source; 32 GB weights

### LPM 1.0
- **Vendor**: Unknown
- **Category**: multimodal
- **Timestamp**: [35:06](https://www.youtube.com/watch?v=1_5sSJK2rU0&t=2106)
- **Why It Matters**: Generates full conversational avatars in real time, with natural facial expressions, eye movements, and body language. Maintains identity consistency over 45+ minutes, a major improvement over other video generators.
- **Sota Comparison**: One of the most realistic and natural avatar generators, with real-time performance.
- **Sota Band**: beats
- **Access Constraint**: Technical report only; no open-source indication

### Unified Vector Floor Plan Generation
- **Vendor**: Unknown
- **Category**: tool
- **Timestamp**: [39:04](https://www.youtube.com/watch?v=1_5sSJK2rU0&t=2344)
- **Why It Matters**: Generates floor plans from text descriptions using a structured markup language (FML), enabling variable room and door configurations. Treats floor plan generation as a language problem.
- **Sota Comparison**: Improvement over previous methods for variable layouts.
- **Sota Band**: beats
- **Access Constraint**: Technical paper only



## Wider context

This week marks a turning point where the most powerful frontier models are being withheld (Claude Mythos) while open-source alternatives like GLM 5.1 close the gap on agentic coding. The trend is clear: capability is no longer the bottleneck—safety and access are. With China's labs (Alibaba, ZAI, DeepSeek) shipping state-of-the-art open models, the closed-source frontier is losing its edge, forcing labs like Anthropic to differentiate on safety rather than raw performance.

## Read next

[[open-source-ai]] · [[ai-safety]] · [[agentic-coding]] · [[world-models]] · [[video-generation]] · [[kv-cache-compression]]
