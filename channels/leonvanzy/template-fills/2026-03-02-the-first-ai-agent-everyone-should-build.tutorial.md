---
video_id: qkzCb1pRdFU
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-03-02-the-first-ai-agent-everyone-should-build.md
source_transcript: ../transcripts/2026-03-02-the-first-ai-agent-everyone-should-build.md
source_summary_hash: sha256:0a22e94d893b7a78b32c56e6e07c47c96530a4e714fe470157e26ec3e55bccc7
source_transcript_hash: sha256:f290580a3a4a428a1b44cd4d41edbfd574c626f31149ced33dc6c2e87da126a5
fill_id: 1e1a73b6-10d2-4a01-9979-5554e8de0e65
published_at: '2026-10-19T21:54:19.817348'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Build a free, self-hosted AI assistant in N8N that remembers you and researches the web.

## Prerequisites

### Node.js and npm
- **Kind**: tool
- **Note**: Required to install N8N locally via npm.

### OpenRouter account
- **Kind**: account
- **Note**: Provides API key for chat model access; paid service.

### SerpAPI account
- **Kind**: account
- **Note**: Provides API key for Google search tool.

## Steps

### Install N8N locally
- **Timestamp**: [00:00](https://www.youtube.com/watch?v=qkzCb1pRdFU&t=0)
- **Action**: Open your command prompt or terminal and install the latest version of N8N globally using npm. Then start N8N and open the provided URL in your browser to access the dashboard.
- **Command Or Clicks**: npm install -g n8n@latest
n8n
- **Choice Branch**: Alternatively, use N8N Cloud (~€24/month) or self-host on a VPS via Hostinger (~$5/month) with coupon 'Leon' for 10% off.

### Create a new workflow from scratch
- **Timestamp**: [02:08](https://www.youtube.com/watch?v=qkzCb1pRdFU&t=128)
- **Action**: From the N8N dashboard, click 'Start from scratch' and rename the workflow to 'My AI Assistant'. Add an 'On chat message' trigger node as the starting point.
- **Command Or Clicks**: Click 'Start from scratch' → rename workflow → add 'On chat message' trigger

### Add AI agent and chat model
- **Timestamp**: [03:55](https://www.youtube.com/watch?v=qkzCb1pRdFU&t=235)
- **Action**: Add an AI agent node and connect a chat model. Choose 'Open Router chat model' and create credentials with your OpenRouter API key. Select Anthropic's Claude 4.6 model.
- **Command Or Clicks**: Add AI agent node → add chat model → create credential → paste API key → select model
- **Choice Branch**: You can also use Ollama to run models locally.

### Set agent personality with system message
- **Timestamp**: [05:11](https://www.youtube.com/watch?v=qkzCb1pRdFU&t=311)
- **Action**: Double-click the AI agent node, add a system message with a role prompt (e.g., 'You are a personal assistant called Luna...') and inject the current date/time using a variable.
- **Command Or Clicks**: Double-click AI agent → add system message → include {{ $now }} variable

### Add conversational memory
- **Timestamp**: [06:02](https://www.youtube.com/watch?v=qkzCb1pRdFU&t=362)
- **Action**: In the AI agent node, assign the 'Simple Memory' node and set it to remember the last 20 messages of the conversation.
- **Command Or Clicks**: Click 'Memory' → add 'Simple Memory' → set to 20 messages

### Create a data table for long-term memory
- **Timestamp**: [07:03](https://www.youtube.com/watch?v=qkzCb1pRdFU&t=423)
- **Action**: Go to the N8N dashboard, create a new data table named 'memories' with columns 'memory key' and 'memory value' (both strings). Add a test record (e.g., favorite color = red).
- **Command Or Clicks**: Dashboard → Data tables → Create new → name 'memories' → add columns → add record

### Add tools to get, insert, and update memories
- **Timestamp**: [08:00](https://www.youtube.com/watch?v=qkzCb1pRdFU&t=480)
- **Action**: Under the AI agent's tools, add three data table tools: 'get memories' (operation: get), 'insert memory' (operation: insert), and 'update memory' (operation: update with condition on ID). Rename them accordingly.
- **Command Or Clicks**: Add tool → Data table → select operation → configure table and fields

### Add web research tools
- **Timestamp**: [09:18](https://www.youtube.com/watch?v=qkzCb1pRdFU&t=558)
- **Action**: Add three tools: SerpAPI for Google search (requires API key), Wikipedia, and Hacker News. No configuration needed for the latter two.
- **Command Or Clicks**: Add tool → SerpAPI → paste API key
Add tool → Wikipedia
Add tool → Hacker News

### Make chat publicly available
- **Timestamp**: [10:20](https://www.youtube.com/watch?v=qkzCb1pRdFU&t=620)
- **Action**: In the chat message node, change mode to 'hosted chat', set authentication with username/password, and update the initial message to 'Luna'. Publish the workflow and copy the URL.
- **Command Or Clicks**: Chat message node → Mode: Hosted chat → Set auth → Publish → Copy URL

### Enable file uploads
- **Timestamp**: [11:21](https://www.youtube.com/watch?v=qkzCb1pRdFU&t=681)
- **Action**: Under options, enable 'allow file uploads', publish the workflow again, and refresh the chat to attach files.
- **Command Or Clicks**: Options → Allow file uploads → Publish → Refresh chat

## Gotchas

### You must provide an OpenRouter API key to use the chat model; without it, the agent won't respond.
- **Severity**: blocking
- **Timestamp**: [03:55](https://www.youtube.com/watch?v=qkzCb1pRdFU&t=235)

### For the update memory tool, you must add a description telling the agent the ID is a number; otherwise it may fail to determine the correct record.
- **Severity**: blocking
- **Timestamp**: [08:00](https://www.youtube.com/watch?v=qkzCb1pRdFU&t=480)

### Conversational memory only lasts within a session; long-term memory requires the data table tools.
- **Severity**: heads_up
- **Timestamp**: [06:02](https://www.youtube.com/watch?v=qkzCb1pRdFU&t=362)

## Where to go next

Check out the creator's school community for structured courses on N8N and Claude Code, plus a community of AI builders. Join now to lock in $7/month before the price increases after 1,000 members.

## Concepts surfaced

[[conversational-memory]] · [[long-term-memory]] · [[tool-calling]] · [[data-tables]] · [[self-hosting]] · [[web-research]]
