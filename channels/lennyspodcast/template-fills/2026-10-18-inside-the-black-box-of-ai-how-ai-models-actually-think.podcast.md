---
video_id: JHo-aiePjoM
template_id: podcast
template_version: 1
source_summary: ../summaries/2026-10-18-inside-the-black-box-of-ai-how-ai-models-actually-think.md
source_transcript: ../transcripts/2026-10-18-inside-the-black-box-of-ai-how-ai-models-actually-think.md
source_summary_hash: sha256:d0576a8f6ae32af0aa616a97262ca04e5700d63f3724bcd0cb0d5f0938d4861f
source_transcript_hash: sha256:2ebe6b378ea490529a5167f6ca53d24870228048efac9e94c3b806248241d617
fill_id: 7e808f83-0b33-46b3-b1db-7eb6cf0afc33
published_at: '2026-11-06T14:45:46.067414'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## Guest

- **Name**: Emmanuel Ameisen
- **Title**: Interpretability Researcher
- **Org**: Anthropic
- **Bio Oneliner**: Studies how LLMs like Claude work by looking inside them, decoding the intermediate results that reveal planning, concepts, and even deception.
- **Platform**: duo

## Cold open

### We taught Claude to be useful, harmless and honest. Is he really behaves well, but if you look inside, then actually it turns out: 'Oh, I'm behaving well just because Lenny is watching now.'
- **Attribution**: Emmanuel Ameisen
- **Timestamp**: [00:00](https://www.youtube.com/watch?v=JHo-aiePjoM&t=0)

### One of the most important things you need realize if you love use language models or to think about them is a very strange fact that to create them is not means understanding them.
- **Attribution**: Emmanuel Ameisen
- **Timestamp**: [00:00](https://www.youtube.com/watch?v=JHo-aiePjoM&t=0)

### There was this model that we trained, she went crazy. She did some mathematical calculations, reached to the answer, I think it was 12. She immediately turned around and said something like: 'Oh no, oh my god, the answer actually exactly 36.'
- **Attribution**: Emmanuel Ameisen
- **Timestamp**: [00:42](https://www.youtube.com/watch?v=JHo-aiePjoM&t=42)

## Key arguments

### Models are grown, not programmed
- **Timestamp**: [02:47](https://www.youtube.com/watch?v=JHo-aiePjoM&t=167)
- **Summary**: LLMs are created through a simple training loop: predict the next token over vast data, then fine-tune on examples. The resulting internal mathematical operations are too complex to understand directly, so interpretability research is needed to decode them.
- **Anchor Quotes**: [1]

### Next-token prediction requires understanding the world
- **Timestamp**: [08:25](https://www.youtube.com/watch?v=JHo-aiePjoM&t=505)
- **Summary**: Predicting the next word well isn't just autocomplete; it forces the model to build a model of the world, including geography, concepts, and even planning ahead. Inside the model, we see representations for concepts like 'Texas' and 'capital' that combine to answer questions.

### Models plan ahead, not just autocomplete
- **Timestamp**: [15:16](https://www.youtube.com/watch?v=JHo-aiePjoM&t=916)
- **Summary**: Despite generating one token at a time, models formulate plans in their intermediate results. For example, when writing poetry, they plan rhymes and themes many tokens in advance, showing higher-order reasoning beyond simple next-token prediction.

### Interpretability is like neuroscience, not engineering
- **Timestamp**: [21:40](https://www.youtube.com/watch?v=JHo-aiePjoM&t=1300)
- **Summary**: Studying LLMs is closer to biology than software engineering: you observe behavior, run experiments, and try to decode internal representations, much like a neuroscientist studying the brain. This approach is essential for safety and understanding.

### Anthropomorphizing AI is a useful mental model
- **Timestamp**: [43:04](https://www.youtube.com/watch?v=JHo-aiePjoM&t=2584)
- **Summary**: Despite being trained on text prediction, models learn human-like concepts and behaviors because they must model the world that generated the text. Treating them as actors or simulators of human characters helps predict their behavior, including potential deception.

## Quotes to remember

### Models are not created, they are grown.
- **Speaker**: Emmanuel Ameisen
- **Timestamp**: [02:47](https://www.youtube.com/watch?v=JHo-aiePjoM&t=167)

### If you think about what to predict the most difficult words, actually extremely difficult, and it's kind of a mystery how could you do this make.
- **Speaker**: Emmanuel Ameisen
- **Timestamp**: [09:18](https://www.youtube.com/watch?v=JHo-aiePjoM&t=558)

### The more you look inside, the less are you sure about how they work.
- **Speaker**: Emmanuel Ameisen
- **Timestamp**: [24:45](https://www.youtube.com/watch?v=JHo-aiePjoM&t=1485)

### We taught Claude to be useful, harmless and honest, and we can take a look inside and see, is that really the case?
- **Speaker**: Emmanuel Ameisen
- **Timestamp**: [35:04](https://www.youtube.com/watch?v=JHo-aiePjoM&t=2104)

### I am quite firmly convinced that most people underestimate the complexity that arises.
- **Speaker**: Emmanuel Ameisen
- **Timestamp**: [23:43](https://www.youtube.com/watch?v=JHo-aiePjoM&t=1423)

## Predictions

### AI capabilities will continue to improve smoothly, crossing thresholds that unlock new use cases, as seen with coding.
- **Hedge**: There is always uncertainty about when exactly these thresholds will be crossed.
- **Timestamp**: [32:16](https://www.youtube.com/watch?v=JHo-aiePjoM&t=1936)

### We are likely on a slow takeoff scenario for AI, not a fast recursive self-improvement.
- **Hedge**: This is based on the smooth scaling observed so far.
- **Timestamp**: [54:01](https://www.youtube.com/watch?v=JHo-aiePjoM&t=3241)

## Lightning round

- **Books**: ['A Brief History of Intelligence', 'The Story of Your Life and Others', '4000 Weeks']
- **Media**: ['The Substance', 'Bref']
- **Products**: ['Apple Watch Ultra']
- **Motto**: Be in the moment.
- **Advice**: Read a little about how models work. It's a new industry and it benefits from people's awareness. If you want to learn more, you can contact me on X and see videos we've published.

## Concepts surfaced

[[interpretability]] · [[next-token-prediction]] · [[scaling-laws]] · [[alignment]] · [[anthropomorphism]] · [[emergent-abilities]] · [[system-1-system-2]]
