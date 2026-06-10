# Seed — Investment Operating System

**Seed is a reusable, file-based operating system for closing a funding round.**
Generic in structure, specific in data. First user: **D10 Group (Sondos & Siyadah)**
raising Seed from investors such as STV, Impact46, and Shorooq.

Built on four distilled philosophies:
- **gstack** (Garry Tan) → named review agents + slash commands + a weekly loop
- **gbrain** (Garry Tan) → typed institutional memory with gap analysis
- **Zolidar** → context/truth first; the deck is the last surface
- **Sequoia/Khosla + top deck benchmarks** → answer-first narrative, Action Titles

## The pipeline every piece of information travels
```
RAW INFO → CLAIM → PROOF GATE (VERIFIED/PARTIAL/MISSING) → SLIDE → INVESTOR ANSWER → DATA-ROOM ASSET
```
**No claim without a gate. No send without QA. No week without a retro.**

## Map
```
core-os/         philosophy · operating loop · 10-dimensions rubric · proof discipline
brain/           the investor memory: funds, people, meetings, questions, objections,
                 claims, commitments, theses (schema + rules + templates)
commands/        11 runnable slash-commands (/investor-office-hours → /investor-package)
agents/          8 reviewer personas (skeptical-vc, deck-doctor, closing-manager…)
proof-gates/     claim · traction · technical · financial · team gates
context/         the truth engine: narrative, market, competition, financials, roadmap
company-layer/   D10 · Sondos · Siyadah profiles + master narrative + master prompt (AR)
playbooks/       per-fund playbooks (method + STV/Impact46/Shorooq skeletons)
pitch-factory/   deck outline (Action Titles) · one-liner · memo · objection ladder
deck/            REAL Slidev deck — `npm i && npm run dev`
data-room/       index · evidence map · metrics pack · questions log
crm/             pipeline · follow-up system · objection tracker
readiness/       term-sheet readiness score (/100, weekly)
retros/          weekly fundraising retro template
```

## Start here
1. Read `core-os/00-philosophy.md` then `core-os/01-operating-loop.md`.
2. Fill `company-layer/` and `context/` with real data (everything marked ⟦DATA⟧).
3. Run `/investor-office-hours` (commands/) with any capable LLM → lock the thesis.
4. Build materials through `/investor-autoplan`. Nothing ships without `/investor-qa`.
5. Run `/fundraising-retro` every week. Track `readiness/` to ≥80/100, then push for term sheets.

## The ten dimensions (every output must pass)
Technical · Memory · Story · Team · Product · Operations · Moat · Scale · Impact · Return
— rubric in `core-os/02-ten-dimensions.md`.

## Reuse for any other company
Copy `company-layer/` + `context/`, replace the data, keep everything else.
