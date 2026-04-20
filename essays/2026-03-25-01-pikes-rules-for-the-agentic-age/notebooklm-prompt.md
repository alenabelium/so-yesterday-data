Create an engaging video overview about how Rob Pike's five rules of programming from 1989 turn out to be the missing playbook for building reliable AI agent systems.

Focus on THREE main points:

1. **The five rules meet five real problems.** Rob Pike — co-creator of Unix and Go — wrote five programming rules in 1989 at Bell Labs: don't guess at bottlenecks, measure before you optimize, don't get fancy when n is small, simple is less buggy, and data dominates. Each rule maps precisely to a production problem in agentic engineering: context compression (data structure determines what survives), codebase instrumentation (teams swap models without baselines), linting agent output (agents are "lazy developers"), multi-agent coordination (teams build meshes before single agents work), and specification fatigue (stuffed context windows instead of clean data structures).

2. **2025 was the year of manufactured complexity.** Anthropic and OpenAI shipped transformative tools but their enterprise customers couldn't use them — the solutions were too complex. Both companies partnered with Accenture, BCG, and Deloitte to bridge the gap. Meanwhile, Nvidia took the opposite approach with Nemo Claw: trust developers to apply sound principles. The essay frames this as complexity-as-a-service versus simplicity-as-a-platform — and argues simplicity wins. Factory.ai's research consistently shows the agent isn't broken; the environment is.

3. **A practical five-phase framework.** The essay builds a concrete adoption framework: Phase 1 (Foundation) — audit your environment and fix linting, testing, and documentation before touching agents. Phase 2 (Simplicity) — one agent, one job, strict linting. Phase 3 (Measurement) — golden test sets, baseline before optimizing. Phase 4 (Data Structures) — invest in specifications and context hierarchies, not context dumps. Phase 5 (Scale) — add multi-agent coordination only when measurement demands it. Each phase has a key question practitioners should ask.

Tone: "Timeless wisdom meets cutting-edge tech." Intellectual but practical. The hook is the surprise: rules written for C programmers at Bell Labs in 1989 are the best guide for 2026 AI engineering. Make the viewer feel smart for appreciating old ideas applied in new ways. Reference the cheat sheet table at the end.

Target audience: Software engineers, engineering managers, and technical leaders building with AI agents who want a principled, no-hype approach to agentic engineering.
