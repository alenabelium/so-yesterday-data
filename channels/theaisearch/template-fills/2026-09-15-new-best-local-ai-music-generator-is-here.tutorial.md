---
video_id: 9RtywbN--QE
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-09-15-new-best-local-ai-music-generator-is-here.md
source_transcript: ../transcripts/2026-09-15-new-best-local-ai-music-generator-is-here.md
source_summary_hash: sha256:22dacac5f37405a1c7b2a6601f5b597efe25ab72ff24601a8d18618471c01b55
source_transcript_hash: sha256:fc167d2482f882ced9fea8b456acda9cc2bb21fe6f60dd5e8316c7967e126862
fill_id: a5bc842b-64cd-4141-a0ab-0271db8899f5
published_at: '2026-09-29T11:24:37.496479'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Install UA2 in Comfy UI to generate original songs or covers with as little as 4 GB VRAM.

## Prerequisites

### Comfy UI
- **Kind**: tool
- **Note**: Latest version installed locally. Update via update Comfy.bat in the root folder.

### GPU with VRAM
- **Kind**: hardware
- **Note**: Minimum 4 GB VRAM for quantized model; 8+ GB recommended for BF-16 version.

### UA2 Workflow JSON
- **Kind**: tool
- **Note**: Download the pre-built workflow file from the video description link.

## Steps

### Update Comfy UI
- **Timestamp**: [12:05](https://www.youtube.com/watch?v=9RtywbN--QE&t=725)
- **Action**: Navigate to your Comfy UI root directory, open the update folder, and run the batch file to ensure you have the latest version.
- **Command Or Clicks**: Double click on update Comfy.bat in the update folder. Press any key to exit after it finishes.

### Load UA2 Workflow
- **Timestamp**: [13:00](https://www.youtube.com/watch?v=9RtywbN--QE&t=780)
- **Action**: Download the UA2 workflow JSON file from the description, save it locally, and drag it into the Comfy UI interface to load the pre-built nodes.
- **Command Or Clicks**: Drag the downloaded UA2 workflow JSON file onto the Comfy UI interface.

### Download Models
- **Timestamp**: [13:24](https://www.youtube.com/watch?v=9RtywbN--QE&t=804)
- **Action**: Download the required audio encoder and model checkpoint from the description links. Place the encoder in models/audio_encoders and the checkpoint in models/checkpoints.
- **Command Or Clicks**: Save audio encoder to Comfy UI/models/audio_encoders. Save BF-16 (7.8GB) or quantized (3.96GB) checkpoint to Comfy UI/models/checkpoints.
- **Choice Branch**: Choose BF-16 for >8GB VRAM; choose quantized for <4GB VRAM.

### Refresh and Select Model
- **Timestamp**: [14:20](https://www.youtube.com/watch?v=9RtywbN--QE&t=860)
- **Action**: Refresh the model list in Comfy UI to recognize the newly downloaded files, then select the checkpoint in the load node.
- **Command Or Clicks**: Press R to refresh. Open the dropdown on the load checkpoint node and select your downloaded model file.

### Configure Text-to-Music
- **Timestamp**: [14:45](https://www.youtube.com/watch?v=9RtywbN--QE&t=885)
- **Action**: Enter your style prompt and lyrics (using metatags like [verse]) in the top nodes. Adjust seed, steps, and CFG as needed.
- **Command Or Clicks**: Input text into style prompt and lyrics boxes. Set max duration, seed, and steps in the sampler node.
- **Choice Branch**: Set seed to random for variety; keep fixed for reproducibility.

### Connect Decoding Path
- **Timestamp**: [16:30](https://www.youtube.com/watch?v=9RtywbN--QE&t=990)
- **Action**: Connect the audio input to the regular decode node if you have >12GB VRAM, bypassing the tiled version. Then run the generation.
- **Command Or Clicks**: Shift+click and drag connection to regular decode node. Ctrl+B to bypass tiled node. Press Run.
- **Choice Branch**: Use tiled decode if VRAM is <12 GB.

### Setup Audio Reference Mode
- **Timestamp**: [21:00](https://www.youtube.com/watch?v=9RtywbN--QE&t=1260)
- **Action**: Unbypass the bottom nodes, connect the audio encoder output to the generate music node, upload your reference audio, and set style/lyrics.
- **Command Or Clicks**: Ctrl+B to unbypass purple nodes. Connect load audio encoder output to generate music node. Upload audio file.
- **Choice Branch**: Select 'melody only' for covers or 'full song' for style transfer.

## Gotchas

### Model weights are licensed under Creative Commons Non-Commercial, prohibiting commercial use or monetization of generations.
- **Severity**: serious
- **Timestamp**: [23:15](https://www.youtube.com/watch?v=9RtywbN--QE&t=1395)

### If your GPU has less than 12 GB VRAM, you must use the tiled decode method instead of the regular decode for stability.
- **Severity**: blocking
- **Timestamp**: [16:45](https://www.youtube.com/watch?v=9RtywbN--QE&t=1005)

### The generated song may exceed your specified max duration if the lyrics are long; reduce max duration to match lyric length.
- **Severity**: heads_up
- **Timestamp**: [18:30](https://www.youtube.com/watch?v=9RtywbN--QE&t=1110)

## Where to go next

UA2's Apache 2 code allows for local modification, while its CC BY-NC weights restrict commercial deployment. Explore the GitHub repo for technical details on the editable score generation mechanism.

## Concepts surfaced

[[local-ai-music]] · [[comfy-ui-tutorial]] · [[open-source-models]] · [[audio-generation-workflow]] · [[creative-commons-license]]
