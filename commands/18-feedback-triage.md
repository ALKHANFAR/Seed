# /feedback-triage — Triage External Feedback Like Greptile Comments

> Translation of gstack's Greptile integration. The problem with any external
> reviewer — advisors, angels, friendly VCs, accelerator mentors — is triage.
> Some feedback is gold. Some is a false positive. Without a triage layer, the
> comments pile up, the founder rewrites the deck after every coffee chat, and
> the narrative turns to mush.

## The classification (every piece of feedback gets exactly one)

**[VALID]** — a real issue. Goes into the findings list, gets fixed before the
next send, and the fix is logged. Reply to the source acknowledging the catch
(this trains your advisors to keep giving you signal).

**[ALREADY FIXED]** — caught previously, fixed in artifact vN. Auto-reply with
the fix ("good catch — addressed in the current version, here it is"). Costs
nothing, builds the relationship.

**[FALSE POSITIVE]** — feedback that's wrong for your case: advice from a
different stage ("you need a CFO" at pre-seed), a different market (US dynamics
applied to KSA), or taste presented as law. **Push back politely with reasoning**
— founder confirms first, then a reply goes out explaining why. Never silently
ignore (kills the relationship) and never silently comply (kills the narrative).

## Learning from history — the batting average

Every confirmed false positive is saved to `brain/feedback-history.md` with the
source. Effects:

1. **Auto-skip:** known FP patterns from that source are pre-classified in future
   rounds of feedback.
2. **Batting average:** `/fundraising-retro` tracks each advisor's hit rate over
   time. The advisor whose feedback is 80% VALID gets pulled closer to the round.
   The one at 20% gets thanked warmly and weighted accordingly.
3. **Cross-source overlap:** when two independent sources flag the same thing,
   it's auto-escalated to VALID-CRITICAL — same logic as cross-model overlap
   in /second-opinion.

## The two-layer review

External feedback arrives asynchronously (the Greptile layer). `/investor-qa`
and `/investor-send` are feedback-aware: before any send, they pull untriaged
feedback, classify it, fix the VALIDs, and reply to the rest. **Nothing falls
through the cracks, and nothing hijacks the narrative.**

Total extra time per send: about 5 minutes. Total saved: your story's coherence.
