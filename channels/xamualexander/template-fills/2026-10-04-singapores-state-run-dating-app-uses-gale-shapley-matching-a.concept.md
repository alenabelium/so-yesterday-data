---
video_id: xTq0PpASM1A
template_id: concept
template_version: 1
source_summary: ../summaries/2026-10-04-singapores-state-run-dating-app-uses-gale-shapley-matching-a.md
source_transcript: ../transcripts/2026-10-04-singapores-state-run-dating-app-uses-gale-shapley-matching-a.md
source_summary_hash: sha256:cbded8b7a7020ff2b96c666a29cfaa479b9022f505d29056e642e4babdd89d07
source_transcript_hash: sha256:7a6c4c030ddb94d150a2378d95c69883c2ddc6b944441e32ade8c1c184e6a9e9
fill_id: fe8a565e-f723-47d2-b5cf-705b522bf9c6
published_at: '2026-10-11T19:13:10.385664'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

Singapore's state-run dating app 'First Date' uses the Gale-Shapley stable marriage algorithm to match public servants. This algorithm guarantees a stable pairing where no two people prefer each other over their assigned matches. The app's design contrasts with for-profit dating apps, which have perverse incentives to keep users single.

## The argument

### Define the Core Algorithm
- **Anchor Timestamps**: ['00:00:00']
- **Claim**: Gale-Shapley, the 1962 stable marriage algorithm, matches participants by having proposers offer to their top pick, receivers hold the best offer and reject the rest, and rejected proposers move down their list until a stable matching is reached. This guarantees no two people prefer each other over their assigned matches.
- **Role**: definition

### Proposer-Optimal Bias
- **Anchor Timestamps**: ['00:05:51']
- **Claim**: Gale-Shapley yields proposer-optimal outcomes: proposers get their best possible stable match, while receivers get their worst. This raises the question of who gets to be the proposer, and whether the choice breaks the algorithm's balance.
- **Role**: evidence

### Counter: Matching vs. Clearing Problem
- **Anchor Timestamps**: ['00:25:18']
- **Claim**: A Hacker News commenter argues the dating market's problem is not a matching problem but a clearing problem: many people cannot meet the 'reserve price' of those they want to date. A more powerful matching algorithm won't fix this, just as a better car sales website won't help someone who can't afford a Ferrari.
- **Role**: counter

### Synthesis: State-Run vs. For-Profit Incentives
- **Anchor Timestamps**: ['00:04:39']
- **Claim**: For-profit dating apps have perverse incentives to keep users single, as matched users leave the platform. Singapore's app is designed to get users off the platform, aligning its success metric with user outcomes. This contrast highlights the potential of state-sponsored game theory to address societal issues.
- **Role**: synthesis

## Evidence and caveats

The algorithm is already used in hospital residency matches and kidney exchanges, and it won the 2012 Nobel Prize in Economics. The host notes that the algorithm runs in quadratic time, which is feasible for Singapore's small population but could be problematic for larger countries. He also acknowledges that the app's success will take years or decades to measure, and that preferences may change over time, which the algorithm does not address.

## Concepts surfaced

[[stable-marriage-problem]] · [[deferred-acceptance]] · [[matching-theory]] · [[perverse-incentives]] · [[clearing-problem]]
