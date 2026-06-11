# Skills Field Manual — Key Notes for This Competition

Source: clief-notes-skills-field-manual-v1.pdf (Clief Notes Premium, March 2026)

The operator folder we're building IS the methodology in this manual applied to a single workflow.

---

## The Core Principle

The biggest lever in AI output quality is not the prompt. It is what information the model can see when it processes that prompt. **Context architecture beats prompt wordsmithing every time.**

---

## The 60/30/10 Framework

| Layer | What it handles | Examples |
|-------|----------------|---------|
| **60%** | Deterministic / database tasks | Lookups, data processing, code execution |
| **30%** | Rule-based tasks | Templates, routing logic, structured processes |
| **10%** | Judgment tasks | Synthesis, novel reasoning, edge case calls |

The operator we're building is primarily a **30% tool** — rules and routing logic. The edge cases encoded in `rules.md` push into 10% territory where judgment is required.

---

## How the Operator Folder Maps to the Skill Stack

| Operator File | Skill Equivalent | Layer |
|---------------|-----------------|-------|
| `identity.md` | Custom instructions / Project system prompt | Infra |
| `rules.md` | The 30% decision logic encoded explicitly | 30% |
| `examples.md` | Few-shot examples that calibrate judgment | 10% |
| `reference/` | Checklists and templates (deterministic scaffolding) | 60%/30% |
| `README.md` | Onboarding doc for a new user/operator | Infra |

---

## Relevant Skill: Custom Skills (Skill 2)

Skills are folders with a SKILL.md that Claude loads on demand. The competition operator folder is essentially a custom skill for one specific workflow.

Key principle from the manual: **Start by noticing what you repeat.** If you copy-paste the same instructions into three different conversations, that is a skill waiting to be packaged.

The SKILL.md description field is critical — Claude uses it to decide when to activate the skill. Write it like a trigger condition.

---

## Relevant Skill: Claude Code + CLAUDE.md (Skill 3)

The CLAUDE.md in an operator folder acts as the persistent system prompt. Write it like orientation notes for a contractor starting their first day:
- What the operator is
- What falls inside and outside its job
- How to handle edge cases
- What requires human escalation

---

## The Decision Question for Building the Operator

From the manual's decision sequence — applied to this comp:

1. Does the operator need persistent context? → Yes → that's `identity.md`
2. Is there a repeatable process? → Yes → that's `rules.md`
3. What's the output format? → Drafted action (email, flag, decline) → template in `reference/`
4. Does it need deep reasoning? → Only on edge cases → handle those explicitly in `rules.md`, not by deferring to the user
