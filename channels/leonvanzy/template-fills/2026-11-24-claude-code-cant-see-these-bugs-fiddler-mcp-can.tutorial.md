---
video_id: P4JSc8TYo4I
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-11-24-claude-code-cant-see-these-bugs-fiddler-mcp-can.md
source_transcript: ../transcripts/2026-11-24-claude-code-cant-see-these-bugs-fiddler-mcp-can.md
source_summary_hash: sha256:c50da9d5fdf8c4592053628b491309471a649f33dd6947e129c552dfb84890e7
source_transcript_hash: sha256:7806d67f1ba3238e916ce2acddc6dd781cbbe792a147a016d218243f1763876b
fill_id: 09263f88-7156-4837-8306-d33ceb5d4d9a
published_at: '2026-11-26T01:40:46.269072'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Connect Fiddler Everywhere to Claude Code via MCP to see and fix HTTP traffic bugs that code analysis alone can't reveal.

## Prerequisites

### Fiddler Everywhere account
- **Kind**: account
- **Note**: Free 10-day trial; sign up at the link in the description.

### Fiddler Everywhere installed
- **Kind**: tool
- **Note**: Supports Mac, Windows, and Linux.

### Claude Code
- **Kind**: tool
- **Note**: The AI coding agent used in the demo; must be installed and accessible.

## Steps

