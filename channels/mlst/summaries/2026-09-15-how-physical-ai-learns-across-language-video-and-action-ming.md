---
title: "How Physical AI Learns Across Language, Video and Action — Ming-Yu Liu"
video_id: L6tLBApQN-g
date: 2026-09-15
url: https://www.youtube.com/watch?v=L6tLBApQN-g
channel: Machine Learning Street Talk
tags:
  - ai-agents
  - ai-strategy
  - ai-tools
  - llm-fundamentals
transcript: ../transcripts/2026-09-15-how-physical-ai-learns-across-language-video-and-action-ming.md
relevant: true
knowledge: true
highlight: true
---

# How Physical AI Learns Across Language, Video and Action — Ming-Yu Liu

## Executive Summary

Ming-Yu Liu discusses Nvidia's Cosmos 3, a world model that integrates language, video, audio, and action to enable physical AI systems like robots and autonomous vehicles to learn and simulate interactions. The model combines a visual-language model with a diffusion-based generator, trained on multiple modalities and time scales, to support tasks like forward dynamics, reverse dynamics, and strategy learning. Liu highlights the use of Cosmos as a neural simulator for policy verification, reducing the need for real-world testing, and introduces Cosmos Streams for closed-loop simulation and Cosmos Edge for on-device deployment. He emphasizes the importance of open models, recipes, and community feedback to accelerate development in physical AI.

## Key Points

- Cosmos 3 is a unified model that processes text, video, audio, and actions, enabling tasks like video understanding, generation, and robot control. [00:00:00](https://www.youtube.com/watch?v=L6tLBApQN-g&t=0)
- The model combines an autoregressive visual-language model with a bidirectional diffusion generator, ensuring consistency across generated video, actions, and audio. [00:03:07](https://www.youtube.com/watch?v=L6tLBApQN-g&t=187)
- A time-positional embedding scheme normalizes different signal frequencies (video, audio, actions) to a common time scale, enabling the model to process multimodal inputs effectively. [00:06:48](https://www.youtube.com/watch?v=L6tLBApQN-g&t=408)
- Training with an information bottleneck across forward dynamics, reverse dynamics, and strategy creates synergy, allowing transfer from human video data to robot action learning. [00:08:15](https://www.youtube.com/watch?v=L6tLBApQN-g&t=495)
- Cosmos can be used as a world simulator for passive policy verification, ranking policies by success rate in simulation to reduce expensive real-world testing. [00:13:47](https://www.youtube.com/watch?v=L6tLBApQN-g&t=827)
- Cosmos Streams provides a toolkit for building closed-loop simulators for various embodiments, while Cosmos Edge runs on-device for real-time, low-latency deployment. [00:19:24](https://www.youtube.com/watch?v=L6tLBApQN-g&t=1164)
