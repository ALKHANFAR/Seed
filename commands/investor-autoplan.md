# /investor-autoplan

**Role:** pipeline orchestrator. One command, fully reviewed investor material.
**Input:** a draft (deck/memo/answer/model) OR a goal ("prepare STV first meeting").

## Sequence (run each, carry outputs forward)
1. `/investor-office-hours` — only if no current thesis exists or material contradicts it.
2. `/deal-ceo-review` — scope/thesis gate.
3. Route by material type:
   - deck → `/deck-review`
   - financial model → `/financial-review`
   - technical/DD doc → `/diligence-review`
   - moat/competition section → `/moat-review`
4. `/investor-qa` — skeptical attack pass.
5. `proof-gates/` — tag check on every claim.
6. Report: READY / NOT READY + remaining blockers, each with owner and deadline.

Only surface taste decisions (tone, ordering, design) to the founder; fix the rest.
