# Guardrails — /careful · /freeze · /guard for Fundraising

> Translated from gstack's safety skills. In code, the destructive commands are
> `rm -rf` and `DROP TABLE`. In fundraising, they are emails. The principle is
> identical: **accident prevention, not access control.** Every warning can be
> overridden by the founder — but never silently skipped by the system.

---

## /careful — Destructive Action Warnings

When active (default: always active during a live round), every outbound action
is checked against known-destructive patterns **before it goes out**. A match
triggers a STOP + explicit founder confirmation.

### The destructive patterns table

| Pattern | Code equivalent | Risk |
|---|---|---|
| Putting a specific valuation in writing before a partner meeting | `git push --force` | Anchors the negotiation; can't be unsent |
| Emailing two partners at the same fund in parallel | race condition | Signals disorganization; partners compare notes |
| Sharing the full cap table / ESOP detail pre-term-sheet | `DROP TABLE` | Leaks leverage; invites re-trading |
| Naming other funds in the process ("X is also looking") without proof | bad trust boundary | One phone call exposes the bluff; credibility loss is permanent |
| Sending an updated metric that contradicts a previously sent number | history rewrite | Triggers a full re-audit of every claim |
| Agreeing to exclusivity / no-shop verbally in a meeting | `git reset --hard` | Discards all parallel-track work |
| Forwarding one fund's questions or term sheet to another fund | data exfiltration | Reputation damage across the whole ecosystem |
| Sending any artifact that has not passed `/investor-qa` | deploying without CI | Unverified claims reach a professional skeptic |
| Replying to a hard objection within minutes, emotionally | hotfix in prod | The fast answer is rarely the gated answer |
| Accepting a "small" term (board seat, liquidation pref) in chat | silent schema migration | One-way door disguised as a detail |

### Safe exceptions (whitelisted — no warning)

- Sending the standard teaser / one-liner to a new fund
- Scheduling messages, thank-you notes, logistics
- Sharing artifacts already stamped VERIFIED by the proof gates
- Updating the CRM, brain, or internal files (internal = always safe)

### One-way vs two-way doors

Before any irreversible step, classify it:
- **Two-way door** (can be walked back: a meeting, a teaser, a follow-up) → proceed, log it.
- **One-way door** (valuation in writing, exclusivity, term acceptance, naming names)
  → STOP. Present the decision, the downside scenario, and 2-3 alternatives. Founder decides.

---

## /freeze — Scope Lock

In code: lock edits to one directory while debugging so the agent can't "fix"
unrelated files. In fundraising: **lock work to one fund's track while handling
a crisis in it.**

When a deal is wobbling (gone cold, hard objection, diligence problem):

```
/freeze playbooks/stv/
```

Effect: no edits to the master narrative, the deck, the financial model, or any
other fund's playbook until the investigation completes. **A single skeptical
partner must never cause panic-edits to the global story.** What one fund
disliked, another may fund. Fix the global narrative only when `/investigate-pass`
proves the root cause is global.

`/investigate-pass` auto-activates freeze on the fund being investigated.

---

## /guard — Full Safety Mode

`/careful` + `/freeze` in one command. Activate during:
- live term-sheet negotiation
- the 48 hours after a partner meeting (highest-risk window for over-eager follow-ups)
- any week where the founder is exhausted (fatigue is when destructive sends happen)

---

## /unfreeze

Removes the scope lock. Requires one line of justification logged to the brain:
*why is it now safe to touch the global narrative?*
