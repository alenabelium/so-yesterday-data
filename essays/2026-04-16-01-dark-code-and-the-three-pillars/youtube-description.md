# Dark Code and the Three Pillars: A Framework for Code Nobody Reads

Production code that no human has ever understood is already running your favorite services. Here's how to manage it.

💥 Amazon's AI coding tool Kira caused a 13-hour AWS outage and broke the Amazon website — missing prices, failed deliveries, broken checkout. Between the incidents, Amazon fired 16,000 engineers. The code that broke everything was AI-generated, passed automated checks, and shipped without anyone understanding it. This is "dark code" — and every company shipping AI-generated code faces the same risk.

🏛️ The three pillars framework. Every system rests on Specification, Tests, and Code. The counterintuitive insight: any two pillars should reconstruct the third. Make code the LEAST important artifact — disposable, regeneratable. StrongDM produces 16,000 lines of Rust daily with two rules: "code must not be written by humans" and "code must not be reviewed by humans." RecursiveAI rebuilt 20,000 lines in three days from specs alone.

🔒 Five assurance levels and the trust problem. From vibe coding (Level 0) to formal mathematical verification (Level 4). When AI writes both code and tests, they share blind spots — Stanford calls this "circular validation." External holdout scenarios break the circle. The human role moves from code reviewer to specification architect and verification strategist.

📖 Read the full essay: https://so-yesterday.ai/essays/2026-04-16-01-dark-code-and-the-three-pillars

⏱️ Timestamps:
00:00 — Introduction: The Amazon Disaster
XX:XX — What Is Dark Code?
XX:XX — The Inversion: Code Is No Longer the Source of Truth
XX:XX — The Three Pillars: Spec + Tests + Code
XX:XX — Any Two Reconstruct the Third
XX:XX — Five Assurance Levels
XX:XX — The Trust Problem: Circular Validation
XX:XX — The Three Questions Every Team Should Ask

---

Based on the essay "Dark Code and the Three Pillars" from so-yesterday.ai — a curated knowledge base for AI transformation.

#AI #DarkCode #SoftwareEngineering #CodeQuality #AIAgents #SpecDriven #AICoding
