---
video_id: a4p6ykdRmzc
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-06-02-every-landing-page-needs-this-claude-code-higgsfield-setup.md
source_transcript: ../transcripts/2026-06-02-every-landing-page-needs-this-claude-code-higgsfield-setup.md
source_summary_hash: sha256:d36b3dd944803d4270ea7110e36efaf3d90a3383d659157dbf8923a5e6b9bd5f
source_transcript_hash: sha256:6fb960b0d262e376e36b34043e755969d737e90a937f35d44234d3ee21e248e7
fill_id: 51d60326-5ba8-4fa0-bfe3-ce2a7525aeb9
published_at: '2026-06-02T22:45:30.892980'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Use Claude Code and Higgsfield AI to generate, animate, and integrate a custom robot avatar into a static landing page.

## Prerequisites

### Higgsfield Account
- **Kind**: account
- **Note**: Required for CLI authentication and video generation credits.

### Node.js Environment
- **Kind**: tool
- **Note**: Needed to run npm install and npm run dev for the starter project.

### Starter Repo
- **Kind**: tool
- **Note**: Download the provided GitHub repo to follow along with the setup.

## Steps

### Install starter project
- **Timestamp**: [00:47](https://www.youtube.com/watch?v=a4p6ykdRmzc&t=47)
- **Action**: Download the repo, install dependencies, and start the dev server.
- **Command Or Clicks**: npm install && npm run dev

### Install Higgsfield skill
- **Timestamp**: [01:56](https://www.youtube.com/watch?v=a4p6ykdRmzc&t=116)
- **Action**: Install the Higgsfield generate skill via Claude Code's skill installer.
- **Command Or Clicks**: Copy add skill command -> Terminal: [paste] -> Select Higgsfield generate skill -> Select Sim link
- **Choice Branch**: Use CLI tool as recommended for Claude Code users.

### Authenticate with Higgsfield
- **Timestamp**: [03:06](https://www.youtube.com/watch?v=a4p6ykdRmzc&t=186)
- **Action**: Ask Claude for auth instructions, copy the command, and run it to connect.
- **Command Or Clicks**: Ask Claude: 'How do I authenticate using the CLI?' -> Copy command -> Terminal: [paste]

### Generate avatar image
- **Timestamp**: [03:06](https://www.youtube.com/watch?v=a4p6ykdRmzc&t=186)
- **Action**: Prompt Claude to generate four robot avatar variations with specific constraints.
- **Command Or Clicks**: Prompt: 'Use Higgsfield to generate four variations of a friendly robot avatar... Use GPT Image 2... Save in public folder.'
- **Choice Branch**: Select GPT Image 2 or other models like Nano Banana.

### Integrate avatar to page
- **Timestamp**: [04:06](https://www.youtube.com/watch?v=a4p6ykdRmzc&t=246)
- **Action**: Ask Claude to add the avatar to the hero section with specific layout and styling.
- **Command Or Clicks**: Prompt: 'Add this avatar image to the hero section... Split hero text left, avatar right... White theme frame.'

### Animate avatar with video
- **Timestamp**: [05:27](https://www.youtube.com/watch?v=a4p6ykdRmzc&t=327)
- **Action**: Generate a subtle idle animation using Sea Dance 2 and save as video.
- **Command Or Clicks**: Prompt: 'Use Higgsfield to animate... with Sea Dance 2... 5-second idle animation... Save as video in public folder.'
- **Choice Branch**: Use Sea Dance 2 for current best results.

### Fix video aspect ratio
- **Timestamp**: [06:14](https://www.youtube.com/watch?v=a4p6ykdRmzc&t=374)
- **Action**: Correct the generated video's aspect ratio and background color.
- **Command Or Clicks**: Prompt: 'Video should be 1:1 aspect ratio... background should be pure white.'

### Finalize and integrate video
- **Timestamp**: [06:14](https://www.youtube.com/watch?v=a4p6ykdRmzc&t=374)
- **Action**: Remove audio, flip direction if needed, and add video to the website.
- **Command Or Clicks**: Prompt: 'Remove audio from this video... flip it horizontally... add to website.'
- **Choice Branch**: Use FFmpeg script if needed to strip audio.

## Gotchas

### Video generation can take several minutes; be patient while Claude processes the request.
- **Severity**: heads_up
- **Timestamp**: [05:27](https://www.youtube.com/watch?v=a4p6ykdRmzc&t=327)

### Ensure the avatar has enough white space at top and bottom to prevent animation clipping.
- **Severity**: serious
- **Timestamp**: [04:06](https://www.youtube.com/watch?v=a4p6ykdRmzc&t=246)

### Remove audio from the video file to avoid unwanted sound on the website.
- **Severity**: blocking
- **Timestamp**: [06:14](https://www.youtube.com/watch?v=a4p6ykdRmzc&t=374)

## Where to go next

Check the Higgsfield video tab to review previous generations. Use the provided link for free credits. Explore more AI coding tips in the channel's playlist.

## Concepts surfaced

[[claude-code]] · [[higgsfield-ai]] · [[ai-avatar-generation]] · [[video-animation]] · [[landing-page-design]] · [[mcp-integration]]
