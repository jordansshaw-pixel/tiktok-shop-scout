# TikTok Shop Product Scout — Folder-Based AI Operator

This is a folder-based AI operator for TikTok Shop affiliates.

Drop this folder into a Claude project or point Claude Code at it. Paste any product listing — a URL, a screenshot, or whatever details you have — and it returns exactly one of three decisions:

- **PROMOTE:** the product scored against a six-dimension rubric, passed compliance, and ships with a category-aware ready-to-film script. Not a brief. Not a hook idea. A script you can film today.
- **SKIP:** the specific rule that killed it is logged in one line.
- **WATCHLIST:** the exact signal that flips the product to PROMOTE is named, with the date to check it.

It never answers "it depends" — missing data gets estimated and scored conservatively, compliance disqualifiers override any score, and edge cases like saturated-but-viral products, wellness-adjacent claim risk, sub-$8 items, seasonal waves, and unconfirmed commission are handled as explicit rules in `rules.md`, not kicked back as questions.

Swap `reference/audience-profile.md` and it redeploys for a different creator. That is the full pipeline: one folder, one decision, every time.

## Judge View

Most AI tools answer a creator's question. This folder governs the decision.

TikTok Shop Product Scout turns messy product signals into one business action: **PROMOTE**, **SKIP**, or **WATCHLIST**. The folder makes the decision path visible: disqualifiers first, then scoring, thresholds, edge cases, and a required output format.

```text
MESSY PRODUCT SIGNAL -> GOVERNED DECISION PATH -> BUSINESS ACTION
```

## Competition Framing

**Cohort:** Business

This is a business decision workflow for affiliate creators: it turns messy TikTok Shop product signals into a governed **PROMOTE / SKIP / WATCHLIST** call before filming time, audience trust, or compliance risk is spent. PROMOTE routes directly to a ready-to-film script. The creator use case is the demo; the underlying pattern is governed AI judgment.

See `submission-positioning.md` for the judge-facing submission definition and `presentation/submission-hub.html` for the single presentation target.

## Operator Core

The operator follows the five-part folder methodology:

| File | Job |
|------|-----|
| `identity.md` | Who the operator is and what workflow it owns |
| `rules.md` | Decision logic: criteria, thresholds, edge cases, escalation rules |
| `examples.md` | Decisions in action, including edge cases |
| `reference/` | Checklists, templates, rubrics, audience profile, and script scaffolds |
| `README.md` | How to use the operator |

Key reference files:

| File | Job |
|------|-----|
| `reference/scoring-rubric.md` | The 1–5 anchors for all six dimensions |
| `reference/disqualifiers.md` | Compliance hard-stops and claim-language rules |
| `reference/audience-profile.md` | The buyer the operator scouts for (swappable) |
| `reference/output-templates.md` | The three output formats — every decision ships in one |
| `reference/script-templates.md` | Category-aware scaffolds for ready-to-film PROMOTE scripts |

## Submission Wrapper

These files package the operator for judging, but are not required for runtime:

| File | Job |
|------|-----|
| `submission-positioning.md` | Business cohort framing and judge-facing submission definition |
| `presentation/` | Judge-facing hub, animated walkthrough, script, demo run, and visual direction |

## Try it

Heatless curlers example video with captions: https://youtube.com/shorts/xiNW8VM4dcg

Paste this after loading the folder: *"Score this: collapsible travel water bottle, $11, commission unknown, saw it three times on my FYP this week."* You should get back a single decision with rubric scores, an estimated-and-labeled commission, and either a brief, a log line, or a flip condition — not a question.
