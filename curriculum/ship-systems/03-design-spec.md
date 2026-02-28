# Module 03: Design Spec

## Ship Systems Weekend — Saturday, 11:00 AM

---

## Objective
Translate the system definition into a technical specification: architecture diagram, data flow, agent roles, and tool list. This is the blueprint you build from.

## Duration
90 minutes (including lunch overlap — participants can eat while designing)

---

## Facilitator Guide

### Frame (10 min)
> "You now know what your system does. This module is about how it does it. By the end, you'll have a spec that another engineer could pick up and build from."

Walk through the four components of a spec:
1. **Architecture diagram** — boxes and arrows. What are the components? How do they connect?
2. **Data flow** — what data moves where? What transformations happen?
3. **Agent roles** — if your system has agents, what does each one do? What are its boundaries?
4. **Tool list** — what external tools, APIs, or services does each agent/component use?

### Build Block (60 min)
Participants fill out the spec template. Encourage hand-drawn architecture diagrams first — paper beats software for speed.

Common failure modes to watch for:
- **Over-architecting**: three agents when one will do. Push for the simplest design that works.
- **Missing data flow**: they know the components but can't explain how data moves between them.
- **Vague tool list**: "uses an LLM" — which model? Which API? What parameters?

### Pair Review (20 min)
Pair participants. Each person explains their spec to their partner in 5 minutes. Partner asks:
- "Where does [X input] go first?"
- "What happens if [Y step] fails?"
- "Which agent handles [Z task]?"

If the builder can't answer clearly, the spec needs work.

---

## Participant Template

### Architecture Spec

**System Name:** ___

**Architecture Diagram:**
_Draw or describe the components and their connections. Use ASCII, a photo of a whiteboard sketch, or a simple diagram tool._

```
[Component A] ---> [Component B] ---> [Output]
      |                  ^
      v                  |
[Component C] -----------+
```

**Components:**

| Component | Responsibility | Technology |
|-----------|---------------|------------|
| | | |
| | | |
| | | |

**Data Flow:**
1. User provides [input] via [method]
2. [Component A] receives input and [action]
3. [Component A] sends [data] to [Component B]
4. [Component B] [processes/transforms] and produces [output]
5. [Output] is returned to user via [method]

**Agent Roles** (if applicable):

| Agent | Role | Tools | Boundaries |
|-------|------|-------|------------|
| | | | |
| | | | |

**Tool & API List:**

| Tool/API | Purpose | Auth Required | Cost |
|----------|---------|---------------|------|
| | | | |
| | | | |

**Key Decisions:**
_List 2-3 architectural decisions you made and why._
1. ___
2. ___
3. ___

---

## Artifact
Each participant commits: `docs/architecture-spec.md` to their repo.
