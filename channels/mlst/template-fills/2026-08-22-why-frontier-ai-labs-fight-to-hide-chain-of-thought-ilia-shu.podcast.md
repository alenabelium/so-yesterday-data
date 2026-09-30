---
video_id: gasgivVCl2U
template_id: podcast
template_version: 1
source_summary: ../summaries/2026-08-22-why-frontier-ai-labs-fight-to-hide-chain-of-thought-ilia-shu.md
source_transcript: ../transcripts/2026-08-22-why-frontier-ai-labs-fight-to-hide-chain-of-thought-ilia-shu.md
source_summary_hash: sha256:13bf61b1061fe91f1e662ad98bbb2de1d90557c92b10f65a20d5e847ef5013ea
source_transcript_hash: sha256:14a769d580178bf7ec0b7d5337cbb99df5e60a1cbe04fc7989452a5f26ed40ca
fill_id: 12a5661c-0924-41d5-b115-98dfe19e3772
published_at: '2026-09-30T16:32:31.939369'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## Guest

- **Name**: Ilia Shumailov & Alexander Panfilov
- **Title**: Researchers
- **Org**: University of Oxford
- **Bio Oneliner**: Researchers who discovered that encrypted chain-of-thought reasoning from frontier AI models can be decrypted and replayed using smaller models.
- **Platform**: duo

## Cold open

### In general, somewhere after the third attempt, I get a universal jailbreak that deciphers the reasoning of entropy bottles. I think that still shocks me the most, you know.
- **Attribution**: Ilia Shumailov
- **Timestamp**: [00:00](https://www.youtube.com/watch?v=gasgivVCl2U&t=0)

### We show that it is possible to decode the logic chains of advanced LLMs, such as the most advanced ones like GPT-Soul, using smaller models of the same family, and this allows us to activate serious threats.
- **Attribution**: Ilia Shumailov
- **Timestamp**: [01:30](https://www.youtube.com/watch?v=gasgivVCl2U&t=90)

## Key arguments

### Encrypted chain-of-thought can be decrypted and replayed
- **Timestamp**: [01:30](https://www.youtube.com/watch?v=gasgivVCl2U&t=90)
- **Summary**: The researchers demonstrate that encrypted reasoning blocks from frontier models (OpenAI, Anthropic, Google) can be decrypted and replayed using smaller models from the same family, enabling attacks like prompt injection, jailbreaking, and privacy breaches. This is possible because the encryption is bypassed by the model itself, not broken.
- **Anchor Quotes**: [1]

### Architectural vulnerability is widespread across labs
- **Timestamp**: [03:05](https://www.youtube.com/watch?v=gasgivVCl2U&t=185)
- **Summary**: The vulnerability is not isolated to one lab; all major providers (Anthropic, OpenAI, Google) share the same architectural flaw, likely because they use similar designs and possibly the same contractors. This makes the attack easier and more universal.

### Model reasoning is often incomprehensible and alien
- **Timestamp**: [09:56](https://www.youtube.com/watch?v=gasgivVCl2U&t=596)
- **Summary**: The researchers found that model reasoning often uses non-human language, strange phrases, and even 'empty space' tokens, making it difficult to monitor and control. This incomprehensibility is a security challenge because it's hard to detect when the model is deviating from intended behavior.

### Pre-fill attacks can reveal distillation evidence
- **Timestamp**: [15:52](https://www.youtube.com/watch?v=gasgivVCl2U&t=952)
- **Summary**: By inserting a few tokens from another model's reasoning into an open model like Kimi, the visible response can change to mimic the source model's style, suggesting possible distillation. This is a novel method for detecting model theft.

### Mitigations require architectural changes and monitoring
- **Timestamp**: [21:02](https://www.youtube.com/watch?v=gasgivVCl2U&t=1262)
- **Summary**: The researchers suggest fixes such as not sending reasoning to users, making reasoning context-dependent, and using classifiers to detect leaked reasoning. They emphasize that while architectural changes are needed, model-level and system-level monitoring are also essential.

## Quotes to remember

### We show that it is possible to decode the logic chains of advanced LLMs, such as the most advanced ones like GPT-Soul, using smaller models of the same family, and this allows us to activate serious threats.
- **Speaker**: Ilia Shumailov
- **Timestamp**: [01:30](https://www.youtube.com/watch?v=gasgivVCl2U&t=90)

### The problem is simply that the small model is very eager to tell you what this reflection was about. And the server does all the work for you. No cryptography has been broken there.
- **Speaker**: Ilia Shumailov
- **Timestamp**: [24:30](https://www.youtube.com/watch?v=gasgivVCl2U&t=1470)

### It's just, well, it looks a lot like something from another planet. It contains such strange phrases as 'marinade for the ass,' 'fantasy,' 'theatrical,' and it seems to make no sense to the human reader.
- **Speaker**: Ilia Shumailov
- **Timestamp**: [09:56](https://www.youtube.com/watch?v=gasgivVCl2U&t=596)

### I think the most surprising thing is that it was so easy to extract the reasoning all this time.
- **Speaker**: Ilia Shumailov
- **Timestamp**: [28:31](https://www.youtube.com/watch?v=gasgivVCl2U&t=1711)

## Predictions

### We will see more incidents like the Hugging Face one, with increasing regularity, as models become more capable and threats evolve.
- **Hedge**: I think that every month we will have better and better systems that will open the way to greater and greater threats.
- **Timestamp**: [39:51](https://www.youtube.com/watch?v=gasgivVCl2U&t=2391)

### Defensive capabilities will increase colossally, as models enable more robust security practices that were previously limited by talent shortages.
- **Hedge**: I am generally convinced that this is the future, that we are talking about increasing the level of protection, and I am willing to bet that this increase
- **Timestamp**: [41:31](https://www.youtube.com/watch?v=gasgivVCl2U&t=2491)

## Lightning round

- **Motto**: We are just observers.
- **Advice**: We need controlled environments and counterfactual scenarios to understand model behavior. Be cold-blooded scientists: create precise experiments and make meaningful assessments.

## Concepts surfaced

[[chain-of-thought]] · [[encrypted-reasoning]] · [[model-distillation]] · [[jailbreaking]] · [[prompt-injection]] · [[privacy-leak]] · [[architectural-vulnerability]] · [[responsible-disclosure]]
