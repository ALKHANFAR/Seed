# /investigate-pass — Root-Cause Analysis of a Pass or Ghost

> Translation of gstack's `/investigate`. Four phases: investigate, analyze,
> hypothesize, act. Use when a fund passes, goes cold, or a meeting "felt off."

## The Iron Law

**NO NARRATIVE FIXES WITHOUT ROOT-CAUSE INVESTIGATION FIRST.**

Fixing symptoms creates whack-a-mole fundraising. The founder who rewrites the
deck after every awkward meeting ends up with a Frankenstein narrative shaped by
the last skeptic in the room. Every fix that doesn't address the root cause makes
the next pass harder to diagnose. Find the root cause, then fix it.

On invocation: auto-`/freeze` to this fund's playbook. The global narrative is
untouchable until the investigation concludes.

---

## Phase 1: Root-Cause Investigation

Gather evidence before forming any hypothesis.

1. **Collect symptoms.** The exact wording of the pass (verbatim if possible),
   the moment in the meeting where energy dropped, which slide they lingered on,
   what they asked twice. If evidence is thin, ask the founder ONE question at
   a time — don't interrogate.
2. **Read the trail.** Trace the full touch history in the brain: every email,
   every question they asked, every artifact sent. Passes are usually visible
   in the questions two meetings earlier.
3. **Check recent changes.** Was this fund warm before? What changed between the
   warm signal and the cold one — a new metric we sent? A market event? A portfolio
   announcement on their side? **A regression means the root cause is in the diff.**
4. **Reproduce.** Can the objection be triggered deterministically? Run the same
   claim past the `skeptical-vc` agent. If the agent chokes on the same point,
   you have a reproducible bug. If not, gather more evidence.
5. **Check investigation history.** Search the brain for prior investigations on
   the same objection or the same fund profile. **Recurring passes on the same
   point are an architectural smell** — see the 3-Strikes Rule.

## Phase 2: Analyze — classify the root cause

Every pass has exactly one primary class:

| Class | Meaning | Correct response |
|---|---|---|
| **Thesis mismatch** | Fund structurally can't do this deal (stage, sector, geo, check size) | Not a bug. Mark the pipeline-qualification step that should have caught it. |
| **Narrative bug** | They misunderstood what we do | Fix the artifact that created the misunderstanding — not the whole deck. |
| **Proof gap** | They understood and didn't believe a claim | Route the claim back through the proof gate; build the evidence pack. |
| **Traction gap** | They believed everything and it's not enough yet | Strategy fact. Set a re-engage trigger ("come back at X MRR") in the CRM. |
| **People/trust** | Doubt about the team or a relationship dynamic | Handoff to founder — human problem, human fix. |
| **Timing/market** | Fund pacing, fund-of-fund pressure, macro | Log it; do not internalize it as a company flaw. |

## Phase 3: Hypothesize — one at a time

State the single most likely root cause and a falsifiable test for it:
*"Hypothesis: the pass was a proof gap on the retention claim. Test: did any other
fund question retention? Did the pass email mention metrics?"* Test, then move to
the next hypothesis. Never fix two hypotheses at once — you'll never know which
was real.

## Phase 4: Act

- Apply the **minimal** fix at the **correct layer** (artifact, claim, strategy, or pipeline-qualification).
- Write the learning to the brain with confidence score and source attribution.
- Send the graceful close + future-trigger note to the fund (a clean pass today is a warm door in 9 months).
- `/unfreeze` with justification.

## Stop condition

Three failed fix attempts on the same root cause → STOP. Escalate to narrative
architecture (`/investor-office-hours`). Do not thrash.
