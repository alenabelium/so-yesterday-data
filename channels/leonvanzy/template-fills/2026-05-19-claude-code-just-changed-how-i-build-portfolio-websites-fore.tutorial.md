---
video_id: DwvZ9f0RYzA
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-05-19-claude-code-just-changed-how-i-build-portfolio-websites-fore.md
source_transcript: ../transcripts/2026-05-19-claude-code-just-changed-how-i-build-portfolio-websites-fore.md
source_summary_hash: sha256:dec598af94861b62a6693670e3f6b3420fe29a9bc62c27cedca6be640d186f1d
source_transcript_hash: sha256:4ad3663f2b8835354810091e2ad3d78a6369b98e0c97908eb180537ebfc34a1a
fill_id: 6654adea-91aa-47e3-9967-37bf7036788b
published_at: '2026-05-21T23:51:59.983331'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Build a terminal-style portfolio with streaming animations and deploy it automatically via GitHub and Hostinger.

## Prerequisites

### Node.js Environment
- **Kind**: tool
- **Note**: Required to run npx create-next-app and manage the Next.js project structure.

### GitHub Account
- **Kind**: account
- **Note**: Needed to host the source code and enable continuous integration with the hosting provider.

### Hostinger Account
- **Kind**: account
- **Note**: Required for hosting the Node.js application and managing domain connections.

## Steps

### Initialize Next.js project
- **Timestamp**: [00:00](https://www.youtube.com/watch?v=DwvZ9f0RYzA&t=0)
- **Action**: Create a new Next.js application in the current directory using the latest version.
- **Command Or Clicks**: npx create-next-app@latest .

### Install Next Best Practices skill
- **Timestamp**: [00:00](https://www.youtube.com/watch?v=DwvZ9f0RYzA&t=0)
- **Action**: Copy the installation command for the Next Best Practices skill, paste it into the terminal, and install it via the coding agent.
- **Command Or Clicks**: [Copy command] -> Paste in terminal -> Select Cloud Code -> Press Enter -> Install

### Install Front-end Design skill
- **Timestamp**: [00:00](https://www.youtube.com/watch?v=DwvZ9f0RYzA&t=0)
- **Action**: Install the front-end design skill to improve the UI experience.
- **Command Or Clicks**: [Install command for front-end design skill]

### Configure terminal UI prompt
- **Timestamp**: [01:31](https://www.youtube.com/watch?v=DwvZ9f0RYzA&t=91)
- **Action**: Create a resources/prompts folder, add a research/build prompt telling the agent to build a terminal-style page using your LinkedIn, YouTube, or CV data.
- **Command Or Clicks**: mkdir -p resources/prompts

### Generate initial portfolio content
- **Timestamp**: [01:31](https://www.youtube.com/watch?v=DwvZ9f0RYzA&t=91)
- **Action**: Paste the research prompt into Claude Code to generate the page content based on your provided resources.
- **Command Or Clicks**: Paste prompt into Claude Code

### Add streaming animations
- **Timestamp**: [02:25](https://www.youtube.com/watch?v=DwvZ9f0RYzA&t=145)
- **Action**: Use a second prompt to add streaming animations and simulated tool calls to the page.
- **Command Or Clicks**: Paste animation prompt into Claude Code

### Implement fake chatbot
- **Timestamp**: [04:32](https://www.youtube.com/watch?v=DwvZ9f0RYzA&t=272)
- **Action**: Create a QA.json file with questions and answers, then use a prompt to implement regex-based matching for a simulated chat window.
- **Command Or Clicks**: Create QA.json -> Paste chat prompt

### Commit and push to GitHub
- **Timestamp**: [05:39](https://www.youtube.com/watch?v=DwvZ9f0RYzA&t=339)
- **Action**: Commit the final code changes and push the repository to GitHub.
- **Command Or Clicks**: git commit -m 'final' && git push origin main

### Deploy via Hostinger
- **Timestamp**: [05:39](https://www.youtube.com/watch?v=DwvZ9f0RYzA&t=339)
- **Action**: Connect your GitHub repository to Hostinger's Node.js deployment service.
- **Command Or Clicks**: Hostinger Dashboard -> Deploy Node.js app -> Connect GitHub Repo

### Verify automatic deployment
- **Timestamp**: [08:18](https://www.youtube.com/watch?v=DwvZ9f0RYzA&t=498)
- **Action**: Make a code change, push to GitHub, and verify that Hostinger automatically rebuilds and updates the live site.
- **Command Or Clicks**: git push -> Check Hostinger deployment logs

## Gotchas

### Animations won't replay on refresh to avoid forcing visitors to rewatch; use the 'new session' button to replay.
- **Severity**: heads_up
- **Timestamp**: [02:25](https://www.youtube.com/watch?v=DwvZ9f0RYzA&t=145)

### The chat feature uses regex matching on a QA.json file, not real AI inference, so it is not a true chatbot.
- **Severity**: serious
- **Timestamp**: [04:32](https://www.youtube.com/watch?v=DwvZ9f0RYzA&t=272)

## Where to go next

Explore advanced Next.js configurations like environment variables in Hostinger or customize the regex patterns in QA.json for more complex portfolio interactions.

## Concepts surfaced

[[next-js]] · [[claude-code]] · [[github-actions]] · [[hostinger-deployment]] · [[terminal-ui-design]]
