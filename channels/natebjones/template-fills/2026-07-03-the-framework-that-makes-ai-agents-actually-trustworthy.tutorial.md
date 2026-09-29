---
video_id: U4TmrlWEY4M
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-07-03-the-framework-that-makes-ai-agents-actually-trustworthy.md
source_transcript: ../transcripts/2026-07-03-the-framework-that-makes-ai-agents-actually-trustworthy.md
source_summary_hash: sha256:9834faa3c12bca3cae9ce1a8873d6f7ba8b284157af15cfad76ec10fcac94b9b
source_transcript_hash: sha256:b74bebee61b0414a45615c2b95f99f0eb4dd7d46098cfa0ae25191bc603876fa
fill_id: 1238b9ec-001a-4ab8-a821-6f096a1eaf1b
published_at: '2026-09-29T11:06:43.489098'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Build a reusable agent skeleton that ingests, chunks, normalizes, and cites unstructured data to create trustworthy, high-stakes AI workflows.

## Prerequisites

### Local Storage
- **Kind**: hardware
- **Note**: Machine capable of running SQLite and storing local source files and records.

### Context Engineering
- **Kind**: knowledge
- **Note**: Understanding of how to define context packs, chunking, and normalization for unstructured data.

## Steps

### Define Context Pack for Email
- **Timestamp**: [04:33](https://www.youtube.com/watch?v=U4TmrlWEY4M&t=273)
- **Action**: Create a context pack that defines what the agent can read (thread, calendar constraints, people) with the goal to prepare a reply with a proposed calendar hold.
- **Command Or Clicks**: Define context pack: thread, calendar constraints, people. Goal: Prepare reply with proposed calendar hold.
- **Choice Branch**: Focus on low-stakes email scheduling to test the skeleton before high-stakes tasks.

### Ingest and Normalize Data
- **Timestamp**: [05:23](https://www.youtube.com/watch?v=U4TmrlWEY4M&t=323)
- **Action**: The agent ingests the thread, pulls out people and date ranges, and normalizes them (dates become dates, people become people) to draft a reply.
- **Command Or Clicks**: Ingest thread. Normalize dates and people. Draft reply.
- **Choice Branch**: Ensure normalization is accurate to make the agent useful for high-trust work.

### Enforce the Gate (No Submission)
- **Timestamp**: [05:23](https://www.youtube.com/watch?v=U4TmrlWEY4M&t=323)
- **Action**: The agent stops after drafting the reply and leaving a receipt of sources and changes. It does not send the email, requiring human approval.
- **Command Or Clicks**: Agent stops. Leaves draft, proposed hold, and receipt. No send action.
- **Choice Branch**: Critical: The agent must never submit, pay, or sign. Human must validate and send.

### Build Insurance Appeal Skeleton
- **Timestamp**: [06:52](https://www.youtube.com/watch?v=U4TmrlWEY4M&t=412)
- **Action**: Reuse the same skeleton for insurance appeals. Ingest denial letters and policy documents, chunking them into addressable pieces.
- **Command Or Clicks**: Ingest denial letter and policy docs. Chunk into tagged pieces.
- **Choice Branch**: Use real insurer policy language but synthetic patient data for the demo.

### Normalize and Store Locally
- **Timestamp**: [08:30](https://www.youtube.com/watch?v=U4TmrlWEY4M&t=510)
- **Action**: Normalize dates, amounts, and missing documents. Store everything locally in SQLite and a folder. No data leaves the machine.
- **Command Or Clicks**: Normalize data. Store in SQLite and local folder.
- **Choice Branch**: Ensure missing documents are flagged to avoid deadline surprises.

### Retrieve and Cite Policy
- **Timestamp**: [08:30](https://www.youtube.com/watch?v=U4TmrlWEY4M&t=510)
- **Action**: Retrieve specific policy sections cited in the denial. Perform a sanity check to see if the policy actually says what the letter implies.
- **Command Or Clicks**: Retrieve by structure: denial reason, policy section, sites, deadline. Sanity check citation.
- **Choice Branch**: Use citation maps to validate arguments rather than relying on vector similarity alone.

### Generate Case File and Stop
- **Timestamp**: [10:02](https://www.youtube.com/watch?v=U4TmrlWEY4M&t=602)
- **Action**: Produce a timeline, denial map, evidence checklist, and draft appeal letter. The agent stops and does not send the appeal.
- **Command Or Clicks**: Produce timeline, denial map, evidence checklist, draft appeal. Stop.
- **Choice Branch**: Human must review the citation map and send the appeal manually.

### Apply Skeleton to Taxes
- **Timestamp**: [11:26](https://www.youtube.com/watch?v=U4TmrlWEY4M&t=686)
- **Action**: Reuse the skeleton for tax prep. Ingest W2s, 1099s, receipts, and bank exports. Chunk into forms and normalize into a tax year ledger.
- **Command Or Clicks**: Ingest tax docs. Chunk into forms. Normalize to tax year ledger (date, vendor, amount, category).
- **Choice Branch**: Use the same agent structure; only the nouns and stakes change.

### Enforce Tax Guardrails
- **Timestamp**: [12:50](https://www.youtube.com/watch?v=U4TmrlWEY4M&t=770)
- **Action**: Apply citation guardrails: deductions must have evidence. Export a reviewable packet (income summary, expense ledger, deduction map) and stop.
- **Command Or Clicks**: Apply citation guardrails. Export packet. Stop.
- **Choice Branch**: Agent does not file taxes or email the CPA. It prepares the folder for human/expert review.

## Gotchas

### The agent is not allowed to submit, pay, or sign. It must stop and leave a receipt for human approval.
- **Severity**: blocking
- **Timestamp**: [03:43](https://www.youtube.com/watch?v=U4TmrlWEY4M&t=223)

### Do not send an agent-generated appeal unread. If it sends a bad appeal, you have two problems: the denial and the mess.
- **Severity**: serious
- **Timestamp**: [10:02](https://www.youtube.com/watch?v=U4TmrlWEY4M&t=602)

### Missing documents must be flagged explicitly. Gaps in evidence can affect what you can act on before deadlines.
- **Severity**: serious
- **Timestamp**: [08:30](https://www.youtube.com/watch?v=U4TmrlWEY4M&t=510)

## Where to go next

The Substack post contains runbooks for healthcare appeals and tax prep, plus context engineering guides. Next video covers putting every model at your fingertips, focusing on cheap open-source models for clean data.

## Concepts surfaced

[[agent-skeleton]] · [[context-engineering]] · [[trustworthy-ai]] · [[human-in-the-loop]] · [[data-normalization]] · [[open-source-ai]]
