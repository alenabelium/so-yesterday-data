---
video_id: ixu0H8bsCts
template_id: podcast
template_version: 1
source_summary: ../summaries/2026-09-14-speech-recognition-is-not-a-solved-problem-pavan-kumar-reddy.md
source_transcript: ../transcripts/2026-09-14-speech-recognition-is-not-a-solved-problem-pavan-kumar-reddy.md
source_summary_hash: sha256:2ec4205338db3555f2711d5fd0bfaa36b811eca20f48a9742c89e4e4369431ad
source_transcript_hash: sha256:69ca6ef4ca5d15c695249b53e49e991c7a29d7c42a9acdb1de8c6a8f606a735e
fill_id: c896d01d-e08c-4d8e-8760-32f5c41a8a12
published_at: '2026-09-30T19:26:52.972197'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## Guest

- **Name**: Pavan Kumar Reddy
- **Title**: Audio Research Lead
- **Org**: Mistral AI
- **Bio Oneliner**: Leads audio research at Mistral AI, focusing on multimodal models, speech recognition, and generation.
- **Platform**: duo

## Cold open

### I think many people don't understands how it works audio generation. The voice is probably one of the main ways of communication people. He certainly is. appeared much earlier than the text.
- **Attribution**: Pavan Kumar Reddy
- **Timestamp**: [00:00](https://www.youtube.com/watch?v=ixu0H8bsCts&t=0)

### The world looked completely otherwise, I think, thanks to neural codecs and autoregressive generation, it was cool that the industry is so advanced.
- **Attribution**: Pavan Kumar Reddy
- **Timestamp**: [00:00](https://www.youtube.com/watch?v=ixu0H8bsCts&t=0)

## Key arguments

### Speech recognition remains unsolved in real-world scenarios
- **Timestamp**: [01:28:06](https://www.youtube.com/watch?v=ixu0H8bsCts&t=5286)
- **Summary**: Despite claims that ASR is solved, customers report many errors in specific deployments, especially with language coverage and acoustic conditions. Models degrade sharply outside popular languages and struggle with background noise, making customization essential.

### End-to-end audio understanding beats cascades
- **Timestamp**: [11:10](https://www.youtube.com/watch?v=ixu0H8bsCts&t=670)
- **Summary**: Voice Style Chat processes audio directly, avoiding error propagation from intermediate transcriptions. This native approach allows querying emotions and time tags without lossy intermediate representations, leveraging attention to focus on relevant audio parts.

### Streaming transcription balances delay and accuracy
- **Timestamp**: [21:47](https://www.youtube.com/watch?v=ixu0H8bsCts&t=1307)
- **Summary**: Streaming models use a target delay parameter to control how long the model waits before outputting text, trading off ambiguity and error rate. Flexible delay settings allow users to optimize for real-time subtitles or higher accuracy with more context.

### Continuous latents and flow matching improve TTS
- **Timestamp**: [31:03](https://www.youtube.com/watch?v=ixu0H8bsCts&t=1863)
- **Summary**: Mistral's TTS uses continuous latent embeddings with flow matching instead of discrete neural codecs, reducing autoregressive steps and avoiding the bottleneck of compression. This approach offers better control over generation quality and variability.

### DPO reduces hallucinations via negative supervision
- **Timestamp**: [01:03:12](https://www.youtube.com/watch?v=ixu0H8bsCts&t=3792)
- **Summary**: DPO provides a mechanism for negative supervision, penalizing degenerate generations like infinite loops or skipped segments. By training on winner-loser pairs, the model learns to avoid these errors while preserving SFT-learned behaviors.

## Quotes to remember

### The voice is probably one of the main ways of communication people. He certainly is. appeared much earlier than the text.
- **Speaker**: Pavan Kumar Reddy
- **Timestamp**: [00:00](https://www.youtube.com/watch?v=ixu0H8bsCts&t=0)

### The longer you wait, the less ambiguities, and the lower probability of errors.
- **Speaker**: Pavan Kumar Reddy
- **Timestamp**: [23:16](https://www.youtube.com/watch?v=ixu0H8bsCts&t=1396)

### I think that current voice stack, being cascading, also gives many observability for system and interpretability, because the interface each of components are natural language.
- **Speaker**: Pavan Kumar Reddy
- **Timestamp**: [01:25:56](https://www.youtube.com/watch?v=ixu0H8bsCts&t=5156)

### I think that in real conditions productivity is the main problem that not yet decided for many environments, and Language coverage is what what I keep hearing about, when it comes to audio models.
- **Speaker**: Pavan Kumar Reddy
- **Timestamp**: [01:31:32](https://www.youtube.com/watch?v=ixu0H8bsCts&t=5492)

### I think that voice technologies will become enough ubiquitous throughout the next 5 years.
- **Speaker**: Pavan Kumar Reddy
- **Timestamp**: [01:32:26](https://www.youtube.com/watch?v=ixu0H8bsCts&t=5546)

## Predictions

### Voice technologies will become ubiquitous within the next 5 years, with voice assistants integrated into daily work and life.
- **Hedge**: I think
- **Timestamp**: [01:32:26](https://www.youtube.com/watch?v=ixu0H8bsCts&t=5546)

### Future voice interfaces will be a combination of visual and audio, with voice as an auxiliary tool rather than the sole interface.
- **Hedge**: probably
- **Timestamp**: [01:39:04](https://www.youtube.com/watch?v=ixu0H8bsCts&t=5944)

## Lightning round

- **Motto**: Voice is the main way of communication; it appeared much earlier than text.
- **Advice**: For real-world deployments, customize models to your specific acoustic conditions and language coverage; don't rely on general-purpose models alone.

## Concepts surfaced

[[speech-recognition]] · [[neural-codec]] · [[autoregressive-generation]] · [[flow-matching]] · [[speaker-diarization]] · [[dpo]] · [[cascade-systems]] · [[multimodal-models]]
