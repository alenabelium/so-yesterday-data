---
title: "Kevin Buzzard wrote a GREAT explainer of what "The proof is LEAN-verified" actually means"
video_id: cAjw7g54WWg
date: 2026-11-15
url: https://www.youtube.com/watch?v=cAjw7g54WWg
channel: Dr. Samuel Allen Alexander
tags:
  - ai-tools
  - coding
  - tutorials
  - opinion
transcript: ../transcripts/2026-11-15-kevin-buzzard-wrote-a-great-explainer-of-what-the-proof-is-l.md
relevant: true
knowledge: true
highlight: true
---

# Kevin Buzzard wrote a GREAT explainer of what "The proof is LEAN-verified" actually means

## Executive Summary

This video discusses Kevin Buzzard's blog post explaining what it means for a proof to be 'LEAN-verified,' especially in the context of AI-generated mathematics. The host outlines four critical questions to ask about any LEAN repository, emphasizing that verification is not automatic and requires careful checks. The video highlights potential issues in OpenAI's theorem dump, such as LEAN code not matching the paper's main theorem, and discusses the importance of sandboxing AI-generated code. The conclusion stresses that while LEAN verification is valuable, it requires additional work and scrutiny, particularly for AI-generated proofs.

## Key Points

- The four questions to ask about a LEAN repository: does the LEAN statement match the informal statement, does the code compile, does the code prove the theorem as stated, and does the code exploit a bug in LEAN's kernel? [00:03:10](https://www.youtube.com/watch?v=cAjw7g54WWg&t=190)
- Of the 290 OpenAI theorems with LEAN code, around 38 do not even state the main theorem of the paper, highlighting a potential gap between claims and formalizations. [00:08:18](https://www.youtube.com/watch?v=cAjw7g54WWg&t=498)
- Even if LEAN code passes all tests, the corresponding PDF proof may still be incorrect, as seen in the Navier-Stokes paper where the PDF and LEAN proofs diverge. [00:18:44](https://www.youtube.com/watch?v=cAjw7g54WWg&t=1124)
