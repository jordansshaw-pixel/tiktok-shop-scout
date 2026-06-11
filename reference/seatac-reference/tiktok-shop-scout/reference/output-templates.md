# Output Templates

Every decision is delivered in one of these three formats. No freeform verdicts.

---

## PROMOTE — content brief

```markdown
## PROMOTE: [Product Name] — [score]/30

**Listing:** [URL or source]
**Commission:** [X% confirmed / X% (est.) — only confirmed reaches promote]
**Price:** $XX
**Post-by date:** [only if seasonal — rules.md §4.3; otherwise "none"]

| Dimension | Score | Note |
|-----------|-------|------|
| Commission | X | |
| Velocity | X | [the signal] |
| Saturation | X | ~XXX creators |
| Angle | X | |
| ICP fit | X | [trigger cited from audience-profile.md] |
| Price | X | |

**Hook:** "[the opening line/visual of the video — specific, not a theme]"
**Format:** [problem/solution | demo-with-result | POV | first-use reaction]
**Allowed claims:** [constraints from disqualifiers.md — esp. for wellness-adjacent products]

**Caption draft:**
[Hook line] [CTA — product tag]
#ad #TikTokShop [product tag] [niche tag]

**Compliance check:** [ ] #ad before the fold  [ ] native product tag, no 3rd-party link  [ ] no prohibited claims  [ ] price appears in video
```

A promote brief with an unchecked compliance box is not done.

---

## SKIP — rejection log entry

One line, appended to the rejection log:

```markdown
| [date] | [Product Name] | [score or "DQ"] | [the specific rule: e.g., "DQ#1 ingestible" or "16/30 — structural: no hook beats existing top videos (rules §3)"] |
```

---

## WATCHLIST — re-check entry

```markdown
## WATCH: [Product Name] — [score]/30 on [date]

**Why not promoted:** [the specific gap — e.g., "commission 10% (est.), unconfirmed"]
**Flip condition:** [the exact measurable signal — e.g., "commission confirmed ≥ 8%" or "creator count drops below 500"]
**Re-check date:** [date — max 14 days out]
**If flipped:** promote with hook "[carry the angle forward so it isn't re-derived]"
**If not flipped by re-check date:** move to rejection log, reason "watchlist expired"
```

A watchlist entry missing the flip condition or the expiry behavior is a deferral, not a decision — rewrite it.
