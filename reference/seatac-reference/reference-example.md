# Reference Example — Devon's Recruiting Firm

Source: Week7_Operator_Reference_Example.pdf

**Do not build this operator.** Use it as a template for how to scope your own.

---

## The Client

Devon runs a 4-person technical recruiting firm in Denver. Places engineers at Series A/B startups, mostly remote-friendly. Reputation built on speed and signal — founders get 3–5 pre-screened candidates per role.

## The Problem

40–60 resumes per day inbound. Devon makes a triage call in ~90 seconds: book a call, send a polite decline, or save for a future role. The call isn't hard — the volume is what kills.

## What Devon Needs

Paste a resume in. Operator reads it against open roles. Outputs one of three things every time:
- **Yes** → drafted outreach email
- **No** → drafted gracious decline
- **Maybe** → flagged for Devon's review

## The Decision Logic Devon Uses

- Stage-fit experience (startup stage match) matters MORE than specific tech stack
- Job hopping = yellow flag, not a red one
- Senior applying for mid-level role = likely trying to downshift on responsibility — can be a fit for some clients (edge case most tools fail on)
- When in doubt → flag for human review

---

## What Good Scope Looks Like

Notice the 5 things Devon is specific about:

1. **Specific workflow** — resume → decision → drafted response
2. **Specific output** — one of three things, every time
3. **Specific decision criteria** — stage experience > tech stack match
4. **Specific edge cases** — the senior applying mid-level
5. **Specific escalation rule** — when in doubt, flag for human review

Your workflow should be at least this specific.

---

## The Methodology Behind It

This is interpretable context methodology. Folders as architecture. Each file does one job well. The structure tells you what's where.

The operator folder IS the system prompt — split across multiple files so each piece is readable, editable, and portable.
