---
title: "SIMPLE proof Lean can't self-verify itself (No Gödel's 2nd incompleteness theorem needed!)"
video_id: 07Ee9Z0B-zQ
date: 2026-08-21
url: https://www.youtube.com/watch?v=07Ee9Z0B-zQ
channel: Dr. Samuel Allen Alexander
tags:
  - llm-fundamentals
  - ai-safety
  - tutorials
transcript: ../transcripts/2026-08-21-simple-proof-lean-cant-self-verify-itself-no-godels-2nd-inco.md
relevant: true
knowledge: true
highlight: false
---

# SIMPLE proof Lean can't self-verify itself (No Gödel's 2nd incompleteness theorem needed!)

## Executive Summary

Dr. Samuel Allen Alexander presents a simple proof that the Lean theorem verifier cannot self-verify, avoiding Gödel's second incompleteness theorem. The proof uses computable ordinals, which are computer programs representing levels of infinity, to show a contradiction if Lean were to verify itself. The talk explains the naive fallacy, introduces computable ordinals with Python examples, and discusses why Gödel's theorem remains relevant for first-order logic systems.

## Key Points

- The naive proof that Lean cannot self-verify fails due to Tarski's undefinability of truth, but the idea is captured using computable ordinals. [00:02:37](https://www.youtube.com/watch?v=07Ee9Z0B-zQ&t=157)
- The corrected proof uses a function f that, given any algorithm enumerating computable ordinals, produces a larger ordinal, leading to a contradiction if Lean could verify itself. [00:04:01](https://www.youtube.com/watch?v=07Ee9Z0B-zQ&t=241)
- Computable ordinals are implemented as Python programs, with examples from 0 to omega^omega, illustrating the hierarchy and the complexity of higher ordinals. [00:09:51](https://www.youtube.com/watch?v=07Ee9Z0B-zQ&t=591)