### Create a Fiddler Everywhere account and install the app
- **Timestamp**: [03:31](https://www.youtube.com/watch?v=P4JSc8TYo4I&t=211)
- **Action**: Go to the Fiddler Everywhere page, click 'Try it for free', download the installer, and complete installation. The app is available on Mac, Windows, and Linux.
- **Command Or Clicks**: Click 'Try it for free' → download → install.

### Log in and open Fiddler Everywhere
- **Timestamp**: [04:39](https://www.youtube.com/watch?v=P4JSc8TYo4I&t=279)
- **Action**: Launch Fiddler Everywhere, log in or create an account. The main interface shows a pure browser (Chrome) for recording traffic, live traffic on the left, and rules on the right.
- **Command Or Clicks**: Open Fiddler Everywhere → log in.

### Configure Fiddler MCP for Claude Code
- **Timestamp**: [05:00](https://www.youtube.com/watch?v=P4JSc8TYo4I&t=300)
- **Action**: Go to Settings → MCP server, choose Claude Code, and click to configure. Restart Claude Code for the changes to take effect.
- **Command Or Clicks**: Settings → MCP server → Claude Code → restart Claude Code.

### Verify MCP connection by listing tools
- **Timestamp**: [05:30](https://www.youtube.com/watch?v=P4JSc8TYo4I&t=330)
- **Action**: In Claude Code, ask the agent to list all Fiddler MCP tools. Claude reports over 20 tools, confirming the connection.
- **Command Or Clicks**: Ask: 'List all Fiddler MCP tools.'

### Open the app in the Fiddler browser
- **Timestamp**: [05:45](https://www.youtube.com/watch?v=P4JSc8TYo4I&t=345)
- **Action**: Ask Claude to open the application in the Fiddler browser. Claude uses the Fiddler MCP to launch a Chrome browser that records traffic.
- **Command Or Clicks**: Ask: 'Open this application in the Fiddler browser.'

### Reproduce the error and inspect the 401 entry
- **Timestamp**: [06:07](https://www.youtube.com/watch?v=P4JSc8TYo4I&t=367)
- **Action**: In the Fiddler browser, click 'Check Forecast' to trigger the error. Then ask Claude to use Fiddler to diagnose why it failed. Claude finds a 401 entry in the traffic.
- **Command Or Clicks**: Click 'Check Forecast' → ask: 'Something went wrong. Use Fiddler to figure out why.'

### Disable header and URL scrubbing in Fiddler
- **Timestamp**: [07:04](https://www.youtube.com/watch?v=P4JSc8TYo4I&t=424)
- **Action**: Go to Settings → Sanitization, disable header scrubbing and URL scrubbing. Save changes, then tell Claude to check again without changing anything.
- **Command Or Clicks**: Settings → Sanitization → disable header scrubbing and URL scrubbing → Save.

### Identify the missing 'Bearer' prefix
- **Timestamp**: [07:30](https://www.youtube.com/watch?v=P4JSc8TYo4I&t=450)
- **Action**: With scrubbing disabled, Fiddler shows the authorization header is missing the 'Bearer' prefix. The response payload indicates a credentials problem.
- **Command Or Clicks**: Inspect the 401 entry in Fiddler.

### Test the fix by editing the request in Composer
- **Timestamp**: [07:58](https://www.youtube.com/watch?v=P4JSc8TYo4I&t=478)
- **Action**: Right-click the entry, select 'Edit in Composer', add 'Bearer ' to the authorization value, and resubmit. Confirm the request succeeds. Then corrupt the token to verify the error returns, and revert.
- **Command Or Clicks**: Right-click → Edit in Composer → add 'Bearer ' → Run.

### Ask Claude to fix the authentication header
- **Timestamp**: [08:30](https://www.youtube.com/watch?v=P4JSc8TYo4I&t=510)
- **Action**: Ask Claude to fix the authentication header in the code. After the fix, click 'Check Forecast' in the app and confirm the correct response.
- **Command Or Clicks**: Ask: 'Fix the authentication header.' → Click 'Check Forecast'.

### Create a rate-limit rule via Claude
- **Timestamp**: [08:50](https://www.youtube.com/watch?v=P4JSc8TYo4I&t=530)
- **Action**: Ask Claude to create a Fiddler rule that simulates rate limiting for the specific forecast endpoint. The rule appears under MCP rules in Fiddler.
- **Command Or Clicks**: Ask: 'Create a rule to simulate rate limiting for this endpoint.'

### Enable the rule and observe 429 responses
- **Timestamp**: [09:06](https://www.youtube.com/watch?v=P4JSc8TYo4I&t=546)
- **Action**: In Fiddler, go to Traffic, enable the MCP rule. Click 'Check Forecast' and see 429 status codes. Open a new Claude session and ask it to diagnose the failure.
- **Command Or Clicks**: Enable rule → Click 'Check Forecast' → New session → ask: 'Forecast not working. Use Fiddler to find out why.'

### Implement retry logic for rate limits
- **Timestamp**: [09:53](https://www.youtube.com/watch?v=P4JSc8TYo4I&t=593)
- **Action**: Ask Claude to add retry logic: repeat the request up to three times, then show a clear message. Re-enable the rule, test, and confirm the retry works. Disable the rule to restore normal operation.
- **Command Or Clicks**: Ask: 'Add retry logic (up to 3 attempts).' → Enable rule → Test → Disable rule.

### Simulate slow responses with a delay rule
- **Timestamp**: [10:30](https://www.youtube.com/watch?v=P4JSc8TYo4I&t=630)
- **Action**: Ask Claude to add a rule that delays the forecast service by 8 seconds. Click 'Check Forecast' and observe the app appears frozen.
- **Command Or Clicks**: Ask: 'Add an 8-second delay to the forecast service.' → Click 'Check Forecast'.

### Diagnose the slow request with Fiddler
- **Timestamp**: [11:02](https://www.youtube.com/watch?v=P4JSc8TYo4I&t=662)
- **Action**: Open a new Claude session and ask it to find which request is slow. Claude uses Fiddler to identify the endpoint and the 8-second latency.
- **Command Or Clicks**: New session → ask: 'Forecast is slow. Use Fiddler to find the slow request.'

## Gotchas

### Fiddler masks sensitive data (API keys, auth headers) by default, hiding the root cause from the agent. Disable scrubbing in Settings → Sanitization to see the full details.
- **Severity**: blocking
- **Timestamp**: [06:07](https://www.youtube.com/watch?v=P4JSc8TYo4I&t=367)

### When you create a rule in one Claude session, it persists; a new session may not know about it and could misdiagnose the issue.
- **Severity**: heads_up
- **Timestamp**: [09:06](https://www.youtube.com/watch?v=P4JSc8TYo4I&t=546)

## Where to go next

Now that you've seen Fiddler MCP in action, explore its rules for load testing and error injection. Check the Fiddler MCP documentation for more advanced scenarios.

## Concepts surfaced

[[http-traffic-inspection]] · [[mcp-server]] · [[ai-agent-debugging]] · [[rate-limiting]] · [[api-testing]]
