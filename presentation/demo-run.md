# Demo Run

This demo is designed to show the operator making a governed decision, not just producing content ideas.

## Product Input

```text
Score this TikTok Shop product:

Product: 2026 Trendy Minimalist Elegant Women's Touchscreen Crossbody Phone Wallet
Price: $15.46
Category: women's accessories / phone wallet / crossbody bag
TikTok Shop signal: 4.4 rating, 17.4K sold, free shipping shown.
Seller: MeshMelt
Details: compact crossbody phone wallet with touchscreen phone pocket, adjustable strap, multiple card slots, coin/cash pouch, multiple color options, designed for errands, travel, shopping, gym, and daily use.
Commission: unknown.
Content angle: "I replaced my purse with this $15 phone wallet," phone-use-through-the-bag demo, what-fits-inside test, travel/errand outfit try-on.
Potential risk: product title is keyword-stuffed and seller quality should be checked through reviews/return policy.
```

## Expected Decision

The expected decision is **WATCHLIST**, not **PROMOTE**.

Reason: the product may score above the promotion threshold, but `rules.md` requires confirmed commission before a product can reach **PROMOTE**. Unknown commission must be estimated conservatively, and a high-scoring product with estimated commission becomes **WATCHLIST**.

## Expected Output

```markdown
## WATCH: 2026 Trendy Minimalist Elegant Women's Touchscreen Crossbody Phone Wallet - 21/30 on 2026-06-11

**Why not promoted:** commission unknown / estimated; `rules.md` section 3 only allows PROMOTE when commission is confirmed.
**Flip condition:** commission confirmed >= 8% within 7 days.
**Re-check date:** 2026-06-18
**If flipped:** promote with hook "I replaced my purse with this $15 phone wallet."
**If not flipped by re-check date:** move to rejection log, reason "watchlist expired"
```

## What This Demonstrates

- The operator does not chase viral-looking products blindly.
- Missing business data is visible, not hidden.
- The output creates a next action, not a vague recommendation.
- The same decision can be repeated because the rule path is documented.

