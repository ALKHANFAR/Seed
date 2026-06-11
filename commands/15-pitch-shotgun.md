# /pitch-shotgun — Variant Exploration with Taste Memory

> Translation of gstack's `/design-shotgun` + `gstack-taste-update`. One answer
> means one perspective, and narrative is a taste game. You need to see options.

## The loop

1. Describe what you need: a one-liner, an opening 30 seconds, a "why now" slide,
   a cold-email hook, an answer to a specific objection.
2. The system reads brand/narrative constraints from `context/` and the target
   fund's playbook.
3. It generates **3 genuinely distinct variants** — different strategies, not
   different adjectives:
   - Variant A: traction-led ("numbers first, story second")
   - Variant B: insight-led ("the market is wrong about X")
   - Variant C: inevitability-led ("this happens with or without us; we're furthest ahead")
4. Side-by-side comparison with an honest note on what each prioritizes and trades off.
5. Founder approves one, remixes ("A's opening + C's close"), or requests a new round.
6. The approved variant is saved with an `approved.json`-style record: variant,
   context, target fund, date.

## Taste memory (the real magic)

Approvals and rejections are written to a persistent **taste profile** per company
and per fund — exactly like gstack's design taste learning:

- The founder consistently picks understated over hype → future variants bias
  understated. This isn't a setting; **it emerges from approvals.**
- STV's partner responded to the insight-led framing; Impact46's responded to
  traction-led → per-fund taste entries.
- **Decay: 5% per week.** What resonated in Q1's market mood is weaker evidence
  in Q3. Old taste fades unless re-confirmed by a new approval. Stale taste is
  worse than no taste.

## Founder-slop detection

gstack scans for AI slop (gradient heroes, 3-column icon grids, "clean modern UI").
The fundraising equivalents — auto-flagged in every variant before the founder
sees them:

- "Revolutionizing / disrupting / game-changing"
- "We have no competitors"
- "1% of a $X B market"
- "Uber for X" without an earned reason
- Hockey-stick charts with no labeled axes
- "World-class team" with no proof nouns
- Vision paragraphs where a number should be

Slop score A-F per variant. Anything below B is rewritten before presentation.

## Chaining

`/pitch-shotgun` picks the direction → `/investor-autoplan` builds the full
artifact from it → `/investor-qa` gates it. Shotgun decides taste; the pipeline
makes it real.
