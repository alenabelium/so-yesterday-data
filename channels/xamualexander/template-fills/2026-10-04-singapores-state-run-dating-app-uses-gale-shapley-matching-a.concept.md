---
video_id: xTq0PpASM1A
template_id: concept
template_version: 1
source_summary: ../summaries/2026-10-04-singapores-state-run-dating-app-uses-gale-shapley-matching-a.md
source_transcript: ../transcripts/2026-10-04-singapores-state-run-dating-app-uses-gale-shapley-matching-a.md
source_summary_hash: sha256:cbded8b7a7020ff2b96c666a29cfaa479b9022f505d29056e642e4babdd89d07
source_transcript_hash: sha256:7a6c4c030ddb94d150a2378d95c69883c2ddc6b944441e32ade8c1c184e6a9e9
fill_id: 0fee7af9-4dce-42cf-a3dd-228e46d29f40
published_at: '2026-10-11T21:03:17.794879'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

Singapore's state-run dating app 'First Date' uses the Gale-Shapley stable marriage algorithm to match public servants. This algorithm guarantees a stable matching but is proposer-optimal, raising questions about fairness and real-world dating dynamics. The experiment tests whether mathematics can outperform for-profit dating apps.

## The argument

### Define the Core Substrate
- **Anchor Timestamps**: ['00:00:00']
- **Claim**: Singapore's 'First Date' app uses the Gale-Shapley stable marriage algorithm, which builds ranked preference lists, has proposers offer to top picks, receivers hold best offers, and repeats until a stable matching is reached where no two people prefer each other over their assigned match.
- **Role**: definition

### Proposer-Optimal Bias
- **Anchor Timestamps**: ['00:04:39']
- **Claim**: Gale-Shapley yields proposer-optimal outcomes: proposers get their best possible stable match, while receivers get their worst. This creates a strategic incentive to be a proposer, but the app's design doesn't clarify who fills that role, potentially undermining fairness.
- **Role**: evidence

### Matching vs. Clearing Problem
- **Anchor Timestamps**: ['00:25:18']
- **Claim**: A key objection is that dating problems are not matching problems but clearing problems: many people fail to meet the 'reserve price' of their desired partners. Even a perfect matching algorithm can't fix a market where transactions don't clear due to mismatched expectations.
- **Role**: counter

### Synthesis: Math vs. Market Incentives
- **Anchor Timestamps**: ['00:32:45']
- **Claim**: The Singapore experiment tests whether state-sponsored game theory can beat free-market dating apps. While the algorithm ensures stability, it doesn't address changing preferences or the clearing problem, and success will only be measurable over years or decades.
- **Role**: synthesis

## Evidence and caveats

The algorithm is already used for hospital residency matches and kidney exchanges, proving its real-world utility. However, the host notes that people's preferences change over time, and the algorithm only guarantees stability at a snapshot. The app is limited to public servants aged 21-35, which may skew results. The host also questions whether the proposer-receiver split is fair and whether the algorithm can scale to larger populations.

## Concepts surfaced

[[stable-marriage-problem]] · [[deferred-acceptance]] · [[matching-theory]] · [[perverse-incentives]] · [[clearing-problem]]
