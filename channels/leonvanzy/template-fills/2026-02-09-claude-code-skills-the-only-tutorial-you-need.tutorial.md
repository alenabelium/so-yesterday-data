---
video_id: vIUJ4Hd7be0
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-02-09-claude-code-skills-the-only-tutorial-you-need.md
source_transcript: ../transcripts/2026-02-09-claude-code-skills-the-only-tutorial-you-need.md
source_summary_hash: sha256:d62bc5a3c0e435dbb100cff0769a6962e7eb88b065c19705b630830df0a9bfc0
source_transcript_hash: sha256:be852d9383a56f490e1959bf934107c5911a099548e60cf52be5c1bc4a6f4b09
fill_id: 076465ed-e040-4481-b5db-c3c427da8654
published_at: '2026-10-19T21:56:21.216155'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Master Claude Code skills: find, install, and create custom skills to extend agent capabilities with minimal token usage.

## Prerequisites

### Claude Code
- **Kind**: tool
- **Note**: CLI tool for interacting with Claude, installed and available in your terminal.

### GitHub account
- **Kind**: account
- **Note**: Optional for browsing marketplaces, but not required for using skills.sh.

### Node.js
- **Kind**: tool
- **Note**: Required for running the Python scripts used in some skills, though not explicitly stated.

## Steps

### Install skills via the plugins marketplace
- **Timestamp**: [03:28](https://www.youtube.com/watch?v=vIUJ4Hd7be0&t=208)
- **Action**: Open Claude Code, navigate to the plugins menu, press right to access marketplaces, add the official Anthropic marketplace by pasting its GitHub URL, then select and install the desired skills.
- **Command Or Clicks**: In Claude Code: /plugin → right arrow → Add marketplace → paste GitHub URL → select skill → press I to install
- **Choice Branch**: Alternatively, use skills.sh for a simpler installation.

### Install skills from skills.sh
- **Timestamp**: [05:45](https://www.youtube.com/watch?v=vIUJ4Hd7be0&t=345)
- **Action**: Visit skills.sh, find a skill (e.g., front-end design), copy the provided command, paste it into your terminal, select your tools (Claude Code, Cursor), choose project or global level, and select symlink for installation.
- **Command Or Clicks**: Copy command from skills.sh → paste in terminal → select tools → choose project level → select symlink
- **Choice Branch**: Project level is recommended for team collaboration.

### Verify installed skills and token usage
- **Timestamp**: [08:18](https://www.youtube.com/watch?v=vIUJ4Hd7be0&t=498)
- **Action**: Open Claude Code, run the skills command to see all project skills, and run the context command to check token usage. Skills use minimal tokens because they are only loaded when needed.
- **Command Or Clicks**: /skills, /context
- **Choice Branch**: Restart Claude Code if skills are not visible.

### Use a skill to fix UI
- **Timestamp**: [10:30](https://www.youtube.com/watch?v=vIUJ4Hd7be0&t=630)
- **Action**: Ask Claude to use the front-end design skill to improve the UI, then use the browser use skill to verify changes. The agent loads the skill context only when needed.
- **Command Or Clicks**: Prompt: 'Please use your front-end design skill to fix up this user interface.'
- **Choice Branch**: Optionally nudge the agent to use a specific skill.

### Create a custom skill using the skill creator
- **Timestamp**: [12:55](https://www.youtube.com/watch?v=vIUJ4Hd7be0&t=775)
- **Action**: Install the skill creator skill from skills.sh, then provide Claude with a description and example code snippet for generating images with Nano Banana Pro. Specify defaults like 1K resolution and square aspect ratio, and instruct to store images in a specific folder.
- **Command Or Clicks**: Install skill creator: copy command from skills.sh → paste in terminal → select Claude Code → project level
- **Choice Branch**: Alternatively, copy documentation and ask Claude to create a skill.

### Handle API keys securely
- **Timestamp**: [16:24](https://www.youtube.com/watch?v=vIUJ4Hd7be0&t=984)
- **Action**: Create a .env file in the project root, add the Gemini API key as an environment variable, and ensure .env is excluded via .gitignore. Tell Claude the variable name so the skill script can read it.
- **Command Or Clicks**: Create .env file → add GEMINI_API_KEY=your_key → add .env to .gitignore
- **Choice Branch**: Never hardcode keys in skills or pass them directly to Claude.

### Test the image generation skill
- **Timestamp**: [18:46](https://www.youtube.com/watch?v=vIUJ4Hd7be0&t=1126)
- **Action**: Restart Claude Code, then ask it to generate an image using the skill. The agent will run the Python script and save the image to the specified folder.
- **Command Or Clicks**: Prompt: 'Please generate an image of a woman jogging next to the beach.'
- **Choice Branch**: Optionally use a free open-source model for local generation.

### Create an image optimizer skill
- **Timestamp**: [19:46](https://www.youtube.com/watch?v=vIUJ4Hd7be0&t=1186)
- **Action**: Ask Claude to create a new skill that optimizes images for the web: resize, convert to WebP, and move to a public folder. The skill will use a Python script.
- **Command Or Clicks**: Prompt: 'Please create a new skill... resize, convert to webp, move to public/assets.'
- **Choice Branch**: Restart Claude Code after creating the skill.

## Gotchas

### Never hardcode API keys in skills; use environment variables and exclude .env from git.
- **Severity**: blocking
- **Timestamp**: [16:24](https://www.youtube.com/watch?v=vIUJ4Hd7be0&t=984)

### Ensure .env is in .gitignore to avoid leaking secrets.
- **Severity**: serious
- **Timestamp**: [16:24](https://www.youtube.com/watch?v=vIUJ4Hd7be0&t=984)

### If skills are not visible, restart Claude Code.
- **Severity**: heads_up
- **Timestamp**: [08:18](https://www.youtube.com/watch?v=vIUJ4Hd7be0&t=498)

## Where to go next

Now that you've mastered skills, explore MCP servers for tool integration, or dive into advanced prompting techniques. Check out the linked video for more Claude Code tutorials.

## Concepts surfaced

[[claude-code]] · [[skills]] · [[mcp-servers]] · [[custom-commands]] · [[api-keys]] · [[image-generation]]
