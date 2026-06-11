# Parallel Tracks — Running 10-15 Funds Like a Conductor

> From gstack's "10-15 parallel sprints" doctrine. One fund track is useful.
> Ten running at once is where the system becomes transformative — IF there is
> a process. Without process, ten tracks are ten sources of chaos.

---

## The doctrine

The sprint structure is what makes parallelism work. Each track knows exactly
what stage it is in and what to do next:

**Research → Thesis-fit → First meeting → Objections → Diligence → Partner meeting → Term sheet**

You manage tracks the way a CEO manages a team: **check in on the decisions that
matter, let the rest run.** The system surfaces only taste decisions; everything
mechanical (follow-up timing, dossier refresh, CRM hygiene) runs on rails.

### Track states

Every fund in `crm/pipeline` carries exactly one state. A track with no state is
a bug. A track that hasn't moved state in 14 days triggers a `/post-meeting-canary`
alert automatically.

### Momentum is the meta-strategy

Parallel tracks exist to create the only honest leverage a seed founder has:
**simultaneity.** Term sheets cluster when partner meetings cluster. Sequence the
pipeline so that 3-5 tracks hit partner-meeting stage in the same two-week window.
The system should flag when the pipeline is drifting into serial mode (one fund far
ahead of all others) — that's a negotiation-leverage bug, not a scheduling detail.

---

## Smart review routing

Just like a well-run startup: the CEO doesn't review infra fixes; design review
isn't needed for backend changes. Translated:

| Artifact changed | Required review | Informational |
|---|---|---|
| Master narrative / thesis | skeptical-vc + deck-doctor | closing-manager |
| Financial model | financial proof gate + skeptical-vc | — |
| Deck (visual/structure) | deck-doctor | skeptical-vc |
| Per-fund playbook | fund-specific agent only | — |
| Follow-up email | /careful check only | — |
| Data-room asset | claim gate | — |

The system tracks which reviews each artifact has passed and **does the smart
thing** — it never asks the founder to run the full gauntlet on a thank-you email,
and never lets a narrative change skip the skeptic.

---

## Send Readiness Dashboard

Before anything leaves the building, show the dashboard (gstack's Review Readiness
Dashboard, translated):

```
+====================================================================+
|                     SEND READINESS DASHBOARD                        |
+====================================================================+
| Gate              | Runs | Last Run         | Status   | Required  |
|-------------------|------|------------------|----------|-----------|
| Claim Gate        |  3   | 2026-06-09       | VERIFIED | YES       |
| /investor-qa      |  1   | 2026-06-10       | CLEAR    | YES       |
| Skeptical VC      |  1   | 2026-06-08       | CLEAR    | no        |
| Deck Doctor       |  0   | —                | —        | no        |
| /diligence-redteam|  1   | 2026-06-01       | 2 OPEN   | no        |
+--------------------------------------------------------------------+
| VERDICT: BLOCKED — /investor-qa stale (deck changed after last run) |
+====================================================================+
```

Claim Gate and `/investor-qa` are the only **blocking** gates (mirror of gstack
where Eng Review is the one required gate). Everything else is informational —
strongly recommended before partner meetings.

---

## Handoff protocol (from /browse handoff)

The system drives 90% of the round. But some moments are CAPTCHAs — they need
the human: a partner wants founder-to-founder dinner; a negotiation turns personal;
an angel needs a phone call, not an email.

When the system detects a stuck track (3 consecutive system-driven touches with
no movement), it **suggests handoff automatically**: it briefs the founder with
the full `[seed-context]` state, the founder takes the human action, says "done,"
and the system **resumes** — re-snapshots the deal state and continues the track.
Never let a track die in the gap between machine work and human work.
