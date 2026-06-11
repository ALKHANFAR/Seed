# /context-save & /context-restore — Never Lose Deal State

> Translation of gstack's `/context-save` / `/context-restore`. Fundraising runs
> in parallel with running the company. Sessions get interrupted for days.
> The state must survive the interruption — and survive a handoff to a co-founder.

## /context-save

Snapshot the entire working state to `brain/context-snapshots/⟦DATE⟧.md`:

```
# Context Snapshot — 2026-06-11

## Pipeline state (one line per active track)
STV        · partner-meeting scheduled 06-18 · owe: updated metrics pack
Impact46   · objection open (unit economics) · rebuttal drafted, NOT sent — needs /investor-qa
Shorooq    · canary cycle 3, silent 6d (baseline 2d) · /investigate-pass candidate

## Decisions made this session
- Held the ask at ⟦DATA⟧ despite second-opinion pressure (founder call; reasoning logged)
- Killed the "no competitors" framing globally

## Remaining work (ordered)
1. Re-gate the ARR claim after the May close numbers
2. STV metrics pack → /investor-send by 06-13
3. Run /diligence-redteam comprehensive (monthly, due)

## Failed approaches this session (do not retry)
- Traction-led opening for Shorooq — partner visibly disengaged; insight-led next time

## Open confusions (Confusion Protocol items awaiting founder)
- Strategic investor interest from ⟦DATA⟧: take the meeting or protect the round's shape?
```

## /context-restore

Reads the latest snapshot + the `[seed-context]` touch blocks since, and produces
a 60-second briefing: state, owed items, deadlines, open confusions. Works for:

- **You, two weeks later** after a product firefight.
- **Your co-founder**, taking a meeting you can't attend — full handoff, zero
  "wait, what did we tell them?"
- **A new session of any LLM** — the OS is host-agnostic, like gstack running
  on 10 different agents. The state lives in files, not in anyone's memory.

Rule: restore NEVER mutates outbound material. It briefs; the founder acts.
