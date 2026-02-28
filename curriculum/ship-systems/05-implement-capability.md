# Module 05: Implement Capability

## Ship Systems Weekend — Saturday, 2:30 PM

---

## Objective
Build the core capability: one complete end-to-end flow that takes real input, processes it through your agent, and produces real output. This is the most important module of the weekend.

## Duration
2.5 hours (until end of Saturday)

---

## Facilitator Guide

### Frame (10 min)
> "You have a skeleton. Now you make it do the one thing it's supposed to do. Not all the things. The one thing. Pick the most important flow from your system definition and make it work end-to-end."

Rules for this module:
1. **One flow only.** Do not try to implement everything. Pick the core capability.
2. **End-to-end means end-to-end.** Input goes in, output comes out. No manual steps in the middle.
3. **Real data, not mock data.** Use actual API calls, actual model responses, actual file operations.
4. **Working beats clean.** Refactor tomorrow. Ship today.

### Selecting the Core Flow (10 min)
Help each participant identify their core flow. Ask:
- "If your system could only do one thing, what would it be?"
- "What's the flow that proves this system works?"
- "What would you show in a 30-second demo?"

That's the flow they implement now.

### Build Block (2 hours)
This is deep work time. Minimize interruptions.

**Facilitator role during build block:**
- Walk the room every 20 minutes
- Check: is anyone stuck? Anyone going down a rabbit hole?
- Common intervention: "That's a nice-to-have. Cut it. Get the core flow working first."
- If someone is blocked on an API or tool issue, help them unblock. Don't let them sit stuck.

**Pacing checkpoints:**
- **:30 min** — First tool should be implemented (not stubbed). If not, scope is too big.
- **:60 min** — Data should be flowing between at least two components. If not, debug the integration.
- **:90 min** — Core flow should produce output (even if rough). If not, cut scope further.
- **:120 min** — Core flow should be complete and repeatable. Commit.

### End of Day Review (10 min)
Quick around-the-room check:
- "Show me your system taking input and producing output."
- No slides. No explanations. Just run it.
- If it works: commit, push, you're done for the day.
- If it doesn't: note what's broken. First task tomorrow is fixing it before Module 06.

---

## Participant Guide

### Step 1: Identify Your Core Flow
Write it as a single sentence:
> "User provides [input], system [processes it using tools X and Y], and produces [output]."

### Step 2: Implement Tools (in order of the data flow)
Work through the flow left to right:
1. Implement the first tool that touches the input
2. Implement the processing/transformation tool(s)
3. Implement the output tool

For each tool:
- Replace the stub with real logic
- Test it in isolation: does it work with sample input?
- Wire it into the agent flow
- Test the integration: does data flow correctly from the previous step?

### Step 3: Run the Full Flow
- Provide real input
- Watch it flow through the system
- Check the output against your success criteria from Module 02
- Fix what's broken
- Run it again

### Step 4: Commit
```bash
git add -A
git commit -m "feat: implement core capability — [describe what the flow does]"
git push
```

---

## Troubleshooting

| Symptom | Likely Cause | Fix |
|---------|-------------|-----|
| Tool works alone but fails in agent | Input/output format mismatch | Check what the agent sends vs. what the tool expects |
| API returns errors | Auth, rate limits, or malformed request | Check API docs, verify key, inspect request payload |
| Output is wrong but no errors | Prompt issue or data transformation bug | Log intermediate steps, inspect what each tool receives and returns |
| System is too slow | Too many API calls or large payloads | Reduce input size for testing, optimize later |
| Scope feels too big | It is too big | Cut features. Ship the minimum flow. |

---

## Artifact
Each participant commits: working core capability with at least one end-to-end flow.

## End of Saturday
You now have a working AI system. It does one thing. It does it for real. Tomorrow you add eval, an interface, deploy it, and record a demo.
