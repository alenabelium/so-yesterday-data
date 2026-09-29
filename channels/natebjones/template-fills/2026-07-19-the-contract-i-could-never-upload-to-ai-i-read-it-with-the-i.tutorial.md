---
video_id: 5slsNizN6MQ
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-07-19-the-contract-i-could-never-upload-to-ai-i-read-it-with-the-i.md
source_transcript: ../transcripts/2026-07-19-the-contract-i-could-never-upload-to-ai-i-read-it-with-the-i.md
source_summary_hash: sha256:64bafb7e861a1f4f24c265df44239e60c725366fc70abd12785b6d84fc30ccdc
source_transcript_hash: sha256:a69bd298185102b49f1844d01fb1ea7bd14f740e011bb458a6cc3a3a08e9f189
fill_id: e98c9e01-abcd-455c-921c-982e1558e7ea
published_at: '2026-09-29T11:20:45.203493'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Use LM Studio with offline models to scan and mask PII in contracts without internet access.

## Prerequisites

### LM Studio
- **Kind**: tool
- **Note**: Download and install the local AI model runner.

### GPT-OSS Safeguard 20B
- **Kind**: tool
- **Note**: Download this specific open-weight model for local inference.

### Offline Environment
- **Kind**: knowledge
- **Note**: Turn off Wi-Fi to ensure no data leaves your machine.

## Steps

### Prepare Offline Environment
- **Timestamp**: [00:00](https://www.youtube.com/watch?v=5slsNizN6MQ&t=0)
- **Action**: Ensure the laptop has no internet connection to guarantee data privacy during the AI processing.
- **Command Or Clicks**: Turn off Wi-Fi.

### Download Model and Preset
- **Timestamp**: [04:15](https://www.youtube.com/watch?v=5slsNizN6MQ&t=255)
- **Action**: Download the GPT-OSS Safeguard 20B model and save a sensitivity instruction as a preset (skill) inside LM Studio.
- **Command Or Clicks**: Download GPT-OSS Safeguard 20B. Save preset: 'find private identity, find financial, security, legal, company, or employment information, mask that evidence, and tell me where the work should happen.'

### Run Local Scan
- **Timestamp**: [05:31](https://www.youtube.com/watch?v=5slsNizN6MQ&t=331)
- **Action**: Load the sensitive document into LM Studio. The model runs entirely locally to identify and mask private data.
- **Command Or Clicks**: Load document. Verify model output masks credentials and flags unreadable sections.

## Gotchas

### Cloud models may leak data even if they claim not to look at files. Always use air-gapped local models for sensitive data.
- **Severity**: blocking
- **Timestamp**: [03:39](https://www.youtube.com/watch?v=5slsNizN6MQ&t=219)

### Open source does not mean vendor-independent. Deep dependence on providers like Microsoft for LoRA training can create lock-in.
- **Severity**: serious
- **Timestamp**: [12:43](https://www.youtube.com/watch?v=5slsNizN6MQ&t=763)

## Where to go next

Check the Substack for the full LM Studio installation guide and the specific preset configuration used in this demo.

## Concepts surfaced

[[local-ai-inference]] · [[data-privacy]] · [[lm-studio]] · [[open-weight-models]] · [[lora-fine-tuning]] · [[air-gapped-security]]
