# Commands — The Investor Stack

Each file is a **runnable prompt**: paste it (plus the referenced inputs) into any
capable LLM, or wire them as slash-commands in Claude Code / your agent platform.
They mirror gstack's sprint: every command's output feeds the next.

```
/investor-office-hours  → thesis & framing       (gstack /office-hours)
/deal-ceo-review        → challenge the deal     (gstack /plan-ceo-review)
/investor-autoplan      → run the full pipeline  (gstack /autoplan)
/deck-review            → fix the deck           (gstack /design-review)
/diligence-review       → technical DD readiness (gstack /plan-eng-review)
/financial-review       → model & unit economics
/moat-review            → defensibility audit
/investor-qa            → skeptical-VC attack    (gstack /qa)
/investor-package       → final gate + send      (gstack /ship)
/fundraising-retro      → weekly loop            (gstack /retro)
/investor-learn         → update the Brain       (gstack /learn)
```
Order matters. Never `/investor-package` without `/investor-qa` first.
