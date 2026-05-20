---
video_id: DwvZ9f0RYzA
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-05-19-claude-code-just-changed-how-i-build-portfolio-websites-fore.md
source_transcript: ../transcripts/2026-05-19-claude-code-just-changed-how-i-build-portfolio-websites-fore.md
source_summary_hash: sha256:dec598af94861b62a6693670e3f6b3420fe29a9bc62c27cedca6be640d186f1d
source_transcript_hash: sha256:4ad3663f2b8835354810091e2ad3d78a6369b98e0c97908eb180537ebfc34a1a
fill_id: 722f1651-58e0-4f15-bcc3-a85ad0419547
published_at: '2026-05-20T08:49:53.790825'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Build a terminal-style portfolio with Claude Code, Next.js, and Hostinger CI/CD.

## Prerequisites

### GitHub Account
- **Kind**: account
- **Note**: Required to host the code repository for the tutorial project.

### Hostinger Account
- **Kind**: account
- **Note**: Required for hosting the deployed Next.js application.

### Node.js Environment
- **Kind**: tool
- **Note**: Needed to run npx create-next-app and manage dependencies.

## Steps

### Initialize Next.js Project
- **Timestamp**: [00:00](https://www.youtube.com/watch?v=DwvZ9f0RYzA&t=0)
- **Action**: Open a blank folder and run the command to create a new Next.js application in the current directory.
- **Command Or Clicks**: npx create-next-app@latest .

### Install Best Practices Skill
- **Timestamp**: [00:00](https://www.youtube.com/watch?v=DwvZ9f0RYzA&t=0)
- **Action**: Copy the command for the Next Best Practices skill, paste it into the terminal, select Cloud Code, and install the project table.
- **Command Or Clicks**: [Paste skill command] -> Select Cloud Code -> Press Enter -> Install

### Install Front-End Design Skill
- **Timestamp**: [00:00](https://www.youtube.com/watch?v=DwvZ9f0RYzA&t=0)
- **Action**: Install the front-end design skill to improve the UI experience of the generated code.
- **Command Or Clicks**: [Install Front-End Design Skill]

### Configure Research Prompt
- **Timestamp**: [01:31](https://www.youtube.com/watch?v=DwvZ9f0RYzA&t=91)
- **Action**: Create a resources/prompts folder, add a research prompt instructing the agent to build a terminal-style page using your LinkedIn, YouTube, and CV data.
- **Command Or Clicks**: mkdir -p resources/prompts

### Generate Initial UI
- **Timestamp**: [01:31](https://www.youtube.com/watch?v=DwvZ9f0RYzA&t=91)
- **Action**: Paste the research prompt into Claude Code, approve the implementation plan, and verify the UI accuracy and context window usage.
- **Command Or Clicks**: [Paste Prompt] -> Approve Plan

### Add Streaming Animations
- **Timestamp**: [02:25](https://www.youtube.com/watch?v=DwvZ9f0RYzA&t=145)
- **Action**: Paste the second prompt from the repository to add typing animations and simulated tool calls that stream in sequentially.
- **Command Or Clicks**: [Paste Animation Prompt]

### Implement Fake Chatbot
- **Timestamp**: [04:32](https://www.youtube.com/watch?v=DwvZ9f0RYzA&t=272)
- **Action**: Create a QA.json file with questions and answers, then use a regex-based prompt to simulate a chatbot interface without real inference.
- **Command Or Clicks**: [Create QA.json] -> [Paste Chat Prompt]

### Commit and Push to GitHub
- **Timestamp**: [05:39](https://www.youtube.com/watch?v=DwvZ9f0RYzA&t=339)
- **Action**: Create a commit named 'final', publish the branch, and name the repository 'portfolio website tutorial'.
- **Command Or Clicks**: git commit -m 'final' && git push

### Deploy via Hostinger
- **Timestamp**: [05:39](https://www.youtube.com/watch?v=DwvZ9f0RYzA&t=339)
- **Action**: Select Hostinger business plan, register a domain (or use temporary), and connect the GitHub repository for deployment.
- **Command Or Clicks**: Hostinger Dashboard -> Deploy Node.js App -> Connect GitHub Repo

### Verify CI/CD Deployment
- **Timestamp**: [08:18](https://www.youtube.com/watch?v=DwvZ9f0RYzA&t=498)
- **Action**: Make a code change (e.g., text color), push to GitHub, and verify that Hostinger automatically builds and deploys the update.
- **Command Or Clicks**: git push

## Gotchas

### Animations do not replay on page refresh to avoid forcing visitors to rewatch; use the 'new session' button to replay.
- **Severity**: heads_up
- **Timestamp**: [02:25](https://www.youtube.com/watch?v=DwvZ9f0RYzA&t=145)

### The chat feature is a fake QA.json regex match, not a real AI inference model.
- **Severity**: heads_up
- **Timestamp**: [04:32](https://www.youtube.com/watch?v=DwvZ9f0RYzA&t=272)

## Where to go next

Check the GitHub repo for free prompts and code. Hostinger offers a free domain with business plans; use code 'leonhosting' for 10% off.

## Concepts surfaced

[[claude-code]] · [[next-js]] · [[terminal-ui]] · [[hostinger-deployment]] · [[github-actions]] · [[fake-chatbot]]
