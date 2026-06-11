# Learnings — Compounding Institutional Memory

> Translation of gstack's `/learn`, domain-skills (per-site notes), and gbrain
> trust tiers. The brain already stores facts (funds, people, meetings). This
> layer stores **learned patterns** — and makes every other command smarter
> automatically.

## The learnings file

`brain/learnings.jsonl` — one JSON line per learning:

```json
{"ts":"2026-06-10","type":"pattern","confidence":9,
 "text":"Saudi seed funds always ask about Saudization plan in meeting 2, never meeting 1",
 "source":"meetings: STV-2026-05-12, Impact46-2026-05-28","refs":["playbooks/stv","playbooks/impact46"]}
{"ts":"2026-06-08","type":"pitfall","confidence":8,
 "text":"Leading with the two-product structure costs 10 minutes of every first meeting — lead with D10 umbrella, reveal structure only if asked",
 "source":"/investigate-pass run 2026-06-07","refs":["company-layer/master-narrative"]}
{"ts":"2026-05-20","type":"preference","confidence":7,
 "text":"Founder prefers understated tone; rejected all hype variants in 3 shotgun rounds",
 "source":"/pitch-shotgun approvals","refs":["pitch-factory/"]}
```

Rules (straight from gstack):
- Every learning carries a **confidence score**, **source attribution**, and the
  files it references.
- Other commands **automatically search learnings before recommending**, and
  display `Prior learning applied:` when one is used. The system gets smarter on
  YOUR round over time — that's the compounding.
- **Prune:** learnings whose referenced artifacts no longer exist are flagged
  stale and offered for pruning. A learning about deck v1 may be poison for deck v4.
- **Export:** learnings can be exported for the co-founder / the next raise.

## Per-fund micro-notes (domain skills)

gstack's browser saves per-site notes ("LinkedIn's Apply button lives in an
iframe") that auto-fire on the next visit. Translated — **per-fund micro-notes**
that auto-load whenever that fund's track is touched:

```
fund: stv
note: "Partner X reads the memo before the deck — always send memo first."
status: quarantined   # becomes ACTIVE after confirmed useful 3 times
```

- New notes are **quarantined** → promoted to **active** after 3 confirmed uses
  (prevents one-off impressions from becoming false doctrine).
- Notes proven across multiple funds get **promoted to global** learnings
  (e.g., "memo-before-deck" turns out to be true for most KSA funds).

## Trust tiers (gbrain's read-write / read-only / deny)

When this OS is reused for another company (the README's reuse path), each
company's brain gets a trust tier:

- **read-write** — the active raise: search and write learnings.
- **read-only** — past raises / other portfolio companies: searchable for
  patterns, never contaminated with the current company's data.
- **deny** — confidential engagements: no interaction at all.

This is how one operator runs multiple raises without cross-contaminating
institutional memory — gstack's multi-client consultant pattern, verbatim.
