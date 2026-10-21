---
title: "New top local AI image generator is here!"
video_id: cUeZMUGCxrw
date: 2026-10-20
url: https://www.youtube.com/watch?v=cUeZMUGCxrw
channel: The AI Search
tags:
  - ai-tools
  - tutorials
  - ai-agents
transcript: ../transcripts/2026-10-20-new-top-local-ai-image-generator-is-here.md
relevant: true
knowledge: true
highlight: true
---

# New top local AI image generator is here!

## Executive Summary

Moss Image is a new open-source, 5-billion-parameter text-to-image generator that delivers high-quality results, including realistic images, anime, and complex infographics, while being small enough to run on GPUs with as little as 4GB of VRAM. The video demonstrates how to install and use Moss Image via ComfyUI, including downloading models, using layout control with bounding boxes, adding LoRAs for style customization, and applying turbo LoRAs to speed up generation. It also covers traditional inpainting for image editing and mentions fine-tuned checkpoints like Chromos for improved quality. The presenter concludes that Moss Image is the best model in its weight class and anticipates rapid community improvements.

## Key Points

- Moss Image is a compact 5B-parameter open-source text-to-image generator that excels at realistic images, anime, and text-heavy infographics, and can run on GPUs with 4GB VRAM or less. [00:00:00](https://www.youtube.com/watch?v=cUeZMUGCxrw&t=0)
- Installation via ComfyUI involves downloading the SFT diffusion model, a text encoder (e.g., Qwen 3.5 9B), and a VAE, then selecting them in the workflow; the int8 versions are recommended for lower VRAM. [00:04:51](https://www.youtube.com/watch?v=cUeZMUGCxrw&t=291)
- Moss Image supports layout control through bounding boxes, allowing precise placement of objects in the image, as demonstrated with a complex scene containing a woman, sofa, coffee table, window, and a Naruto poster. [00:09:32](https://www.youtube.com/watch?v=cUeZMUGCxrw&t=572)
- Adding LoRAs (e.g., Sumi ink style) enhances flexibility, and using an 8-step DMD LoRA with CFG=1 can speed up generation by 3-4 times. [00:12:23](https://www.youtube.com/watch?v=cUeZMUGCxrw&t=743)
- Image editing is possible via traditional inpainting in ComfyUI, though it is less flexible than semantic editors like Nano Banana; fine-tuned checkpoints like Chromos offer improved quality. [00:18:03](https://www.youtube.com/watch?v=cUeZMUGCxrw&t=1083)
