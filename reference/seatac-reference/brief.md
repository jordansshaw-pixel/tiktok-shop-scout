# Clief Notes Weekly Competition #7 — The Operator

**Deadline:** Saturday, June 13, 2026 at 12:00 PM EST
**Submit:** Public GitHub repo link in the comments + 2–3 sentence description

---

## The Challenge

Build a folder-based AI operator that handles ONE operational workflow end-to-end. You pick the workflow.

Deliverable: one operator folder someone could drop into a Claude project and use to handle a real business workflow without babysitting.

---

## Pick Your Workflow

Be specific. "Customer support" is too broad. "Refund request triage for an ecommerce store doing under 200 orders per month" is the right level.

Spark ideas:
- Customer support triage (which tier handles this ticket?)
- Content review and approval
- Lead intake and qualification
- Refund request handler
- Partnership pitch evaluator
- Podcast guest pitch sorter
- Freelance project intake
- Resume screen for one specific role
- Meeting request triage (book, decline, delegate)

---

## The Core Distinction

An operator is NOT a chatbot.

- A chatbot responds.
- An operator makes a decision, then routes the work.

When the operator gets an input, it should decide and act. The user comes back to find the work already done, or correctly flagged for their input. "Use good judgment" is not a rule. "If years of experience is under 3, decline unless they've shipped a notable open source project" is.

---

## Required Folder Structure

```
operator-name/
├── identity.md       ← who the operator is and what workflow they own; what's in/out of scope
├── rules.md          ← decision logic, criteria, edge cases, escalation rules (the heart of the operator)
├── examples.md       ← 2–3 decisions in action; at least one edge case
├── reference/        ← checklists, templates, scoring rubrics, response templates
└── README.md         ← one paragraph, stranger can use it with zero other context
```

---

## What Goes in Each File

**identity.md** — Who is this operator and what workflow do they own? Be explicit about what falls inside their job and what falls outside it.

**rules.md** — The decision logic. Criteria. Edge cases. Escalation rules. This is the heart of the operator. Be specific. "Use good judgment" is not a rule.

**examples.md** — 2–3 example decisions showing the logic in action. Include at least one edge case. Show the operator handling something the obvious rules don't cover.

**reference/** — Sub-folder for criteria checklists, templates, scoring rubrics, or response templates the operator needs to do its job.

**README.md** — How someone uses this folder. One paragraph someone could follow with no other context.

---

## The Bar

Someone with no context should use your folder, feed it three real examples, and trust the output enough to act on it.

If the operator kicks the decision back to the user every time, you've missed the assignment.

---

## Judging Criteria (in order)

1. Does the operator actually make decisions? Or does it kick the question back?
2. Are the edge cases handled or hand-waved?
3. Would the output be trustworthy enough to act on?
4. README quality — can a stranger figure this out?

---

## Why This Matters for a Resume

"I built a folder-based AI operator that handles [workflow] end-to-end" is the kind of work companies pay for. Writing decision logic into rules is the foundation of automation — it translates directly into ops roles, automation engineering, and AI product work.
