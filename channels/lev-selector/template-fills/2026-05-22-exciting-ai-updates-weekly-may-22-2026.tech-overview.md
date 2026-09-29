---
video_id: -NqSCfOB8yg
template_id: tech-overview
template_version: 1
source_summary: ../summaries/2026-05-22-exciting-ai-updates-weekly-may-22-2026.md
source_transcript: ../transcripts/2026-05-22-exciting-ai-updates-weekly-may-22-2026.md
source_summary_hash: sha256:48a95e747feaf76d3a3dc7d3896a54c7c4545fd3dc4f730d91320c84ff67754f
source_transcript_hash: sha256:0ffd628ea4bdf0eca87c0d9c36f94bfeae6ab18620b0e27ac180e7fbf8ef6563
fill_id: 14398167-c088-445b-92f5-433e99d0216f
published_at: '2026-05-31T01:05:42.553745'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Anthropic closed a $30B raise at a $900B valuation and hired Andrej Karpathy, while Google IO shipped Gemini 3.5 Flash and the cloud-hosted Gemini Spark personal agent.

## Tools covered

### M-Dash Harness
- **Vendor**: Microsoft
- **Category**: agent
- **Timestamp**: [00:02](https://www.youtube.com/watch?v=-NqSCfOB8yg&t=2)
- **Why It Matters**: A multimodel agentic scanning harness that topped the CyberGym cybersecurity benchmark using a generally available model, beating Anthropic's unreleased MAUS and showing the harness matters more than the model.
- **Sota Comparison**: Outperforms Anthropic's secretive proprietary MAUS model on CyberGym despite using an off-the-shelf base model.
- **Sota Band**: beats

### Qwen 3.7 Max Preview
- **Vendor**: Alibaba
- **Category**: agent
- **Timestamp**: [00:02](https://www.youtube.com/watch?v=-NqSCfOB8yg&t=2)
- **Why It Matters**: A strong, much cheaper Chinese model built for agentic multi-step jobs; it recently ran 35 hours non-stop with over a thousand tool calls fully autonomously, a current world record.
- **Sota Comparison**: Cheaper than American models with comparable agentic performance; 1M token context and 48 native languages.
- **Sota Band**: new

### Grok 4.3
- **Vendor**: xAI
- **Category**: reasoning
- **Timestamp**: [03:04](https://www.youtube.com/watch?v=-NqSCfOB8yg&t=184)
- **Why It Matters**: A reasoning model with fast and deep expert modes for long multifile context; the host subscribed, was disappointed, and unsubscribed, preferring Claude.
- **Sota Band**: behind
- **Access Constraint**: paid subscribers only

### Gemini Omni
- **Vendor**: Google
- **Category**: world-model
- **Timestamp**: [06:36](https://www.youtube.com/watch?v=-NqSCfOB8yg&t=396)
- **Why It Matters**: A family of world models announced at Google IO that can generate videos and games.
- **Sota Band**: new

### Gemini 3.5 Flash
- **Vendor**: Google
- **Category**: multimodal
- **Timestamp**: [06:51](https://www.youtube.com/watch?v=-NqSCfOB8yg&t=411)
- **Why It Matters**: Now the default Gemini model at roughly 300 tokens/second, matching or exceeding Gemini 3.1 Pro with a 1M token context, 64K output, and configurable thinking levels at low cost.
- **Sota Comparison**: Matches or exceeds the prior 3.1 Pro tier while being much cheaper than competing models.
- **Sota Band**: parity

### Gemini Spark
- **Vendor**: Google
- **Category**: agent
- **Timestamp**: [06:51](https://www.youtube.com/watch?v=-NqSCfOB8yg&t=411)
- **Why It Matters**: A personal agent running on Google Cloud with immediate access to your Google account, workspace, docs, and email, working 24/7 via an agentic harness and Anti-Gravity.
- **Sota Comparison**: Positioned as Google's answer to Open Claw, but cloud-hosted with built-in Google account access.
- **Sota Band**: new
- **Access Constraint**: requires paid Gemini subscription

### Anti-Gravity
- **Vendor**: Google
- **Category**: coding
- **Timestamp**: [06:51](https://www.youtube.com/watch?v=-NqSCfOB8yg&t=411)
- **Why It Matters**: Google's agent-first IDE, built after acquiring Windsurf, serving as the development interface for agentic coding workflows.
- **Sota Band**: new

### TML Interaction Small
- **Vendor**: Thinking Machines Lab
- **Category**: multimodal
- **Timestamp**: [10:07](https://www.youtube.com/watch?v=-NqSCfOB8yg&t=607)
- **Why It Matters**: A 276B-parameter mixture-of-experts full-duplex real-time interaction model from Mira Murati's lab that combines an interaction model and a reasoning model with no conversational delay.
- **Sota Band**: new
- **Access Constraint**: limited research preview soon

### Claude for Legal
- **Vendor**: Anthropic
- **Category**: tool
- **Timestamp**: [13:15](https://www.youtube.com/watch?v=-NqSCfOB8yg&t=795)
- **Why It Matters**: Adds 12 new practice-area plugins covering corporate, employment, privacy, IP, litigation, and governance, plus over 20 new MCP connectors for drafting and reviewing contracts.
- **Sota Band**: new

### Cray
- **Vendor**: Cray
- **Category**: image
- **Timestamp**: [16:12](https://www.youtube.com/watch?v=-NqSCfOB8yg&t=972)
- **Why It Matters**: A San Francisco startup generating high-fidelity visuals in under 15 seconds with mood boards, style references, a real-time canvas for live sketching, and a 22K resolution enhancer.
- **Sota Band**: new

### Hermes Agent
- **Vendor**: Hermes
- **Category**: agent
- **Timestamp**: [17:17](https://www.youtube.com/watch?v=-NqSCfOB8yg&t=1037)
- **Why It Matters**: An open agent at 163K GitHub stars and growing fast that self-improves between tasks by reviewing its history and creating or refining skills.
- **Sota Comparison**: Fewer stars than Open Claw's 374K but growing faster; both now self-improve via a dreaming feature.
- **Sota Band**: parity

### Open Claw
- **Vendor**: Open Claw
- **Category**: agent
- **Timestamp**: [17:17](https://www.youtube.com/watch?v=-NqSCfOB8yg&t=1037)
- **Why It Matters**: An open agent with 374K GitHub stars that now self-improves via a dreaming feature, comparable to Hermes; a three-person team ran ~100 autonomous agents on it consuming $1.3M in OpenAI credits in one month.
- **Sota Band**: parity

### Graphify
- **Vendor**: Graphify
- **Category**: tool
- **Timestamp**: [20:33](https://www.youtube.com/watch?v=-NqSCfOB8yg&t=1233)
- **Why It Matters**: Indexes local files and large code bases into interactive structured storage for RAG, cutting LLM token consumption by 70% while improving speed and accuracy, and generates HTML visualizations, Obsidian vaults, and MCP servers.
- **Sota Band**: new

### Gemini API File Search
- **Vendor**: Google
- **Category**: tool
- **Timestamp**: [20:33](https://www.youtube.com/watch?v=-NqSCfOB8yg&t=1233)
- **Why It Matters**: Provides cloud virtual storage where you upload files and ask questions about them, working as a multimodal RAG in the cloud.
- **Sota Band**: new

### Google AI Pointer
- **Vendor**: Google
- **Category**: tool
- **Timestamp**: [23:17](https://www.youtube.com/watch?v=-NqSCfOB8yg&t=1397)
- **Why It Matters**: Lets you point your mouse at on-screen elements and issue commands; it is aware of screen content and pointer location, so you can ask it to summarize or fix what you point to.
- **Sota Band**: new

### Zero Programming Language
- **Vendor**: Vercel Labs
- **Category**: coding
- **Timestamp**: [23:17](https://www.youtube.com/watch?v=-NqSCfOB8yg&t=1397)
- **Why It Matters**: A fast compiled mini-Rust-like language from Chris State that emits structured machine-readable JSON diagnostics with stable codes and fix plans, making it easier for AI agents to use and debug.
- **Sota Band**: new

### ChatGPT Personal Finance
- **Vendor**: OpenAI
- **Category**: tool
- **Timestamp**: [25:22](https://www.youtube.com/watch?v=-NqSCfOB8yg&t=1522)
- **Why It Matters**: Integrates with Plaid so ChatGPT can connect to your banks and generate financial analysis reports, dashboards, and advice, though it does not execute transactions.
- **Sota Band**: new

### MiniMax Mavis
- **Vendor**: MiniMax (Tencent)
- **Category**: agent
- **Timestamp**: [26:51](https://www.youtube.com/watch?v=-NqSCfOB8yg&t=1611)
- **Why It Matters**: A personal AI assistant now in beta for Windows and Android that operates 24/7, supports multiple LLMs, and uses leader, worker, and verifier agents with an adversarial worker-verifier loop to reduce hallucinations.
- **Sota Band**: new

### Recursive Intelligence
- **Vendor**: Recursive Intelligence
- **Category**: tool
- **Timestamp**: [29:45](https://www.youtube.com/watch?v=-NqSCfOB8yg&t=1785)
- **Why It Matters**: Founded by ex-Google Brain and Anthropic researchers with $335M in funding, it aims to make chip design up to 100,000 times faster to enable on-demand custom chips and a Cambrian explosion of specialized hardware.
- **Sota Band**: new



## Wider context

The week's through-line is that the agentic harness is now the differentiator, not the raw model: Microsoft's M-Dash beats Anthropic's secret MAUS, and Qwen 3.7 Max runs 35 hours unattended. As agents go continuous and token-hungry, the gating constraints shift to RAG without vector databases, sandbox isolation for autonomous agents, and faster custom silicon.

## Read next

[[retrieval-augmented-generation]] · [[ai-agents]] · [[agent-sandboxing]] · [[mixture-of-experts]] · [[world-models]] · [[model-quantization]]
