---
title: "Pike's Rules for the Agentic Age: Why 1989 Programming Wisdom Is Your Best AI Strategy"
date: "2026-03-25"
description: "Rob Pike's five rules of programming — written in 1989 — turn out to be the missing playbook for building reliable AI agent systems. A practical framework for applying timeless engineering principles to the agentic era."
slug: "2026-03-25-01-pikes-rules-for-the-agentic-age"
video: "9XdTBnu3vFI"
---

# Pike's Rules for the Agentic Age: Why 1989 Programming Wisdom Is Your Best AI Strategy

> *This essay is based on Nate Jones's video ["Your Engineers Can Build What Accenture Charges You Millions For"](https://www.youtube.com/watch?v=7AO4w4Y_L24) (March 24, 2026). Full credit to Nate for the original analysis connecting Rob Pike's rules to modern agentic engineering challenges. The framework below extends his insights into a practical guide for teams building with AI agents.*

---

In 1989, Rob Pike — co-creator of Unix and Go, and one of the most influential systems programmers alive — wrote down [five rules of programming](https://www.lysator.liu.se/c/pikestyle.html) in his "Notes on Programming in C." They were meant for Bell Labs engineers writing C code on terminals. Thirty-seven years later, they might be the most important thing you read about AI agents.

That's the thesis Nate Jones laid out in his recent video, and it's one worth taking seriously. Because while the AI industry spent 2025 selling complexity — multi-agent meshes, elaborate orchestration frameworks, consultant-driven "transformation paradigms" — the teams actually shipping reliable agent systems kept rediscovering the same thing: the old rules still work. They just need to be read with fresh eyes.

---

## The Five Rules, Then and Now

Pike's rules are taught in computer science programs. Senior engineers pass them to juniors. They're carved into the discipline's bedrock. Here they are, verbatim:

<!--
┌─────────────────────────────────────────────────────────────────────┐
│                   ROB PIKE'S FIVE RULES (1989)                      │
├─────┬───────────────────────────────────────────────────────────────┤
│  1  │ You can't tell where a program is going to spend its time.    │
│     │ Bottlenecks occur in surprising places. Don't put in a speed  │
│     │ hack until you've proven that's where the bottleneck is.      │
├─────┼───────────────────────────────────────────────────────────────┤
│  2  │ Measure. Don't tune for speed until you've measured, and      │
│     │ even then don't unless one part overwhelms the rest.          │
├─────┼───────────────────────────────────────────────────────────────┤
│  3  │ Fancy algorithms are slow when n is small, and n is usually   │
│     │ small. Don't get fancy.                                       │
├─────┼───────────────────────────────────────────────────────────────┤
│  4  │ Fancy algorithms are buggier than simple ones and harder to   │
│     │ implement. Use simple algorithms as well as simple data        │
│     │ structures.                                                    │
├─────┼───────────────────────────────────────────────────────────────┤
│  5  │ Data dominates. If you've chosen the right data structures    │
│     │ and organized things well, the algorithms will almost always   │
│     │ be self-evident.                                               │
└─────┴───────────────────────────────────────────────────────────────┘
-->

What makes these rules so durable is that they're not about C, or Unix, or any particular technology. They're about how complexity behaves in real systems. And that's exactly the problem AI agent builders are drowning in right now.

---

## Why 2025 Was the Year of Manufactured Complexity

As Jones documents, both Anthropic and OpenAI spent 2025 learning a painful lesson: their enterprise customers couldn't actually use what they shipped. Claude Code and Codex were transformative internally — Anthropic ships features seemingly every eight hours — but external engineering teams couldn't replicate those results. The solutions were too complex to adopt.

The response? Partner with big consulting firms — Accenture, BCG, Deloitte, PwC — to bridge the gap. OpenAI and Anthropic effectively outsourced their change management because the complexity they'd created required an entire services layer to explain.

Meanwhile, Nvidia took a different approach with Nemo Claw. Instead of adding consulting intermediaries, Jensen Huang walked onstage and essentially said: *you developers are smart. You can figure this out.* Nemo Claw wraps OpenClaw in enterprise-grade security — YAML-based policy guardrails, model constraints, local-first compute — but trusts engineers to apply sound principles to build with it.

The difference isn't just corporate strategy. It's a philosophical bet: complexity-as-a-service versus simplicity-as-a-platform.

---

## Pike's Rules Applied: Five Hard Problems in Agent Engineering

Jones identifies five production challenges in agent deployment. Each one maps directly to Pike's principles. Here's how:

### Problem 1: Context Compression → Pike's Rule 5 (Data Dominates)

Long-running agent sessions fill up context windows — even million-token ones. Every compression strategy is lossy. Factory.ai tested three approaches: their own anchored iterative summarization (incremental, structured), OpenAI's compact endpoint (opaque, highly compressed), and Anthropic's SDK compression (detailed but regenerates fully each cycle).

Factory's incremental approach scored highest because it enforces data structure: explicit sections for session intent, file modifications, decisions, and next steps. The structure forces preservation. You can't silently drop critical context when the format demands it.

**Pike's insight:** Get the data structures right, and the algorithm becomes self-evident. In context compression, that means structuring your session state so that compression *has* to preserve what matters — not hoping a black-box algorithm figures it out.

### Problem 2: Codebase Instrumentation → Pike's Rule 2 (Measure)

"Don't tune for speed until you've measured" is decades old. It's also the single biggest gap in most agent deployments.

Teams complain about poor LLM responses without ever establishing a baseline. They swap models, rewrite prompts, add complexity — all without measuring what "good" looks like. Factory.ai's agent readiness framework evaluates codebases across eight pillars — style and validation, build systems, testing, documentation, dev environment, code quality, observability, and security — and consistently finds the same thing: the agent isn't broken. The environment is.

**Pike's insight:** Measure before you optimize. Establish baselines. Build golden test sets. Know what latency looks like, what a good response set looks like. Then — and only then — tune.

### Problem 3: Linting and Code Quality → Pike's Rule 4 (Simple Is Less Buggy)

Agents are, as Jones puts it, "lazy developers that are happy to throw it off their plates." Without strict linting — enforced style, consistency checks, static analysis — agent-generated code drifts toward entropy.

This isn't an AI problem. It's a software hygiene problem that gets amplified when the code producer doesn't care about craft. Factory.ai documents obsessive linting rules that essentially put code in a straitjacket: it *must* adhere to best practices at all times.

**Pike's insight:** Fancy algorithms are buggier. Simple structures are easier to debug. In the agentic context, strict linting *is* the simplicity constraint — it prevents agents from generating complex, unmaintainable code that humans can't review effectively.

### Problem 4: Multi-Agent Coordination → Pike's Rule 1 & 3 (Don't Optimize Prematurely)

The industry is converging on planner-executor patterns for multi-agent work. It's simple. It works. And yet teams regularly try to over-engineer it — building elaborate agent meshes before they can even measure whether a single agent does the job.

**Pike's insight:** Don't get fancy until you've proven you need to. Build the simplest possible agentic pipeline. Add complexity only when measurement proves it's necessary. Your n is usually small.

### Problem 5: Specification Fatigue → Pike's Rule 5 (Data Dominates, Again)

The hardest problem. Teams struggle to define specs clearly upfront. They stuff everything into context windows instead of building clean context graphs. They take shortcuts on requirements because writing precise specifications is hard, tedious work.

But this is exactly Pike's Rule 5 in disguise: if your data structures (specifications, context hierarchies, documentation) are well-organized, the agent's behavior becomes self-evident. If they're not, no amount of prompt engineering saves you.

**Pike's insight:** Write dumb code, have smart objects. In agentic terms: write simple agents, have smart specifications.

---

## The Framework: Pike's Rules for AI Practitioners

Here's a practical framework for applying these timeless principles to your AI agent work — whether you're an engineer, a product manager, or someone "coding under the desk" at a non-technical company.

<!--
┌─────────────────────────────────────────────────────────────────────────────┐
│          THE PIKE FRAMEWORK FOR AGENTIC ENGINEERING                         │
│          ─────────────────────────────────────────────                       │
│                                                                             │
│  PHASE 1: FOUNDATION                                                        │
│  ┌────────────────────────────────────────────────────────────────────┐     │
│  │  ✦ Audit your environment before touching agents                   │     │
│  │  ✦ Fix linting, testing, documentation, and build systems FIRST   │     │
│  │  ✦ Create an agents.md or CLAUDE.md that describes your codebase   │     │
│  │  ✦ Establish baselines: what does "good output" look like?        │     │
│  └────────────────────────────────────────────────────────────────────┘     │
│                              ↓                                              │
│  PHASE 2: SIMPLICITY                                                        │
│  ┌────────────────────────────────────────────────────────────────────┐     │
│  │  ✦ Start with ONE agent doing ONE job                              │     │
│  │  ✦ Use planner → executor pattern only when needed                │     │
│  │  ✦ Resist the urge to build multi-agent meshes                    │     │
│  │  ✦ Enforce strict linting on all agent-generated code             │     │
│  └────────────────────────────────────────────────────────────────────┘     │
│                              ↓                                              │
│  PHASE 3: MEASUREMENT                                                       │
│  ┌────────────────────────────────────────────────────────────────────┐     │
│  │  ✦ Build golden test sets for evaluating agent output              │     │
│  │  ✦ Measure latency, accuracy, and cost per task                   │     │
│  │  ✦ Only optimize the part that overwhelms the rest                │     │
│  │  ✦ Profile before you assume — bottlenecks are never obvious      │     │
│  └────────────────────────────────────────────────────────────────────┘     │
│                              ↓                                              │
│  PHASE 4: DATA STRUCTURES                                                   │
│  ┌────────────────────────────────────────────────────────────────────┐     │
│  │  ✦ Invest in specifications — they are your highest-leverage work │     │
│  │  ✦ Build context hierarchies, not context dumps                   │     │
│  │  ✦ Use structured compression (milestones, summaries, sections)   │     │
│  │  ✦ Design for agent navigation: clean graphs > stuffed windows    │     │
│  └────────────────────────────────────────────────────────────────────┘     │
│                              ↓                                              │
│  PHASE 5: SCALE (only when proven necessary)                                │
│  ┌────────────────────────────────────────────────────────────────────┐     │
│  │  ✦ Add multi-agent coordination AFTER single-agent limits are hit │     │
│  │  ✦ Use milestone-based agent handoffs for long tasks              │     │
│  │  ✦ Let agents die and refresh context rather than stuffing windows│     │
│  │  ✦ Complexify only what measurement tells you to complexify       │     │
│  └────────────────────────────────────────────────────────────────────┘     │
└─────────────────────────────────────────────────────────────────────────────┘
-->

### Phase 1: Foundation — Fix the Environment, Not the Agent

Before you write a single prompt, audit your codebase environment. Factory.ai's data consistently shows that the agent isn't the broken thing — the environment is. Fix your linting configs, document your builds, set up dev containers, create an `agents.md` or `CLAUDE.md` file. Establish what "good" looks like before you start measuring against it.

**Key question:** *If a new human engineer joined tomorrow, could they ship on day one? If not, your agent can't either.*

### Phase 2: Simplicity — One Agent, One Job

Start with a single agent handling a single well-defined task. Use a planner-executor pattern only when a single agent genuinely can't handle the scope. Resist every urge to build elaborate multi-agent orchestration. Enforce strict linting on everything the agent produces.

**Key question:** *Can I explain what this agent does in one sentence? If not, it's too complex.*

### Phase 3: Measurement — Baseline Before You Optimize

Build golden test sets. Measure latency, accuracy, and cost per task. When someone says "the LLM responses aren't good," ask: compared to what? Only optimize the component that measurably overwhelms the rest. This is Pike's Rule 2 applied directly.

**Key question:** *Do I have a number, or do I have a feeling?*

### Phase 4: Data Structures — Specifications Are Your Highest-Leverage Work

This is Pike's Rule 5 — the most important one. Invest heavily in specifications, context hierarchies, and structured documentation. Build context graphs that agents can navigate cleanly, rather than stuffing everything into a prompt and hoping. Use structured compression that preserves milestones, decisions, and next steps.

**Key question:** *If I look at my data structures alone, is the agent's behavior self-evident?*

### Phase 5: Scale — Only When Measurement Demands It

Add multi-agent coordination only after you've hit proven single-agent limits. Use milestone-based handoffs for long-running tasks — let agents complete a phase, save structured state, and hand off to a fresh agent with a clean context window. Complexify only what your measurements tell you to complexify.

**Key question:** *Have I measured a bottleneck, or am I guessing where the complexity needs to go?*

---

## The Quick-Reference Cheat Sheet

| Pike's Rule (1989) | Agentic Translation (2026) | Common Mistake |
|---|---|---|
| **1. Bottlenecks surprise you** | Profile agent systems before optimizing | Rewriting prompts without data on what's actually failing |
| **2. Measure first** | Baseline agent performance with golden test sets | Swapping models or adding agents based on vibes |
| **3. Don't get fancy** | Start with one agent, one task | Building multi-agent meshes before single agents work |
| **4. Simple is less buggy** | Enforce strict linting on agent output | Letting agents generate complex, unreviewed code |
| **5. Data dominates** | Invest in specs, context graphs, and structured environments | Stuffing context windows instead of organizing information |

---

## The Deeper Lesson: Hype Cycles Forget, Principles Don't

Jones makes a point worth sitting with: every hype cycle — cloud, mobile, AI — makes us forget the fundamentals. We think everything is new. We rebrand old practices with new jargon. Consultants sell this novelty because complexity drums up business.

But the engineering teams that actually ship — at Nvidia building close to the metal, at Factory.ai obsessing over linting rules, at the companies where agents are genuinely productive — they all converge on the same ancient wisdom. Keep it simple. Measure before you optimize. Get your data structures right. Let the algorithms follow.

Fred Brooks said it in 1975 in *The Mythical Man-Month*: "Show me your tables, and I won't usually need your flowcharts; they'll be obvious." Pike restated it in 1989. And in 2026, as we hand more and more autonomy to AI agents, it's truer than ever.

The agent isn't the hard part. The environment, the specifications, the data structures — that's where the real work is. And it always has been.

You don't need Accenture to tell you that. Pike already did.

---

*Based on: ["Your Engineers Can Build What Accenture Charges You Millions For"](https://www.youtube.com/watch?v=7AO4w4Y_L24) by Nate Jones (March 24, 2026). Additional references: Rob Pike, ["Notes on Programming in C"](https://www.lysator.liu.se/c/pikestyle.html) (1989); Fred Brooks, "The Mythical Man-Month" (1975); Brian W. Kernighan & Rob Pike, "The Practice of Programming" (1999); [Factory.ai](https://www.factory.ai/) agent readiness research.*
