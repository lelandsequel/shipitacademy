# Module 04: AI Stack

## Leverage Systems Weekend — Saturday, 1:00 PM

---

## Objective
Design the AI stack for your leverage system: which models, which tools, how they connect, and how the orchestration works. This is the technical design that turns your thesis into a buildable system.

## Duration
90 minutes

---

## Facilitator Guide

### Frame (10 min)
> "You have a thesis. Now you design the system that proves it. An AI stack is three layers: models (what thinks), tools (what acts), and orchestration (what coordinates). By the end of this module, you'll know exactly what you're building."

### The Three Layers

**Layer 1: Models**
- Which LLM(s) are you using?
- What tasks does each model handle?
- What quality/speed/cost tradeoffs are you making?
- API or local?

**Layer 2: Tools**
- What external services, APIs, or data sources does the system use?
- What file/data operations are needed?
- What integrations connect to existing workflow?

**Layer 3: Orchestration**
- How do the models and tools connect?
- What's the sequence of operations?
- Where does the human enter the loop?
- What triggers the workflow? (Manual, scheduled, event-driven)

### Build Block (70 min)

**Step 1: Model Selection (15 min)**
Participants choose models based on their task requirements:

| Consideration | Options |
|--------------|---------|
| Complex reasoning | Claude, GPT-4 class |
| Fast, simple tasks | Claude Haiku, GPT-4o-mini |
| Structured output | Any model with JSON mode |
| Code generation | Claude, GPT-4 class |
| Embeddings/search | Voyage, OpenAI embeddings |
| Vision/multimodal | Claude, GPT-4V |

**Step 2: Tool Inventory (20 min)**
List every tool the system needs:
- Data sources (APIs, databases, files)
- Processing tools (parsers, formatters, validators)
- Output tools (file writers, email senders, API calls)
- Integration tools (Slack, Notion, Google Docs, CRM)

**Step 3: Orchestration Design (35 min)**
Draw the flow:
1. What triggers the workflow?
2. What's the first step?
3. How does data flow between steps?
4. Where does a human review or approve?
5. What's the final output?

### Review (10 min)
Each participant explains their stack in 2 minutes:
- "I'm using [model] for [task], [tool] for [task], orchestrated by [method]."
- Facilitator checks: is this buildable in the next module? If the stack is too complex, simplify.

---

## Participant Template

### AI Stack Design

**System Name:** ___

**Models:**

| Model | Task | Why This Model |
|-------|------|---------------|
| | | |
| | | |

**Tools:**

| Tool/API | Purpose | Auth/Setup Required |
|----------|---------|-------------------|
| | | |
| | | |
| | | |

**Orchestration Flow:**

```
[Trigger] --> [Step 1: ___] --> [Step 2: ___] --> [Step 3: ___] --> [Output]
                  |                                    ^
                  v                                    |
            [Human Review] ------- approve ---------> +
```

**Step-by-Step Flow:**
1. Trigger: ___
2. Step 1: ___ (model/tool: ___)
3. Step 2: ___ (model/tool: ___)
4. Step 3: ___ (model/tool: ___)
5. Human checkpoint (if applicable): ___
6. Output: ___

**Orchestration Method:**
- [ ] Script (Python/Node sequential execution)
- [ ] Agent framework (LangChain, CrewAI, custom)
- [ ] Workflow tool (Make, Zapier, n8n)
- [ ] Custom orchestrator

**Environment Requirements:**
- API keys needed: ___
- Accounts needed: ___
- Data access needed: ___

---

## Artifact
Each participant commits: `docs/ai-stack.md` with model, tool, and orchestration decisions documented.
