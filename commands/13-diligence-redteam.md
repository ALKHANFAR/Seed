# /diligence-redteam — Chief Skeptic Officer

> Translation of gstack's `/cso` (OWASP + STRIDE, zero-noise, 8/10 confidence gate,
> concrete exploit scenario per finding). This is the audit that finds what kills
> the deal in diligence — before the associate does.

## Two modes (exactly like /cso)

- **Daily / pre-send (zero-noise):** only findings with confidence ≥ 8/10 are
  reported. No nitpicks, no maybes. If it's flagged, it's real. Run before any
  partner meeting or data-room share.
- **Comprehensive (monthly deep scan):** confidence bar drops to 2/10; everything
  surfaces. Run monthly and before opening the data room to a lead.

Trend tracking across runs: findings open/closed per week feed the `readiness/`
score. A finding that survives two comprehensive scans is escalated to the founder
as a structural risk.

## The threat model — "OWASP Top 10 of Fundraising"

What an associate, an analyst, or a rival founder whispering in the partner's ear
will attack:

1. **Claim injection** — a number in the deck that doesn't reconcile with the data
   room. (The #1 deal-killer. One inconsistency triggers a full re-audit.)
2. **Broken provenance** — "ARR" that includes one-time revenue; "users" that means
   signups; a logo on the customer slide that's actually a pilot.
3. **Sensitive exposure** — anything in the data room that shouldn't be there yet
   (cap-table drama, churn cohort you didn't mention, legal threads).
4. **Cross-entity confusion** — Sondos vs Siyadah vs D10: revenue, costs, IP, and
   contracts must map cleanly to entities. Holding-structure ambiguity = diligence quicksand.
5. **Broken access control** — who has the deck? Forwarded teasers with stale
   numbers circulating is a live vulnerability.
6. **Dependency supply chain** — concentration risk: top customer %, single
   channel, key-person dependency, one cloud vendor, regulatory single point of failure.
7. **Stale components** — outdated market sizing, dead competitor cited as alive,
   a regulation that changed last quarter.
8. **Insufficient logging** — claims with no audit trail. "Where did this 40% number
   come from?" must have a one-click answer in the evidence map.
9. **Privilege escalation** — promises made in meetings that exceed what the
   artifacts support ("we can be profitable by Q4" said verbally, supported nowhere).
10. **Denial of service** — the founder as bottleneck: questions that take >48h to
    answer kill momentum. Pre-compute the standard 30 diligence answers.

## Finding format — the kill scenario

Every finding ships with severity, evidence, **and a concrete kill scenario** —
exactly like /cso's "concrete exploit scenario":

```
CRITICAL · confidence 9/10
Finding: Deck slide 7 says "SAR 2.1M ARR"; metrics pack shows SAR 1.7M recurring
         + SAR 0.4M one-time implementation fees.
Kill scenario: STV associate reconciles the two during diligence week, flags it
         to the partner as "metric inflation." Partner doesn't accuse you — he
         just lets the process quietly stall. You never learn why.
Fix: Re-gate the claim. Slide says "SAR 2.1M revenue run-rate (1.7M recurring)."
         Update the evidence map. Re-run /investor-qa.
```

## False-positive discipline (zero-noise)

Like /cso's 17 FP exclusions: maintain `proof-gates/redteam-exclusions.md` —
patterns confirmed as non-issues (e.g., "pilot revenue counted separately and
labeled" is fine once labeled). Confirmed FPs are auto-skipped in future runs,
and the red team's batting average is tracked in `/fundraising-retro`.
