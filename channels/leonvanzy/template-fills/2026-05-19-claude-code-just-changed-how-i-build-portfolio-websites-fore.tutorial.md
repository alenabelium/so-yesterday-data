---
video_id: DwvZ9f0RYzA
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-05-19-claude-code-just-changed-how-i-build-portfolio-websites-fore.md
source_transcript: ../transcripts/2026-05-19-claude-code-just-changed-how-i-build-portfolio-websites-fore.md
source_summary_hash: sha256:dec598af94861b62a6693670e3f6b3420fe29a9bc62c27cedca6be640d186f1d
source_transcript_hash: sha256:4ad3663f2b8835354810091e2ad3d78a6369b98e0c97908eb180537ebfc34a1a
fill_id: 65a69b56-ba83-4c21-b849-3b675afe1fd6
published_at: '2026-05-22T01:01:28.701260'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Build a terminal-style portfolio with Claude Code, Next.js, and deploy via Hostinger.

## Prerequisites

### GitHub Account
- **Kind**: account
- **Note**: Required to host the project repository for deployment.

### Hostinger Account
- **Kind**: account
- **Note**: Hosting provider used for deploying the Next.js application.

### Node.js Environment
- **Kind**: tool
- **Note**: Needed to run npx create-next-app and manage dependencies.

### Terminal Access
- **Kind**: tool
- **Note**: Command line interface to execute installation and deployment commands.

## Steps

### Initialize Next.js Project
- **Timestamp**: [00:25](https://www.youtube.com/watch?v=DwvZ9f0RYzA&t=25)
- **Action**: Open a blank folder and run the command to create a new Next.js application in the current directory.
- **Command Or Clicks**: npx create-next-app@latest .

### Install Best Practices Skill
- **Timestamp**: [00:45](https://www.youtube.com/watch?v=DwvZ9f0RYzA&t=45)
- **Action**: Copy the command for the Next Best Practices skill, paste it into the terminal, select Claude Code, press enter, and install the project table.
- **Command Or Clicks**: Copy skill command -> Paste in terminal -> Select Claude Code -> Enter -> Install

### Install Front-End Design Skill
- **Timestamp**: [00:55](https://www.youtube.com/watch?v=DwvZ9f0RYzA&t=55)
- **Action**: Install the front-end design skill to improve the UI experience.
- **Command Or Clicks**: Install front-end design skill

### Switch to Planning Mode
- **Timestamp**: [01:31](https://www.youtube.com/watch?v=DwvZ9f0RYzA&t=91)
- **Action**: Switch the coding agent to planning mode and paste the research and build prompt.
- **Command Or Clicks**: Switch to planning mode -> Paste prompt

### Provide Research Resources
- **Timestamp**: [01:45](https://www.youtube.com/watch?v=DwvZ9f0RYzA&t=105)
- **Action**: Create a resources folder with a prompts subfolder containing links to LinkedIn, YouTube, X, or a CV for the agent to research.
- **Command Or Clicks**: mkdir resources/prompts

### Approve Implementation Plan
- **Timestamp**: [02:25](https://www.youtube.com/watch?v=DwvZ9f0RYzA&t=145)
- **Action**: Approve the agent's implementation plan to generate the terminal-style UI.
- **Command Or Clicks**: Approve implementation plan

### Add Streaming Animations
- **Timestamp**: [03:15](https://www.youtube.com/watch?v=DwvZ9f0RYzA&t=195)
- **Action**: Paste the second prompt explaining how to add animations and mimic tool calls, then refresh the page.
- **Command Or Clicks**: Paste animation prompt -> Refresh page

### Set Up Chat Window
- **Timestamp**: [04:32](https://www.youtube.com/watch?v=DwvZ9f0RYzA&t=272)
- **Action**: Create a QA.json file with questions and answers, then use regex to match user input to answers for a simulated chatbot.
- **Command Or Clicks**: Create QA.json -> Paste chat prompt

### Commit and Push to GitHub
- **Timestamp**: [05:39](https://www.youtube.com/watch?v=DwvZ9f0RYzA&t=339)
- **Action**: Create a commit named 'final', publish the branch, and name the repository 'portfolio website tutorial'.
- **Command Or Clicks**: git commit -m 'final' -> git push origin main

### Deploy via Hostinger
- **Timestamp**: [06:10](https://www.youtube.com/watch?v=DwvZ9f0RYzA&t=370)
- **Action**: Select Hostinger business plan, register a domain, and connect the GitHub repository for deployment.
- **Command Or Clicks**: Select Business Plan -> Connect GitHub Repo -> Install/Authorize

### Verify Deployment and CI
- **Timestamp**: [07:27](https://www.youtube.com/watch?v=DwvZ9f0RYzA&t=447)
- **Action**: Test the live site, then make a code change, push to GitHub, and verify automatic deployment to Hostinger.
- **Command Or Clicks**: Push change -> Check Hostinger deployment log

## Gotchas

### Animations do not replay on refresh to avoid forcing visitors to rewatch; use 'new session' to replay.
- **Severity**: heads_up
- **Timestamp**: [03:45](https://www.youtube.com/watch?v=DwvZ9f0RYzA&t=225)

### The chat feature uses regex matching on QA.json, not real AI inference, so it is not an accurate chatbot.
- **Severity**: heads_up
- **Timestamp**: [04:45](https://www.youtube.com/watch?v=DwvZ9f0RYzA&t=285)

### Use a temporary domain first to test, then connect your registered domain later to avoid wasting a domain.
- **Severity**: serious
- **Timestamp**: [06:30](https://www.youtube.com/watch?v=DwvZ9f0RYzA&t=390)

## Where to go next

Check the GitHub repo for free prompts and code. Hostinger offers a 10% discount with code leonhosting. Explore environment variables for advanced Next.js apps.

## Concepts surfaced

[[claude-code]] · [[next-js]] · [[terminal-ui]] · [[hostinger-deployment]] · [[github-actions]] · [[regex-chatbot]]
