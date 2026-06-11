# Presentation Layer

This folder packages TikTok Shop Product Scout for **Weekly Comp #7: The Operator**.

Competition context: the stated prize is a free seat in the Lyceum.

The operator itself lives in the root files. This layer explains the submission quickly, shows the business workflow, and gives a video or live-demo wrapper without changing the decision logic.

## Judge View

**Cohort:** Business

**Competition:** Weekly Comp #7: The Operator

**Position:** A folder-based AI operator that turns TikTok Shop product scouting from gut instinct into a governed **PROMOTE / SKIP / WATCHLIST** decision workflow.

**The point:** One folder takes a messy product signal and returns one decision. PROMOTE includes a ready-to-film script; SKIP logs the rule that killed it; WATCHLIST names the flip signal and re-check date. The TikTok Shop use case is the demo. The larger pattern is governed AI judgment: scoped identity, explicit rules, proof gates, memory discipline, and fixed output formats.

## Presentation Assets

| File | Use |
|---|---|
| `submission-hub.html` | Single target page with repo/operator links, walkthrough link, embedded README card, and heatless curlers YouTube production example |
| `animated-walkthrough.html` | Auto-playing animated PROMOTE-to-script workflow walkthrough for recording |
| `walkthrough-script.md` | 90-second captioned video or live narration script |
| `demo-run.md` | A concrete product input and expected governed output |
| `visual-direction.md` | Simple branding and screen/slide direction |

## Navigation Map

Use `submission-hub.html` as the start page.

| Destination | Path |
|---|---|
| Submission hub | `submission-hub.html` |
| Walkthrough | `animated-walkthrough.html` |
| Embedded README card | `submission-hub.html#operator-readme` |
| GitHub | `https://github.com/jordansshaw-pixel/tiktok-shop-scout/tree/main` |

## Recommended Submission Flow

1. Open with the creator problem: viral products create noisy business decisions.
2. Show the folder structure: identity, rules, reference files, output templates.
3. Run one product through the operator.
4. Show that the output is not advice; it is a business action.
5. Close with the reusable pattern: swap the audience profile, keep the governance path.

## Core Visual

```text
MESSY PRODUCT SIGNAL
        |
        v
DISQUALIFIERS -> SCORE -> THRESHOLD -> EDGE CASES
        |
        v
PROMOTE / SKIP / WATCHLIST
```

## Recording Recommendation

Open `animated-walkthrough.html` in a browser and record the page while it auto-plays. Use `walkthrough-script.md` as the narration track, or let the on-screen captions carry the story.

## Skool Submission Target

Use `submission-hub.html` as the single presentation target. It keeps the operator repo, animated walkthrough, and downstream video example in one place while preserving the scope boundary: the scout decides, scripts, and routes; downstream production happens after the operator.
