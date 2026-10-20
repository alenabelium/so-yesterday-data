---
video_id: 9aIYhjeYxzM
template_id: tech-overview
template_version: 1
source_summary: ../summaries/2026-04-28-gpt-55-vs-claude-vs-gemini-the-real-difference-nobodys-talki.md
source_transcript: ../transcripts/2026-04-28-gpt-55-vs-claude-vs-gemini-the-real-difference-nobodys-talki.md
source_summary_hash: sha256:c2a17b997f84257b3daabf8d008bbce5af3973124d9dee59ac4d5e7da09c37a9
source_transcript_hash: sha256:b794877134631a63fc71c097425e7844cc7240da1e3695a4abd72519a96e14be
fill_id: b0514fe2-6e26-4ec6-83df-408fa80b98c9
published_at: '2026-10-20T00:12:04.253145'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

GPT-5.5 is the strongest model in the world today, winning a 23-deliverable executive package by 20 points over Opus 4.7, but it still trails Claude on visual taste and needs validation on backend data hygiene.

## Tools covered

### GPT-5.5
- **Vendor**: OpenAI
- **Category**: reasoning
- **Timestamp**: [00:00](https://www.youtube.com/watch?v=9aIYhjeYxzM&t=0)
- **Why It Matters**: Host's top pick for complex, messy, multi-step work. Scored 87.3 on Dingo vs 67.0 for Opus 4.7, caught planted fake customers in Splash Brothers, and showed strong information density in Artemis 2. Feels like a bigger pre-train, not just more inference compute.
- **Sota Comparison**: Host claims it's the strongest model in the world today, beating Opus 4.7, Sonnet 4.7, and Gemini 3.1 Pro on his private bench.
- **Sota Band**: beats
- **Access Constraint**: Available in ChatGPT and Codex

### Opus 4.7
- **Vendor**: Anthropic
- **Category**: reasoning
- **Timestamp**: [04:31](https://www.youtube.com/watch?v=9aIYhjeYxzM&t=271)
- **Why It Matters**: Still the host's go-to for blank-canvas visual taste and planning. Produced stronger visuals in Artemis 2 and better front-end craft, but scored lower on Dingo (67.0) and missed fake customers in Splash Brothers.
- **Sota Comparison**: Host says it's a real advancement but a bridge release under the shadow of Mythos; trails GPT-5.5 on complex execution.
- **Sota Band**: behind
- **Access Constraint**: Available via Claude

### Gemini 3.1 Pro
- **Vendor**: Google
- **Category**: reasoning
- **Timestamp**: [09:49](https://www.youtube.com/watch?v=9aIYhjeYxzM&t=589)
- **Why It Matters**: Scored 49.8 on Dingo, the lowest of the four. Understood parts of the premise but produced fake file types (HTML/text with wrong extensions), which is a critical failure for real deliverables.
- **Sota Comparison**: Trails GPT-5.5 and Opus 4.7 on the host's executive knowledge work test.
- **Sota Band**: behind
- **Access Constraint**: Available via Gemini

### Codex
- **Vendor**: OpenAI
- **Category**: agent
- **Timestamp**: [20:37](https://www.youtube.com/watch?v=9aIYhjeYxzM&t=1237)
- **Why It Matters**: The environment where 5.5 shines: file access, code editing, browser control, and iterative testing. Host says a model this strong trapped in a chat window is underused; Codex lets it act on real work.
- **Sota Comparison**: Host implies it's the best place to run 5.5 for serious work, compared to ChatGPT's consumer surface.
- **Sota Band**: inferred
- **Access Constraint**: Available via OpenAI

### Images 2.0
- **Vendor**: OpenAI
- **Category**: image
- **Timestamp**: [04:31](https://www.youtube.com/watch?v=9aIYhjeYxzM&t=271)
- **Why It Matters**: Changes the workflow for visual work: generate a mockup, then hand it to 5.5 in Codex to implement faithfully. Host uses it to compensate for 5.5's weaker blank-canvas taste.
- **Sota Comparison**: Host implies it's good enough to design a custom Lego set with accurate part numbers, a capability that didn't exist a week ago.
- **Sota Band**: inferred
- **Access Constraint**: Available via ChatGPT

### Dingo and Company
- **Vendor**: natebjones
- **Category**: other
- **Timestamp**: [07:41](https://www.youtube.com/watch?v=9aIYhjeYxzM&t=461)
- **Why It Matters**: A private benchmark: 23-deliverable executive launch package for a fictional dingo pet tech startup. Tests judgment, production discipline, and artifact quality. GPT-5.5 won by a wide margin (87.3 vs 67.0).
- **Sota Comparison**: GPT-5.5 beats Opus 4.7, Sonnet 4.7, and Gemini 3.1 Pro on this test.
- **Sota Band**: beats
- **Access Constraint**: Private benchmark

### Splash Brothers
- **Vendor**: natebjones
- **Category**: other
- **Timestamp**: [11:36](https://www.youtube.com/watch?v=9aIYhjeYxzM&t=696)
- **Why It Matters**: A dirty data migration test with 465 files and planted traps. GPT-5.5 is the first model to catch fake customers (Mickey Mouse, test customer) and merge duplicates, but still missed backend hygiene like service code conflicts.
- **Sota Comparison**: Host notes 5.5 regressed on some backend discipline vs 5.4, but improved on intuitive catches.
- **Sota Band**: inferred
- **Access Constraint**: Private benchmark

### Artemis 2
- **Vendor**: natebjones
- **Category**: other
- **Timestamp**: [17:39](https://www.youtube.com/watch?v=9aIYhjeYxzM&t=1059)
- **Why It Matters**: Interactive 3D NASA visualization test. GPT-5.5 excelled at information density but looked cartoonish; Opus 4.7 had better visuals but less discoverable info. Host suggests combining Opus's visuals with 5.5's density.
- **Sota Comparison**: Opus 4.7 beats GPT-5.5 on visual composition; GPT-5.5 beats Opus on information density.
- **Sota Band**: parity
- **Access Constraint**: Private benchmark

### GPT-5.5 in Codex
- **Timestamp**: [27:36](https://www.youtube.com/watch?v=9aIYhjeYxzM&t=1656)
- **One Liner**: Host's pick for the strongest default for complex, messy, multi-step work; pairs with Images 2.0 for visual direction.
- **Sota Band**: beats

## Wider context

The frontier is moving faster than benchmarks capture. GPT-5.5's edge isn't just raw scores—it's that the model can carry a task across many steps and tools, compressing the expensive 'nothing to coherent first version' phase. But the host's private tests reveal a nuanced picture: 5.5 is a runaway winner on executive work, yet it regresses on backend hygiene and still can't match Opus on blank-canvas taste. The real shift is routing: using 5.5 in Codex for execution, Opus for taste, and Images 2.0 for visual references. This week's release changes what you can ask a model to do, not just how well it answers.

## Read next

[[multi-model-routing]] · [[agentic-workflows]] · [[benchmark-design]] · [[data-migration]] · [[visual-taste]]
