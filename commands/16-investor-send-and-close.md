# /investor-send & /close-and-verify — The Last Mile

> Translation of gstack's `/ship` and `/land-and-deploy`. "A lot of branches die
> when the interesting work is done and only the boring release work is left.
> Humans procrastinate that part. AI should not." A lot of **deals** die the same
> way — after the great meeting, in the boring follow-through.

---

## /investor-send — the release engineer

For a ready artifact, not for deciding what to build. Stop brainstorming; execute:

1. **Sync with truth.** Re-check every number in the artifact against the current
   `context/` and metrics pack. Anything that drifted since the artifact was
   drafted gets updated or flagged. (= sync main)
2. **Run the gates.** Claim gate + `/investor-qa` + `/careful` destructive-pattern
   scan. (= run tests)
3. **Check the Send Readiness Dashboard.** Blocking gates must be green. If the
   skeptical-vc review is missing, ask — but don't hard-block (mirror of gstack's
   review gate). Decisions are saved per artifact so the founder is never re-asked.
4. **Versioning.** Stamp the artifact (deck v3.2, metrics pack 2026-06). A fund
   must never hold two unlabeled versions of the same document. (= changelog)
5. **Send + log.** The touch is committed to the brain with a `[seed-context]`
   block, CRM state advances, follow-up timer starts.

### Bootstrap rule (from /ship's test bootstrap)

If the target fund has **no playbook yet**, `/investor-send` refuses to send and
bootstraps one first: thesis research, portfolio scan, partner dossier, 5 likely
objections. Sending into a fund with zero playbook is deploying with no tests.

---

## /close-and-verify — from "approved" to "verified in production"

`/investor-send` gets the yes-energy. `/close-and-verify` finishes the job —
because **a verbal yes is a merged PR, not a deployed one.**

The pipeline after a term sheet / verbal commitment:

1. **Merge:** term sheet reviewed (counsel = CI), signed.
2. **Deploy:** definitive docs, conditions precedent checklist, KYC, board consents.
3. **Health check:** money in the account. That is the ONLY green status.
4. **Canary:** first 30 days post-close — investor onboarding, first update sent,
   information rights satisfied. A closed investor who feels ignored in month one
   is a production incident waiting for the Series A.

First run walks through a dry-run of the closing checklist with counsel before
anything irreversible. After that, it trusts the config and runs straight through.

If the close breaks (re-trade, stalled docs, a condition that can't be met), it
reports exactly what failed and whether to roll back — i.e., re-open parallel
tracks immediately. **Never let the pipeline go serial on an unverified close.**
