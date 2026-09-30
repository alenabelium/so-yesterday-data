---
title: "Speech Recognition Is Not a Solved Problem — Pavan Kumar Reddy"
video_id: ixu0H8bsCts
date: 2026-09-14
url: https://www.youtube.com/watch?v=ixu0H8bsCts
channel: Machine Learning Street Talk
tags:
  - ai-agents
  - ai-strategy
  - llm-fundamentals
  - industry-news
transcript: ../transcripts/2026-09-14-speech-recognition-is-not-a-solved-problem-pavan-kumar-reddy.md
relevant: true
knowledge: true
highlight: true
---

# Speech Recognition Is Not a Solved Problem — Pavan Kumar Reddy

## Executive Summary

Pavan Kumar Reddy, an audio research lead at Mistral AI, argues that speech recognition remains an unsolved problem despite advances in neural codecs and autoregressive generation. He discusses Mistral's audio models, including Voice Style Chat for audio understanding and a streaming transcription model, emphasizing the trade-offs between cascaded and end-to-end approaches. The conversation covers technical topics like continuous latent variables, flow matching for TTS, speaker diarization challenges, and the use of DPO to reduce hallucinations. Reddy concludes that while voice interfaces will become ubiquitous, current systems still struggle with real-world acoustic conditions and language coverage, and he advocates for customizable, component-based solutions over monolithic models.

## Key Points

- Speech recognition is not solved; real-world deployments face errors in specific scenarios, especially with noisy environments and less common languages. [29:33](https://www.youtube.com/watch?v=ixu0H8bsCts&t=1773)
- Mistral's audio understanding model (Voice Style Chat) processes audio directly, avoiding cascaded transcription errors and enabling queries about emotions and timestamps. [09:49](https://www.youtube.com/watch?v=ixu0H8bsCts&t=589)
- Streaming transcription models use a target delay parameter to balance quality and latency, with longer delays reducing ambiguity and errors. [23:16](https://www.youtube.com/watch?v=ixu0H8bsCts&t=1396)
- For TTS, Mistral uses continuous latent embeddings with flow matching instead of discrete neural codecs, allowing finer control over generation steps and quality. [35:03](https://www.youtube.com/watch?v=ixu0H8bsCts&t=2103)
- Speaker diarization remains a difficult problem, especially with overlapping speech; models can be superhuman but still struggle with multi-speaker noisy environments. [56:36](https://www.youtube.com/watch?v=ixu0H8bsCts&t=3396)
- DPO is used to reduce hallucinations and degenerate generation in ASR models by providing negative supervision, complementing positive-only training like SFT. [01:04:38](https://www.youtube.com/watch?v=ixu0H8bsCts&t=3878)
