# TikTok Shop Product Scout — Folder-Based AI Operator

Drop this folder into a Claude project (or point Claude Code at it) and paste in any TikTok Shop product — a listing URL, a screenshot description, or just the details you have. The operator scores it against a six-dimension rubric and returns exactly one of three decisions: **PROMOTE** (with a filming-ready content brief: hook, format, and an FTC-compliant caption draft), **SKIP** (with the specific rule that killed it, logged), or **WATCHLIST** (with the exact measurable signal that would flip the decision and a re-check date). It never answers "it depends" — missing data gets estimated and scored conservatively, compliance disqualifiers override any score, and edge cases (saturated-but-viral products, sub-$8 items, seasonal waves, wellness-adjacent claim risk) are handled by explicit rules in `rules.md` rather than kicked back to you. To use it for your own audience instead of the default (US women 18–34 impulse-shopping on TikTok Shop), swap `reference/audience-profile.md` — the decision logic stays the same.

## Files

| File | Job |
|------|-----|
| `identity.md` | Who the operator is, what's in/out of scope, the one escalation rule |
| `rules.md` | The decision logic — disqualifiers → rubric → thresholds → edge cases |
| `examples.md` | Three worked decisions, including an edge case the rules don't directly cover |
| `reference/scoring-rubric.md` | The 1–5 anchors for all six dimensions |
| `reference/disqualifiers.md` | Compliance hard-stops and claim-language rules |
| `reference/audience-profile.md` | The buyer the operator scouts for (swappable) |
| `reference/output-templates.md` | The three output formats — every decision ships in one |

## Try it

Paste this after loading the folder: *"Score this: collapsible travel water bottle, $11, commission unknown, saw it three times on my FYP this week."* You should get back a single decision with rubric scores, an estimated-and-labeled commission, and either a brief, a log line, or a flip condition — not a question.
