# Commands — The Investor Stack

Each file is a **runnable prompt**: paste it (plus the referenced inputs) into any
capable LLM, or wire them as slash-commands in Claude Code / your agent platform.
They mirror gstack's sprint: every command's output feeds the next.

## The sprint (Think → Plan → Build → Review → Send → Monitor → Learn)

```
/investor-office-hours    → thesis & framing          (gstack /office-hours)
/deal-ceo-review          → challenge the deal        (gstack /plan-ceo-review)
/investor-autoplan        → run the full pipeline     (gstack /autoplan)
/pitch-shotgun            → narrative variants +      (gstack /design-shotgun
                            taste memory                + taste learning)
/deck-review              → fix the deck              (gstack /design-review)
/diligence-review         → technical DD readiness    (gstack /plan-eng-review)
/financial-review         → model & unit economics
/moat-review              → defensibility audit
/investor-qa              → skeptical-VC attack       (gstack /qa)
/second-opinion           → blind cross-model review  (gstack /codex)
/diligence-redteam        → kill-scenario audit       (gstack /cso)
/investor-send            → gates + version + send    (gstack /ship)
/investor-package         → final gate + package      (gstack /ship)
/post-meeting-canary      → 24h/72h/7d/14d monitoring (gstack /canary)
/funnel-benchmark         → conversion baselines      (gstack /benchmark)
/feedback-triage          → VALID/FIXED/FP triage     (gstack Greptile layer)
/investigate-pass         → root cause of a pass      (gstack /investigate)
/close-and-verify         → term sheet → money in     (gstack /land-and-deploy)
/context-save · /context-restore → deal-state snapshots (gstack same)
/fundraising-retro        → weekly loop               (gstack /retro)
/investor-learn           → update the Brain          (gstack /learn)
```

File index: numbered files (`12-…` → `19-…`) are the gstack-uplift commands;
named files are the original eleven. One registry, one sprint.

## Order rules (non-negotiable)

- Never `/investor-package` or `/investor-send` without `/investor-qa` first.
- Never send to a fund with no playbook — `/investor-send` bootstraps one (see 16).
- Every send starts a `/post-meeting-canary`. Every pass triggers `/investigate-pass`.
- Three failed rebuttals on the same objection → stop wording, rebuild narrative
  (`core-os/05-confusion-protocol-and-3-strikes.md`).
- All sends pass the Send Readiness Dashboard (`core-os/06-parallel-tracks.md`).
- Destructive actions (valuation in writing, cap table, exclusivity) hit /careful
  warnings first (`core-os/04-guardrails.md`).
