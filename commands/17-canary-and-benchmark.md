# /post-meeting-canary & /funnel-benchmark

> Translations of gstack's `/canary` (post-deploy monitoring) and `/benchmark`
> (performance baselines). Deploying the pitch is not the end — it's when
> monitoring starts.

---

## /post-meeting-canary

After every meeting or send, the system watches the track for anomalies on a
schedule — exactly like canary cycles after a deploy:

```
Cycle 1 (24h):  Thank-you + promised materials sent? Their promised intro made?
Cycle 2 (72h):  Reply received? Deck opened (if trackable)? Any partner activity
                (LinkedIn views, mutual-contact pings)?
Cycle 3 (7d):   Movement or silence? Silence = console error. Alert raised.
Cycle 4 (14d):  No movement → track flagged STALLED. Suggest one value-add touch
                (a relevant metric milestone, a customer win — never "just
                checking in"), or trigger /investigate-pass.
```

Anomalies to alert on:
- A promised next step that passed its date (theirs or ours) — the #1 silent deal killer
- A question asked in the meeting that we never answered in writing
- Sudden tone change between touches (warm → formal)
- The fund announcing an investment in an adjacent/competing company (re-evaluate the track immediately)

Baselines: each fund's normal response latency is recorded. A fund that always
replies in 2 days going silent for 6 is a regression; a fund that always takes
a week is not. **Compare against baseline, not against your anxiety.**

---

## /funnel-benchmark

Establish baselines, then measure every narrative change against them. Real
measurements, not vibes:

```
Baseline (before deck v3):
  Cold/warm outreach → reply:        ⟦DATA⟧ %
  Reply → first meeting:             ⟦DATA⟧ %
  First meeting → second meeting:    ⟦DATA⟧ %   ← the Core Web Vital of fundraising
  Second meeting → partner meeting:  ⟦DATA⟧ %
  Median days between stages:        ⟦DATA⟧
  Objection frequency table:         top 5 with counts
```

Rules:
- **Multiple runs averaged.** One meeting after a deck change proves nothing;
  judge after 4-5 at the same stage.
- **Before/after on every material change.** Changed the one-liner? The opening?
  The ask? Benchmark the conversion delta or you're flying blind.
- **The metric that matters most is first → second meeting.** First meetings
  measure your network; second meetings measure your story.
- Trends persist in `readiness/` so `/fundraising-retro` can show whether the
  machine is actually improving week over week — gstack's "not vibes — data."
