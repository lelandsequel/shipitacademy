# Module 07: Add Interface

## Ship Systems Weekend — Sunday, 10:30 AM

---

## Objective
Add a user-facing interface to your system. Your system works and is tested — now make it usable by someone who isn't you. Choose one: CLI, web UI, or API endpoint.

## Duration
90 minutes

---

## Facilitator Guide

### Frame (10 min)
> "Your system works in a test harness. Now make it work for a user. Pick the interface that makes sense for your system and your audience. Don't overthink it — you have 90 minutes."

### Choosing an Interface (5 min)
Help participants pick the right interface:

| Interface | Best When | Tech Options |
|-----------|-----------|-------------|
| **CLI** | Your user is technical, the system is a tool | argparse, commander, click, inquirer |
| **Web UI** | You want to demo visually, the system has visual output | Next.js, Streamlit, Gradio, plain HTML |
| **API Endpoint** | The system will be consumed by other software | Express, FastAPI, Hono |

Rule: pick one. Do not build two. You have 90 minutes.

### Build Block (70 min)

**CLI path:**
- Parse arguments or interactive prompts
- Call the agent/system with parsed input
- Display output in a readable format
- Handle errors gracefully
- Add `--help` flag

**Web UI path:**
- Single page: input form and output display
- Call the agent/system from the frontend or via a local API
- Show loading state while processing
- Display output clearly
- No auth required for the weekend build

**API path:**
- Single endpoint that accepts input
- Calls the agent/system
- Returns structured JSON output
- Include basic error responses (400, 500)
- Document the endpoint in README

### Checkpoint (5 min)
> "Can someone who has never seen your code use your system? If you handed them your laptop, could they figure it out in 60 seconds? If not, simplify."

---

## Participant Checklist

### CLI
- [ ] Entry point command works (`node cli.js`, `python cli.py`, or binary)
- [ ] Accepts input via arguments or interactive prompts
- [ ] Displays output in readable format
- [ ] `--help` shows usage instructions
- [ ] Errors display useful messages (not stack traces)

### Web UI
- [ ] Starts with a single command (`npm run dev`, `streamlit run app.py`)
- [ ] Input form accepts user data
- [ ] Submit button triggers the system
- [ ] Loading state visible during processing
- [ ] Output displays clearly on the page

### API
- [ ] Server starts with a single command
- [ ] Endpoint accepts POST with JSON body
- [ ] Returns structured JSON response
- [ ] Returns appropriate error codes
- [ ] README documents the endpoint, request format, and response format

---

## Artifact
Each participant commits: working interface (CLI, web UI, or API endpoint) that a user can interact with.
