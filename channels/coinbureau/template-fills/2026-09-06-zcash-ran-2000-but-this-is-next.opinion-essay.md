---
video_id: IoNozEcWRDA
template_id: opinion-essay
template_version: 1
source_summary: ../summaries/2026-09-06-zcash-ran-2000-but-this-is-next.md
source_transcript: ../transcripts/2026-09-06-zcash-ran-2000-but-this-is-next.md
source_summary_hash: sha256:bca2511ba245a5d3aad9f09f9b7af23505de0996ca11a75330dd2811a9be68f1
source_transcript_hash: sha256:7f4f68cd1a09db3bb44c59c06005fb0f589aa966872aeace6891e57881065861
fill_id: cc6dc3bc-76aa-4a3c-9a0b-cb7f47b06f2b
published_at: '2026-10-13T07:47:21.837272'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## Thesis

Privacy for decisions, not just assets, is the underpriced half of the privacy trade, and Interfold's encrypted voting is the first practical step toward making it a core crypto infrastructure.

## Argument

The market has already repriced privacy for assets: Zcash is up over 1,900% in a year, shielded supply has jumped from 8% to over 30%, and Grayscale launched the first US spot privacy coin ETF. But that's only half the thesis. The other half is privacy for decisions, and it's still underpriced.

The problem is vote bribery. On a public blockchain, a visible vote can be proven, and a provable vote can be bought. Vitalik proposed MACI in 2019 to solve this with encrypted votes and receipt-freeness, but it had a fatal flaw: a single trusted coordinator held the decryption key. That coordinator could censor, be hacked, or be subpoenaed. MACI never escaped the lab.

Interfold, formerly Enclave, fixes that hole. Its Crisp protocol uses fully homomorphic encryption and threshold cryptography. FHE lets the system count votes without reading them—a ballot box that can tally but not peek. The decryption key is split across a committee of Cypher Nodes, so no single party can decrypt. The computation runs in a self-destructing encrypted execution environment, and zero-knowledge proofs verify eligibility without revealing the ballot. The result is a secret ballot that anyone can audit but nobody can read.

This isn't fully trustless—the committee is still a trusted party, just a distributed one. But it's a practical step toward the trustless system Vitalik described in his August blog post on local mixing. Vitalik's endorsement goes beyond words: he joined Interfold's token auction with 16 ETH.

The stakes are high. Token voting has failed publicly: DAO participation is below 10%,

## Counterpoints

- A committee holding the key is still a trusted party—just a bigger one. Interfold spreads trust across independent operators with collateral, but it's not fully trustless.
- There's no serious technical teardown of Interfold yet, and the absence of criticism isn't evidence of quality.
- Interfold might only be gaining traction because Vitalik endorsed it, not because the tech is proven.

## Concepts surfaced

[[fully-homomorphic-encryption]] · [[threshold-cryptography]] · [[zero-knowledge-proofs]] · [[dao-governance]] · [[encrypted-mempools]]
