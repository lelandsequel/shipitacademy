# Operator Foundry — Build Task

## What You're Building
A complete Weekend Intensive program for **Operator Foundry** — an elite AI systems training lab.
Ghost-founder model: founder (TJ) is hidden, Charles is the facilitator, all content is branded as Operator Foundry.

## Source Material
Read: `/Users/sokpyeon/Library/Mobile Documents/com~apple~TextEdit/Documents/Weekenders.txt`

## Directory: `/Users/sokpyeon/.openclaw/workspace/operator-foundry/`

---

## DELIVERABLE 1: CURRICULUM MODULES

### Track A — Ship Systems Weekend

Create: `curriculum/ship-systems/`

**Saturday modules:**
- `01-kickoff.md` — Frame the goal, introduce the system, set expectations (facilitator guide + participant handout)
- `02-define-system.md` — Participants define what AI system they're building: problem, user, inputs/outputs
- `03-design-spec.md` — Write the spec: architecture diagram, data flow, agent roles, tool list
- `04-scaffold-agent.md` — Scaffold the codebase: repo setup, agent skeleton, tool stubs
- `05-implement-capability.md` — Build the core capability: first working end-to-end flow

**Sunday modules:**
- `06-add-eval.md` — Add evaluation: test cases, pass/fail criteria, automated checks
- `07-add-interface.md` — Add an interface: CLI, web UI, or API endpoint
- `08-deploy.md` — Deploy it: Vercel/Railway/Fly, env setup, live URL
- `09-record-demo.md` — Record a 2-min demo: what it does, how it works, what you'd build next

**Outcome doc:** `ship-systems-outcome.md` — what participants walk away with

---

### Track B — Leverage Systems Weekend

Create: `curriculum/leverage-systems/`

**Saturday modules:**
- `01-kickoff.md` — Frame the leverage model, introduce operator thinking
- `02-leverage-map.md` — Map current workflow: where time goes, where AI can multiply output
- `03-opportunity-thesis.md` — Pick the highest-leverage opportunity and write a one-page thesis
- `04-ai-stack.md` — Design the AI stack: models, tools, orchestration layer
- `05-workflow.md` — Build the workflow: first automated pipeline end-to-end

**Sunday modules:**
- `06-value-asset.md` — Create a value asset: doc, template, or tool that captures the leverage
- `07-positioning.md` — Write positioning: what you now offer, who it's for, why it's different
- `08-proof.md` — Capture proof: before/after, time saved, output quality comparison
- `09-outreach.md` — Write one outreach message to one real prospect using the new leverage

**Outcome doc:** `leverage-systems-outcome.md` — what participants walk away with

---

## DELIVERABLE 2: OPS INFRASTRUCTURE

Create: `ops/`

- `welcome-email.md` — Welcome email sent on registration. Warm, practical, sets expectations. Operator Foundry voice (not TJ personal brand).
- `setup-checklist.md` — What participants need before the weekend: accounts, tools, repo access, Discord invite
- `pre-weekend-brief.md` — Sent Thursday before the weekend. Schedule, what to bring, mindset
- `facilitator-runbook.md` — Charles's guide: how to run the weekend, pacing, how to handle stuck participants, artifact reviews
- `participant-agreement.md` — Short 1-page agreement: what they're building, what they'll have at the end, code of conduct

---

## DELIVERABLE 3: LANDING PAGE

Create: `site/index.html`

Single-page site. No framework, pure HTML/CSS. URL placeholder: `[DOMAIN]` (will be swapped in).

**Design**: Dark, engineering-grade, no fluff. NOT a generic course landing page. Think: YC, Stripe, Linear vibes. Dark background (#0A0A0A), clean white/grey type, one accent color (electric blue #0066FF or amber #F59E0B — pick whichever looks right).

**Sections:**
1. **Hero** — "Ship a real AI system in 48 hours." Sub: "Operator Foundry Weekend Intensives. Two tracks. One cohort. No fluff." CTA: "Apply for the next cohort →"
2. **The Problem** — Most AI training is demos and slides. You leave with nothing. Operator Foundry is different: you build something real and ship it before Sunday is over.
3. **Two Tracks** — Ship Systems: build a working AI system. Leverage Systems: build your operator leverage package. (Brief description of each)
4. **The Weekend** — Saturday: define, design, scaffold, build. Sunday: eval, deploy, demo. You ship.
5. **Who This Is For** — Developers who want to build AI systems. Operators who want AI leverage. Founders who want to move faster. NOT for beginners.
6. **Facilitator** — Charles Jourdan. [short bio placeholder]. Photo placeholder.
7. **Apply** — Simple form placeholder (name, email, which track, why you want in). CTA button.
8. **Footer** — "Operator Foundry is a program by TJ Jourdan." Small text. No more founder presence than that.

---

## STYLE GUIDE (all content)

**Voice**: Direct, engineering-grade, practitioner. No hype. No "transform your life." No emoji.
**Avoid**: founder personality, personal branding, inspirational quotes
**Use**: artifact names, system names, concrete outcomes, real tools
**Brand name**: always "Operator Foundry" — never "TJ's program" or similar

---

## WHEN DONE

Run: `openclaw system event --text "Done: Operator Foundry build complete — curriculum (2 tracks, 9 modules each), ops infra (5 docs), landing page. All in /workspace/operator-foundry/" --mode now`
