# Module 06: Add Eval

## Ship Systems Weekend — Sunday, 9:00 AM

---

## Objective
Add evaluation to your system: test cases, pass/fail criteria, and automated checks. A system without eval is a toy. A system with eval is infrastructure.

## Duration
90 minutes

---

## Facilitator Guide

### Frame (10 min)
> "Yesterday you built a system that works. Today you prove it works. Eval is what separates a weekend hack from a real system. If you can't test it, you can't trust it, and you can't improve it."

Three levels of eval:
1. **Functional tests** — does the system produce output in the correct format?
2. **Quality tests** — is the output good? Does it meet the success criteria from Module 02?
3. **Regression tests** — when you change something, does the system still work?

For this weekend, participants build levels 1 and 2. Level 3 comes naturally from having 1 and 2.

### Build Block (70 min)

**Step 1: Define Test Cases (20 min)**
Participants write 3-5 test cases:
- 2 "happy path" cases — standard inputs that should produce correct output
- 1 "edge case" — unusual but valid input
- 1 "failure case" — invalid input that should be handled gracefully
- 1 "quality case" — input where you evaluate output quality, not just format

**Step 2: Write Pass/Fail Criteria (15 min)**
For each test case, define:
- What "pass" looks like (specific, measurable)
- What "fail" looks like
- Any partial credit criteria (for quality tests)

**Step 3: Implement Automated Checks (35 min)**
Create a test file that:
- Runs each test case through the system
- Checks output against pass/fail criteria
- Reports results: passed, failed, or error
- Can be run with a single command (`npm test`, `pytest`, or a custom script)

### Review (10 min)
Each participant runs their test suite. Report:
- How many tests pass?
- Which tests fail? Why?
- What would you add with more time?

---

## Participant Template

### Test Case Template

```markdown
## Test Case: [Name]

**Input:**
[Exact input to provide to the system]

**Expected Output:**
[What the system should produce — be specific about format and content]

**Pass Criteria:**
- [ ] Output is in correct format
- [ ] Output contains [specific element]
- [ ] Output does not contain [specific anti-pattern]

**Type:** happy-path | edge-case | failure | quality
```

### Eval Script Structure

```
tests/
  eval.{ts,py}           # Main eval runner
  cases/
    case-01-happy.json    # Test case data
    case-02-happy.json
    case-03-edge.json
    case-04-failure.json
    case-05-quality.json
```

### Minimum Eval Requirements
- [ ] 3+ test cases defined with inputs and expected outputs
- [ ] Pass/fail criteria written for each case
- [ ] Automated eval script that runs all cases
- [ ] Script reports pass/fail per case
- [ ] Script exits with non-zero code if any test fails
- [ ] All tests can be run with a single command

---

## Artifact
Each participant commits: test cases, eval criteria, and automated eval script.
