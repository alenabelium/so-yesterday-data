---
video_id: VFLieg8JjLA
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-04-18-claude-code-build-an-ai-agent-that-finds-vulnerabilities.md
source_transcript: ../transcripts/2026-04-18-claude-code-build-an-ai-agent-that-finds-vulnerabilities.md
source_summary_hash: sha256:5cb5d0a197b0bcd7801851fac7657e4ed6ba6b83d00c8eed50a8476f9be87e39
source_transcript_hash: sha256:d292f0dfd05790b5a59e9649aec36e7a313445943c00ff64cd74d96d6beafff7
fill_id: 71db3e87-c1cf-4f58-979a-bfc4bc094cbb
published_at: '2026-05-18T07:15:55.657125'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Build a reusable Claude Code skill and sub-agent to automatically audit codebases for OWASP Top 10 vulnerabilities.

## Prerequisites

### Claude Code
- **Kind**: tool
- **Note**: The primary coding agent used to create skills and sub-agents.

### GitHub CLI
- **Kind**: tool
- **Note**: Required if starting with a blank project to clone repositories locally.

### OWASP Top 10 Knowledge
- **Kind**: knowledge
- **Note**: Understanding of the standard awareness document for critical web application security risks.

## Steps

### Install the Skill Creator Skill
- **Timestamp**: [03:18](https://www.youtube.com/watch?v=VFLieg8JjLA&t=198)
- **Action**: Install the skill creator tool into the project folder to enable skill generation capabilities.
- **Command Or Clicks**: Run the command copied from skills.sage at the project level.
- **Choice Branch**: Install at project level to keep the skill local to this workspace.

### Create the Security Skill via Voice
- **Timestamp**: [04:10](https://www.youtube.com/watch?v=VFLieg8JjLA&t=250)
- **Action**: Boot Claude Code with the Opus 4.7 model and use the skill creator to dictate instructions for a security vulnerability skill that handles both existing projects and new GitHub repos.
- **Command Or Clicks**: Trust folder, select Opus 4.7, invoke skill creator, dictate requirements.
- **Choice Branch**: Use voice dictation for the skill definition to speed up the process.

### Configure OWASP References
- **Timestamp**: [05:43](https://www.youtube.com/watch?v=VFLieg8JjLA&t=343)
- **Action**: Instruct the agent to extract OWASP Top 10 items into separate reference documents within a subfolder, rather than embedding them in skills.md, to keep the main file clean.
- **Command Or Clicks**: Copy OWASP Top 10 article, paste into prompt, request extraction to reference folder.
- **Choice Branch**: Ensure the agent creates separate markdown files for each vulnerability type.

### Define Audit Output Structure
- **Timestamp**: [06:56](https://www.youtube.com/watch?v=VFLieg8JjLA&t=416)
- **Action**: Specify that the skill must store the final audit report in a date-stamped folder named /audit/.
- **Command Or Clicks**: Dictate: 'Store the report in a folder called /audit/ and let's just do date or current date.'
- **Choice Branch**: None.

### Verify Skill Structure
- **Timestamp**: [08:11](https://www.youtube.com/watch?v=VFLieg8JjLA&t=491)
- **Action**: Confirm with the agent that the skill.md file contains only execution flow and references, while the detailed vulnerability data is in the references subfolder.
- **Command Or Clicks**: Ask agent to verify separation of concerns between skills.md and reference docs.
- **Choice Branch**: None.

### Create the Sub-Agent
- **Timestamp**: [09:16](https://www.youtube.com/watch?v=VFLieg8JjLA&t=556)
- **Action**: Create a new sub-agent named 'security scanner' that references the security scanner skill, has access to all tools, uses Opus, and is scoped to the project.
- **Command Or Clicks**: Create new agent, name 'security scanner', reference skill, grant tool access, select Opus, set color to red.
- **Choice Branch**: Scope the agent to the current project.

### Execute the Security Audit
- **Timestamp**: [10:11](https://www.youtube.com/watch?v=VFLieg8JjLA&t=611)
- **Action**: Spin up a new Claude Code session, verify the skill and agent are visible, and instruct the agent to perform a security audit on the application.
- **Command Or Clicks**: Navigate to skills/agents, invoke 'Please perform a security audit on this application.'
- **Choice Branch**: Use the sub-agent directly or invoke the skill from the main agent.

## Gotchas

### Do not add all OWASP Top 10 content into the single skills.md file; keep it as a reference to separate documents.
- **Severity**: serious
- **Timestamp**: [08:11](https://www.youtube.com/watch?v=VFLieg8JjLA&t=491)

### Remove the solution file from the project folder before scanning to prevent the agent from cheating.
- **Severity**: blocking
- **Timestamp**: [02:11](https://www.youtube.com/watch?v=VFLieg8JjLA&t=131)

## Where to go next

Explore the agentic coding masterclass for fundamentals on agents and LLMs, including interactive tokenizer presentations.

## Concepts surfaced

[[claude-code-skills]] · [[sub-agent-architecture]] · [[owasp-top-10]] · [[ai-security-scanning]] · [[agentic-workflows]]
