# Module 05: Workflow

## Leverage Systems Weekend — Saturday, 2:30 PM

---

## Objective
Build the workflow: a complete automated pipeline that takes real input, processes it through your AI stack, and produces real output. By the end of Saturday, your leverage system works end-to-end.

## Duration
2.5 hours (until end of Saturday)

---

## Facilitator Guide

### Frame (10 min)
> "You have a thesis and a stack design. Now you build the pipeline. One end-to-end flow. Real input. Real AI processing. Real output. When this works, you have proof your leverage thesis is valid."

### Rules for This Module
1. **One pipeline.** Not three. The core flow from your thesis.
2. **Real data.** Use your actual work inputs — a real email, a real document, a real dataset.
3. **End-to-end.** Input goes in one end, output comes out the other. No manual steps in between (except designed human checkpoints).
4. **Working beats perfect.** The output doesn't need to be polished. It needs to exist and be correct.

### Build Block (2 hours)

**Step 1: Set Up the Orchestration (30 min)**
- Create the project structure
- Install dependencies
- Configure API keys and connections
- Set up the entry point that kicks off the workflow

**Step 2: Build Each Step (60 min)**
Work through the flow in order:
1. Input ingestion — get the real data into the system
2. AI processing — model calls with the right prompts
3. Transformation — shape the output into the desired format
4. Human checkpoint — if applicable, show the output for review
5. Final output — produce the deliverable

**Step 3: Run with Real Data (30 min)**
- Feed in actual input from your work
- Watch it flow through the pipeline
- Inspect the output: is it usable? Does it match what you'd produce manually?
- Note quality gaps — don't fix them all now, but document them

**Pacing Checkpoints:**
- **:30 min** — Orchestration set up, first step working
- **:60 min** — At least two steps connected and passing data
- **:90 min** — Full pipeline running (output may be rough)
- **:120 min** — Pipeline produces usable output with real data

### End of Day Review (10 min)
Each participant demonstrates:
- "Here's my input: [shows real data]"
- "Here's what the system produces: [shows output]"
- "Here's what I'd normally spend [X hours] doing manually"

No slides. Just run the pipeline.

---

## Participant Guide

### Step 1: Prepare Your Input
Gather real data from your actual work:
- A real email, document, or dataset you've processed before
- Something you know the correct output for (so you can compare)
- At least 2-3 examples: one for building, one for testing

### Step 2: Build the Pipeline
Follow your AI stack design. Implement each step:

```
[Input] --> [Step 1] --> [Step 2] --> [Step 3] --> [Output]
```

For each step:
1. Write the code/configuration
2. Test it with sample data
3. Connect it to the previous step
4. Verify data flows correctly

### Step 3: Run End-to-End
- Use your real input
- Run the full pipeline
- Compare output to what you'd produce manually
- Note: where is it good? Where is it weak?

### Step 4: Document and Commit
```bash
git add -A
git commit -m "feat: working leverage pipeline — [describe what it does]"
```

Record:
- Input used: ___
- Output produced: ___
- Time to run: ___
- Manual equivalent time: ___
- Quality assessment: ___

---

## Troubleshooting

| Issue | Fix |
|-------|-----|
| API returns low-quality output | Improve the prompt. Be more specific about format and quality criteria. |
| Pipeline breaks between steps | Check data format: what step N outputs must match what step N+1 expects |
| Output is wrong format | Add a formatting/parsing step between the AI call and the output |
| Too slow | Reduce input size for testing. Optimize prompts. Consider faster models for simple steps. |
| Scope too big | Cut to one pipeline. One input, one output. Expand tomorrow. |

---

## Artifact
Each participant: working end-to-end pipeline with real data producing real output.

## End of Saturday
Your leverage system works. Tomorrow you build the value asset, write positioning, capture proof, and send outreach.
