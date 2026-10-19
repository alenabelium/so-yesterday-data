---
title: "FASTER Fourier Transform? Is O-notation a scam??"
video_id: C-lYf2OvU8I
date: 2026-10-14
url: https://www.youtube.com/watch?v=C-lYf2OvU8I
channel: Dr. Samuel Allen Alexander
tags:
  - ai-strategy
  - llm-fundamentals
  - opinion
  - ai-tools
transcript: ../transcripts/2026-10-14-faster-fourier-transform-is-o-notation-a-scam.md
relevant: true
knowledge: true
highlight: true
---

# FASTER Fourier Transform? Is O-notation a scam??

## Executive Summary

Dr. Samuel Allen Alexander discusses OpenAI's claimed faster Fourier transform algorithm, which is asymptotically faster than the Cooley-Tukey FFT but only for astronomically large inputs, making it a 'galactic algorithm' with no practical use. He explains how big O notation can be abused, leading to theoretical results that are disconnected from real-world computing. The video also critiques the culture of theoretical computer science that rewards such impractical results, while defending the mathematical validity of the work. Alexander uses a Socratic dialogue to illustrate the complexities of replacing big O notation with simpler alternatives.

## Key Points

- OpenAI's new Fourier transform algorithm is asymptotically faster than the classic Cooley-Tukey FFT, but only for inputs larger than a googolplex, making it practically useless. [00:08:39](https://www.youtube.com/watch?v=C-lYf2OvU8I&t=519)
- The algorithm relies on an unrealistic computational model with exact complex arithmetic and unbounded coefficients, which would require exponential memory in practice. [00:09:46](https://www.youtube.com/watch?v=C-lYf2OvU8I&t=586)
- Big O notation can hide enormous constants, leading to 'galactic algorithms' that are theoretically faster but never practical, a problem highlighted by Ben Recht and others. [00:06:56](https://www.youtube.com/watch?v=C-lYf2OvU8I&t=416)
- Theoretical computer science often rewards impractical results, and AI is now automating this tendency, but such results still have mathematical value, akin to Einstein's relativity being irrelevant for bridge-building. [00:15:04](https://www.youtube.com/watch?v=C-lYf2OvU8I&t=904)
- A Socratic dialogue demonstrates why replacing big O notation with simple real numbers is impossible without losing the essential distinctions between complexity classes. [00:19:22](https://www.youtube.com/watch?v=C-lYf2OvU8I&t=1162)
