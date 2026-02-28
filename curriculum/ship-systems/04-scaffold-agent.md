# Module 04: Scaffold Agent

## Ship Systems Weekend — Saturday, 1:00 PM

---

## Objective
Set up the repository, create the agent skeleton, and stub out every tool. By the end of this module, you have a runnable project that does nothing yet — but has the right shape.

## Duration
90 minutes

---

## Facilitator Guide

### Frame (10 min)
> "You have a spec. Now you build the skeleton. This module is about structure, not logic. When you're done, your project runs, your agent initializes, and every tool is a stub that returns a placeholder. No real logic yet — that's next module."

Why scaffold first:
- Forces you to validate your architecture before writing business logic
- Catches dependency issues early
- Creates a commit checkpoint you can always return to
- Makes the implementation module faster because the structure is settled

### Build Block (70 min)

**Step 1: Repository Setup (15 min)**
Participants should have a repo from the setup checklist. If not, create one now.

Required structure (adapt to language/framework):
```
project/
  src/
    agent.{ts,py}       # Main agent entry point
    tools/               # One file per tool
      tool-a.{ts,py}
      tool-b.{ts,py}
    config.{ts,py}       # Configuration and env vars
  tests/                 # Empty for now — Module 06
  docs/
    system-definition.md # From Module 02
    architecture-spec.md # From Module 03
  .env.example           # Required env vars (no secrets)
  README.md              # What the system does, how to run it
```

**Step 2: Agent Skeleton (25 min)**
- Initialize the agent with the chosen framework/SDK
- Configure model, system prompt, and tool registration
- Agent should start and respond to a basic health check

**Step 3: Tool Stubs (30 min)**
- Create one file per tool from the architecture spec
- Each tool stub: correct function signature, docstring, returns a placeholder
- Register all tools with the agent
- Run the agent — it should start without errors

### Checkpoint
> "Run your agent. Does it start? Does it list its tools? Can you send it a message and get a response (even a placeholder)? If yes, commit. If no, fix it before moving on."

---

## Participant Checklist

- [ ] Repository initialized with correct structure
- [ ] README with project name, description, and run instructions
- [ ] `.env.example` with all required environment variables listed
- [ ] Agent entry point created and runnable
- [ ] System prompt written (from system definition)
- [ ] All tools stubbed with correct signatures
- [ ] All tools registered with agent
- [ ] Agent starts without errors
- [ ] Agent responds to basic input (even with placeholder output)
- [ ] Code committed: `git commit -m "scaffold: agent skeleton with tool stubs"`

---

## Common Issues

| Problem | Fix |
|---------|-----|
| Missing API key | Check `.env` file, confirm key is set |
| Import errors | Check package installation, run `npm install` or `pip install -r requirements.txt` |
| Agent won't start | Check entry point, confirm main function is called |
| Tool not registered | Verify tool registration in agent config |
| Wrong SDK version | Check `package.json` or `requirements.txt` for version pinning |

---

## Artifact
Each participant commits their scaffold: runnable agent with all tools stubbed.
