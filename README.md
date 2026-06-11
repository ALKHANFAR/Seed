# Seed — Investment Operating System

**Seed is a reusable, file-based operating system for closing a funding round.**
Generic in structure, specific in data. First user: **D10 Group (Sondos & Siyadah)**
raising Seed from investors such as STV, Impact46, and Shorooq.

Built on four distilled philosophies:
- **gstack** (Garry Tan) → named review agents + slash commands + a weekly loop
  + the deep layer: Boil-the-Ocean ethos, guardrails, Confusion Protocol,
  parallel tracks, taste memory (see `GSTACK_UPLIFT.md`)
- **gbrain** (Garry Tan) → typed institutional memory with gap analysis
- **Zolidar** → context/truth first; the deck is the last surface
- **Sequoia/Khosla + top deck benchmarks** → answer-first narrative, Action Titles

## The pipeline every piece of information travels
```
RAW INFO → CLAIM → PROOF GATE (VERIFIED/PARTIAL/MISSING) → SLIDE → /second-opinion
   → SEND READINESS DASHBOARD → /investor-send → /post-meeting-canary
   → /feedback-triage → LEARNING (brain)
   → (pass?)  /investigate-pass → (3 strikes?) narrative rebuild
   → (yes?)   /close-and-verify → MONEY IN ACCOUNT → 30-day canary
```
**No claim without a gate. No send without QA. No silence without a canary.
No pass without a root cause. No week without a retro. No lesson learned twice.**

## Map
```
core-os/         philosophy · operating loop · 10-dimensions rubric · fundraising
                 ethos · guardrails · confusion protocol & 3-strikes · parallel
                 tracks · proof discipline
brain/           the investor memory: funds, people, meetings, questions, objections,
                 claims, commitments, theses (schema + rules + templates)
                 + learnings.jsonl (compounding patterns, see learnings-spec.md)
commands/        19 runnable slash-commands (/investor-office-hours → /close-and-verify)
agents/          8 reviewer personas (skeptical-vc, deck-doctor, closing-manager…)
proof-gates/     claim · traction · technical · financial · team gates
                 + redteam exclusions (confirmed false positives)
context/         the truth engine: narrative, market, competition, financials, roadmap
company-layer/   D10 · Sondos · Siyadah profiles + master narrative + master prompt (AR)
playbooks/       per-fund playbooks (method + STV/Impact46/Shorooq skeletons)
pitch-factory/   deck outline (Action Titles) · one-liner · memo · objection ladder
deck/            REAL Slidev deck — `npm i && npm run dev`
data-room/       index · evidence map · metrics pack · questions log
crm/             pipeline · follow-up system · objection tracker
readiness/       term-sheet readiness score (/100, weekly) + funnel benchmarks
retros/          weekly fundraising retro template
GSTACK_UPLIFT.md the full gstack→fundraising translation table
```

## Start here
1. Read `core-os/00-philosophy.md`, `core-os/01-operating-loop.md`,
   then `core-os/03-fundraising-ethos.md` (the deep operating principles).
2. Fill `company-layer/` and `context/` with real data (everything marked ⟦DATA⟧).
3. Run `/investor-office-hours` (commands/) with any capable LLM → lock the thesis.
4. Build materials through `/investor-autoplan`. Nothing ships without `/investor-qa`
   — and nothing leaves the building without the Send Readiness Dashboard
   (`core-os/06-parallel-tracks.md`) showing all blocking gates green.
5. After every meeting: `/investor-learn` + start `/post-meeting-canary` cycles.
   On any pass or ghost: `/investigate-pass` before touching the narrative.
6. Run `/fundraising-retro` every week. Track `readiness/` to ≥80/100, then push
   for term sheets. Close through `/close-and-verify` — a verbal yes is a merged
   PR, not a deployed one.

## The ten dimensions (every output must pass)
Technical · Memory · Story · Team · Product · Operations · Moat · Scale · Impact · Return
— rubric in `core-os/02-ten-dimensions.md`.

## Reuse for any other company
Copy `company-layer/` + `context/`, replace the data, keep everything else.
Set the brain trust tier (read-write / read-only / deny) per
`brain/learnings-spec.md` so raises never cross-contaminate.
