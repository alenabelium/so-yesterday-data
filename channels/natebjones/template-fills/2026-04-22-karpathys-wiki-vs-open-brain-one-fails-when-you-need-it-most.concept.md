---
video_id: dxq7WtWxi44
template_id: concept
template_version: 1
source_summary: ../summaries/2026-04-22-karpathys-wiki-vs-open-brain-one-fails-when-you-need-it-most.md
source_transcript: ../transcripts/2026-04-22-karpathys-wiki-vs-open-brain-one-fails-when-you-need-it-most.md
source_summary_hash: sha256:a8e8689ef31be9ab931f680af54bead1e5191231e326ba692343bc5325a4beb7
source_transcript_hash: sha256:3cb168bc85a459652a778301e2a701762040e9268c438787c2cd84a85702c467
fill_id: 837bfb88-b049-4f72-9d7f-5c6ca4c3f5ca
published_at: '2026-10-20T00:12:14.401877'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

AI memory systems split on when the AI does the hard thinking: at information ingest (write-time, like Karpathy's wiki) or at query time (like OpenBrain's structured database). The wiki compiles understanding into browsable notes, ideal for solo deep research but prone to error compounding and scale limits. OpenBrain stores facts faithfully and synthesizes on demand, scaling to teams and multi-agent workflows but lacking pre-built narratives. A hybrid graph layer can combine both strengths.

## The argument

### Define the Core Fork: Write-Time vs. Query-Time
- **Anchor Timestamps**: ['00:08:05']
- **Claim**: Every AI knowledge system must answer: when does the AI do the hard thinking? Karpathy's wiki is write-time: it synthesizes at ingest, compiling understanding into notes. OpenBrain is query-time: it stores facts faithfully and synthesizes fresh at query. This fork determines all downstream trade-offs.
- **Role**: definition

### Wiki Compiles, Database Reconstructs
- **Anchor Timestamps**: ['00:04:12']
- **Claim**: Karpathy's wiki compiles knowledge once and keeps it current, avoiding re-derivation on every query. OpenBrain reconstructs understanding from structured data each time, which is token-heavy but preserves detail. The wiki is like a tutor's study guide; OpenBrain is a filing cabinet with a librarian.
- **Role**: evidence

### Wiki Breaks at Scale and Drift
- **Anchor Timestamps**: ['00:23:03']
- **Claim**: The wiki approach breaks at scale: multi-agent writes conflict, and neglected wikis drift into confident misinformation because old syntheses read well but become wrong. Karpathy's own design works best at 100–10,000 documents, not corporate scale. OpenBrain's staleness looks like ignorance, not active misinformation.
- **Role**: counter

### Hybrid: Graph Layer Over Structured Data
- **Anchor Timestamps**: ['00:30:38']
- **Claim**: The hybrid model keeps OpenBrain as the authoritative store and adds a graph plugin that generates wiki-style pages on demand. This compilation agent reads structured data, synthesizes topic summaries, and produces browsable pages without editing the database directly, preventing error compounding and enabling scale.
- **Role**: synthesis

## Evidence and caveats

Karpathy's wiki wins for solo deep research: reading 10 papers over weeks, contradictions flagged at ingest, cross-references built automatically. OpenBrain wins for precise queries (e.g., 'every meeting note from Q1 where pricing was discussed'), multi-agent access, and volume beyond 10,000 entries. Caveats: the wiki's editorial decisions can drop nuance; most users won't maintain raw-source discipline. OpenBrain's deep synthesis can be unpredictable without a prior map, and it lacks browsability—though plugins (Obsidian, contradiction audits) address this. The hybrid graph layer is new and requires disciplined data input to compound.

## Concepts surfaced

[[karpathy-wiki]] · [[openbrain]] · [[context-layer]] · [[ai-memory]] · [[multi-agent-systems]] · [[knowledge-graph]]
