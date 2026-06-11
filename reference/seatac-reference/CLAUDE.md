# CF_Projects / 07_Competition

Clief Notes Weekly Competition #7 — The Operator.

**Deadline:** Saturday, June 13, 2026 at 12:00 PM EST

## What This Folder Is

Working directory for building and submitting a folder-based AI operator to the Clief Notes weekly comp.

## Key Files

| File | Purpose |
|------|---------|
| `brief.md` | Full competition rules and judging criteria |
| `reference-example.md` | Breakdown of the Devon recruiting firm example (do not build this) |
| `skills-field-manual-notes.md` | Relevant methodology from the Clief Notes Skills Field Manual |

## The Deliverable

A public GitHub repo containing one operator folder with:
- `identity.md`
- `rules.md`
- `examples.md`
- `reference/` subfolder
- `README.md`

Plus 2–3 sentence description of what workflow the operator handles and what decisions it makes.

## Operator Folder — `tiktok-shop-scout/`

**Workflow selected (2026-06-10):** TikTok Shop affiliate product triage. Paste a product listing → operator scores it on a 6-dimension rubric (commission, velocity, saturation, angle, ICP fit, price) → outputs PROMOTE (filming-ready brief + compliant caption), SKIP (logged with the killing rule), or WATCHLIST (measurable flip condition + re-check date).

Decision logic adapted from the live Hokulani pipeline (`Hokulani/agents/market-analyzer/`, `product-scout/`, `_config/compliance.md`, `_config/icp.md`).

**Submission description (draft):**
> I built a folder-based operator that triages TikTok Shop affiliate products end-to-end: paste a listing and it scores six dimensions against a rubric, applies FTC/compliance hard-stops, and returns exactly one decision — Promote (with a category-aware ready-to-film script, compliant caption, and rubric scores), Skip (logged with the rule that killed it), or Watchlist (with the measurable signal that flips it and an expiry date). Edge cases like saturated-but-viral products, sub-$8 AOV traps, seasonal waves, and wellness-adjacent claim risk are encoded as explicit rules, so the operator decides instead of deferring. A Promote doesn't hand back a brief — it hands back a script you can film today. Swap one reference file (the audience profile) and the same logic redeploys for any creator.

**Remaining before deadline (Sat June 13, 12:00 PM EST):**
- [x] Push `tiktok-shop-scout/` to a public GitHub repo — **https://github.com/jordansshaw-pixel/tiktok-shop-scout** (pushed 2026-06-10)
- [ ] Post repo link + description in the comp comments (manual — Coco)

Note: canonical source lives in this folder (`tiktok-shop-scout/`). The pushed working copy is at `%TEMP%\tiktok-shop-scout` — if you edit the operator here, re-copy and push from there (repo-local git identity already configured).
