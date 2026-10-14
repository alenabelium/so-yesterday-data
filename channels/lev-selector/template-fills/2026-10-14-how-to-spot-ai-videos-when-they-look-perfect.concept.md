---
video_id: hMzkEQhIzIs
template_id: concept
template_version: 1
source_summary: ../summaries/2026-10-14-how-to-spot-ai-videos-when-they-look-perfect.md
source_transcript: ../transcripts/2026-10-14-how-to-spot-ai-videos-when-they-look-perfect.md
source_summary_hash: sha256:aa2f7940194f9ca1e2ec1222e7e3bcf75394eb3d48589b30517ad61a6a30455d
source_transcript_hash: sha256:88651f3b18f209fe2a73e697d22da8f0825ff4f3e56b8fec49b4486d4cda7ff1
fill_id: 8e90233c-5a7a-40f8-9553-a71b06481740
published_at: '2026-10-14T15:42:59.611970'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

When AI videos look flawless, visual inspection fails. This framework introduces three levels of verification: checking C2PA digital signatures, detecting invisible watermarks like Google SynthID, and independently verifying events through reverse image search and official sources. The key shift is from asking 'Does this look real?' to asking 'What independent evidence supports that this actually happened?'

## The argument

### Define the Core Substrate
- **Anchor Timestamps**: ['00:00:00']
- **Claim**: The first level is digital origin: C2PA, an open standard for content credentials, provides a cryptographically signed record of the file—what tools were used, what edits were claimed, and who signed those claims. This is the foundation, but it only verifies the integrity of the statements, not the event itself.
- **Role**: definition

### Evidence: Invisible Watermarks
- **Anchor Timestamps**: ['00:01:16']
- **Claim**: The second level is invisible watermarks: Google SynthID embeds a signal into supported AI-generated images, audio, and video. The SynthID detector can verify content from supported systems. This is valuable evidence, but its absence does not prove the video was captured on camera, since not every generator uses SynthID.
- **Role**: evidence

### Counter: The Limits of Signatures and Detectors
- **Anchor Timestamps**: ['00:01:16']
- **Claim**: A valid C2PA signature does not prove the event actually occurred, and the absence of C2PA data is not proof of forgery because platforms can remove metadata. Similarly, a detector showing 99% AI is not mathematical proof—it's a model estimate, and models make mistakes.
- **Role**: counter

### Synthesis: Independent Event Verification
- **Anchor Timestamps**: ['00:02:42']
- **Claim**: The third and most important level is verifying the event independently: use the InVid WeVerify extension to extract keyframes and reverse image search them. If a flawless clip of an explosion near an airport finds an older upload or official sources don't confirm the incident, that's stronger evidence than any visual flaw.
- **Role**: synthesis

## Evidence and caveats

The speaker's worked example: a viral clip of an explosion near an airport looks flawless, but reverse image search finds a similar video from 2 years ago, and official sources and local reporters do not confirm the incident. This is more important than noticing a strange finger. Caveats: a valid C2PA signature only verifies the integrity of the statements, not that the event occurred; absence of C2PA data is not proof of forgery because platforms can remove metadata; absence of SynthID does not mean the video was captured on camera because not every generator uses it; and a detector showing 99% AI is a model estimate, not mathematical proof.

## Concepts surfaced

[[c2pa-content-credentials]] · [[synthid-watermark]] · [[reverse-image-search]] · [[invidd-weverify]] · [[generative-video-detection]]
