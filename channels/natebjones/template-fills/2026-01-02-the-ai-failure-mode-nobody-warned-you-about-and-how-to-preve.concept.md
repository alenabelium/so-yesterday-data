---
video_id: T74uZgfu6mU
template_id: concept
template_version: 1
source_summary: ../summaries/2026-01-02-the-ai-failure-mode-nobody-warned-you-about-and-how-to-preve.md
source_transcript: ../transcripts/2026-01-02-the-ai-failure-mode-nobody-warned-you-about-and-how-to-preve.md
source_summary_hash: sha256:d8c679f5d66d06cb1f707b1f7ba12a97f5cb121d39ac04b920775d6b1fcb2b8e
source_transcript_hash: sha256:d995ec51d91342e1aa9169eec03b3c49889d8673b716f1399b9fa7ed16c5ef23
fill_id: 5c18e92d-bbd3-49d8-8a91-f39ca63226f4
published_at: '2026-10-20T01:36:15.757053'
key_points_suppressed: false
provenance: agent:template-fill-v1
---

## TL;DR

AI agents fail not by hallucinating but by confidently executing the wrong goal because they misread the user's intent. Intent is latent, not explicit in text, making it the core unsolved problem in agentic systems. Builders can mitigate this with disambiguation loops, externalized intent artifacts, and separating interpretation from execution.

## The argument

### The Failure Mode: Confident Misreading of Intent
- **Anchor Timestamps**: ['00:00:00']
- **Claim**: The agent's core failure is not hallucination but intent misalignment: it takes a fuzzy request, guesses a goal, commits, and executes confidently without checking back. This is the central problem of agentic systems, more fundamental than tool calling or orchestration.
- **Role**: definition

### Why Intent Is Latent, Not Explicit
- **Anchor Timestamps**: ['00:04:25']
- **Claim**: Context is explicit content (entities, constraints, facts), but intent is latent: priorities, tradeoffs, what 'done' looks like, what's risky, and what to do when instructions conflict. LLMs are trained for plausible continuations, not to infer these unspoken human priorities, creating a fundamental language mismatch.
- **Role**: definition

### Mitigation: Active Disambiguation Loops
- **Anchor Timestamps**: ['00:06:52']
- **Claim**: Treat clarification as a design problem: build systems that ask targeted questions to maximize information gain and narrow the solution space. This can be bolted onto prompts and agentic systems, forcing the model to surface assumptions and ask for clarification when intent is unclear.
- **Role**: evidence

### Mitigation: Externalize Intent as a Versioned Artifact
- **Anchor Timestamps**: ['00:09:22']
- **Claim**: Make intent a separate document—an 'intent commit'—that records goals, failure conditions, tradeoffs, and priorities. This turns intent into an interface and workflow problem, allowing updates and versioning independent of the prompt, and enabling inspection and testing before execution.
- **Role**: evidence

### Synthesis: Separate Interpretation from Execution
- **Anchor Timestamps**: ['00:14:06']
- **Claim**: The path forward is to architect systems that separate interpretation from execution, using eval suites with ambiguous prompts and disambiguation loops for destructive actions. This mirrors crypto's intent-based systems, where explicit intent representations and solver-checker mechanisms ensure high-fidelity execution.
- **Role**: synthesis

## Evidence and caveats

The speaker notes that LLMs are surprisingly practical for token generation, but intent remains unsolved. He cites the emergence of eval as a discipline and tools like LangChain/LangSmith and Google's ADK as progress, yet intent is still a bottleneck. He mentions that more context can sometimes make things worse due to 'lost in the middle' challenges. He also references Andre Karpathy's observation that humans learn from sparse examples better than models. The speaker cautions that disambiguation loops must be used selectively—asking questions at every step defeats the purpose of an agent. He also notes that crypto's intent-based systems are an imperfect analogy but a useful clue.

## Concepts surfaced

[[agentic-systems]] · [[llm-hallucination]] · [[prompt-engineering]] · [[evaluation-harnesses]] · [[reinforcement-learning]]
