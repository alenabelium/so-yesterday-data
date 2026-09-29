---
video_id: ltbzgzZZmgI
template_id: concept
template_version: 1
source_summary: ../summaries/2026-05-22-your-ai-writes-from-twenty-sources-it-cannot-tell-which-one.md
source_transcript: ../transcripts/2026-05-22-your-ai-writes-from-twenty-sources-it-cannot-tell-which-one.md
source_summary_hash: sha256:5f4acb5177251cbfaee113657d20825619e139e55bd9ca94c68b4b9a88f9c16f
source_transcript_hash: sha256:7e269adf5ef9b23aa0b9e656550b04136e14d37a9bfb694be5f5cca96b721e00
fill_id: 3849d50d-ff81-4677-ae1d-9dcfe4a9c603
published_at: '2026-05-31T00:57:23.454791'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

Professional AI hallucinations like the Sullivan & Cromwell fabricated-citation filing come from messy source environments, not weak models. The fix is structural: before asking an agent to produce anything, have it build a bounded "data room" and audit the sources. Recent file-capable agents make this the first move of any serious project.

## The argument

### The model is not the problem; the environment is
- **Anchor Timestamps**: [0]
- **Claim**: A top law firm filed a motion with dozens of fabricated citations using the best AI tooling money can buy. You cannot tell a language model not to hallucinate, because there is no separate truth-check pass for the instruction to hook into. The messy working environment around the model is the real source of 2026 hallucinations.
- **Role**: definition

### File-capable agents flip the workflow
- **Anchor Timestamps**: [103]
- **Claim**: Opus 4.7 and GPT 5.5 run long agentic tasks directly on your file system: they walk folder trees, open files, compare dates, and inspect metadata. Because of that, the first useful prompt in a serious project is no longer "write the document" but "build me the room to do the work in."
- **Role**: evidence

### First instruction: organize, do not produce
- **Anchor Timestamps**: [316]
- **Claim**: Asking AI to write from a general mess forces two jobs at once: figure out what the sources are and produce the artifact. Instead, the first instruction should find the relevant materials, preserve originals, and build a data inventory flagging which files are authoritative, duplicate, stale, or missing before synthesizing anything.
- **Role**: synthesis

### Audit artifacts make the agent's judgment legible
- **Anchor Timestamps**: [779]
- **Claim**: The source inventory, conflict log, and missing-context list surface disagreements and gaps without silently resolving them. The missing material is often more important than what you have; asking for the final output too quickly turns those gaps into hallucination traps the model invents its way around.
- **Role**: evidence

### The canvas, and the colleague not the gopher
- **Anchor Timestamps**: [1034]
- **Claim**: Source data is the substrate, the gesso under the canvas; get it wrong and the final work cannot look right. A messy folder can no longer be patched with a sharp prompt because the mess now sits inside the agent's context window. Letting the agent shape the data room with you treats it as a colleague rather than a gopher.
- **Role**: synthesis

## Evidence and caveats

The source inventory is just a table: for every file the agent records path, type, date, apparent authority, current-or-superseded status, what claims it supports, its limitations, and how to use it. The conflict log surfaces disagreements (old PDF vs current plan, mismatched stakeholder names, unsourced numbers) and recommends responses without resolving them silently. The missing-context list names absent decisions, unsourced numbers, and referenced-but-missing files. A duplicates report flags suspected duplicates, confidence, and version families so the agent never blends three versions of a plan or overweights a twice-exported transcript.

Caveats: the host is explicit that this is calibrated for serious, long-running knowledge work (e.g. 30-50 hour coding runs, reports, board docs), not casual chats where it is overkill, and not back-office data-pipeline operations. He also stresses this makes the work inspectable, not perfect, and that he would not attempt the workflow with models earlier than Opus 4.7 / GPT 5.5.

## Concepts surfaced

[[context-engineering]] · [[ai-hallucinations]] · [[ai-agents]] · [[agentic-workflows]]
