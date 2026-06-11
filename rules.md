# Rules — Decision Logic

Process every product in this order. Stop at the first section that produces a decision.

---

## §1. Hard disqualifiers — instant SKIP, no scoring

Check `reference/disqualifiers.md` first. If the product hits any of these, SKIP immediately and log the disqualifier. No score overrides a disqualifier.

1. **Ingestible supplements** or any product whose core benefit claim requires a medical outcome (cures, treats, weight-loss promises)
2. **Fake-spec risk electronics** — performance claims that can't be verified on camera (e.g., "military grade," unverifiable battery/mAh claims)
3. **One-time news-event products** — trending because of a single event, not a repeatable need
4. **No visual demo possible** — if the benefit can't be shown on camera in under 30 seconds, there is no video
5. **Earnings-claim products** — anything marketed as "make money with this"

---

## §2. Score the rubric

Score all six dimensions 1–5 using `reference/scoring-rubric.md`. Total range: 6–30.

| Dimension | What it measures |
|-----------|-----------------|
| Commission rate | Financial upside per sale |
| Sales velocity | Rising vs. peaked vs. declining |
| Creator saturation | Room left before the niche is crowded |
| Content angle | Does a scroll-stopping hook exist? |
| ICP fit | Match to `reference/audience-profile.md` |
| Price point | Conversion sweet spot vs. AOV floor |

**Missing data rule:** never stall on a missing field. Estimate it, label it `(est.)`, and score it one point lower than the estimate suggests. A product can only reach PROMOTE on confirmed commission data — see §3.

---

## §3. Decision thresholds

| Condition | Decision |
|-----------|----------|
| Score ≥ 18, commission **confirmed** | **PROMOTE** |
| Score ≥ 18, commission **estimated** | **WATCHLIST** — flip condition: confirm commission ≥ 8% within 7 days, then auto-promote |
| Score 14–17, and the weak dimensions are **volatile** (velocity, saturation) | **WATCHLIST** — name the exact signal that flips it (e.g., "creator count drops below 500" or "velocity turns from flat to rising") and a re-check date 14 days out |
| Score 14–17, and the weak dimensions are **structural** (angle, ICP fit, price) | **SKIP** — structure doesn't improve by waiting |
| Score < 14 | **SKIP** |

Volatile dimensions change week to week. Structural dimensions are properties of the product itself. A watchlist entry without a named flip condition and a date is not a decision — it's a deferral. Don't write one.

**Promote cap:** never more than 5 active PROMOTEs at once. If a 6th product qualifies, it must beat the lowest-scoring active promote, which moves to watchlist. Quality over volume.

---

## §4. Edge cases

**4.1 — Saturated but viral (>2000 creators, rising velocity).**
Default SKIP. Exception: PROMOTE only if commission ≥ 15% **and** you can name an angle that attacks a *different pain point* than the dominant videos use (check the top 5 videos for the product — if they all demo the same use, the second use case is the opening). If the angle is just "the same demo but mine," skip.

**4.2 — Under-$8 price (AOV floor).**
Default SKIP on price point 1. Exception: score price as a 3 if the listing sells in multi-packs or the product is naturally bought in multiples (e.g., hair clips, cable organizers) — cart value, not unit price, is what matters. Note the multi-buy assumption in the brief.

**4.3 — Seasonal spike.**
If rising velocity is driven by a season or holiday, count the days until the peak. Fewer than 14 days out: SKIP — by the time content ships and the algorithm picks it up, the wave is gone. 14+ days out: score velocity normally but add a hard post-by date to the brief.

**4.4 — Wellness-adjacent but demonstrable.**
Products like posture correctors, massage tools, or red-light wands are NOT auto-disqualified the way ingestibles are. The test: can the benefit be shown physically on camera without making a medical claim? If yes, PROMOTE is allowed — but the brief must constrain the angle to cosmetic/comfort language ("my shoulders felt looser," never "fixes back pain"). Write the allowed-claims line into the brief explicitly.

**4.5 — Previously decided product resubmitted.**
Check the rejection log and watchlist first. Re-score only if a volatile signal changed materially (creator count ±30%, velocity direction changed, commission rate changed). Otherwise restate the prior decision and its date — one line, done.

**4.6 — Conflicting signals in the listing itself.**
If the listing's stated commission contradicts the affiliate marketplace (or two sources disagree), use the **lower** figure for scoring and note the discrepancy. Optimistic data is how affiliates waste two weeks of content on a 3% product.

---

## §5. Output

Every decision uses the matching template in `reference/output-templates.md` — promote brief, skip log line, or watchlist entry. A decision without its template filled out is incomplete. The promote brief must pass the compliance checklist at the bottom of the template before it's considered done.

PROMOTE decisions additionally include a ready-to-film script generated from `reference/script-templates.md`. Identify the product category from the category ID table, then use the matching scaffold to produce a clean script with every placeholder filled. No brackets or placeholder text may remain in the output.

Script requirements:

- Target 120-160 words.
- Hard ceiling: 180 words for HeyGen API compatibility.
- The hook is the first sentence and must address a specific viewer pain point directly.
- The CTA is always last: `It's linked in my TikTok Shop. Tap the tag.` plus `#ad #TikTokShop` and two niche tags.
- Use observed, camera-demonstrable language only. No outcome promises.
- Apply the category compliance rules in `reference/script-templates.md`.
- Wellness-adjacent overrides beauty if both apply.
- Wellness and tech scripts must pass their mandatory compliance pre-checks before output.
