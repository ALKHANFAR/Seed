# /investor-learn

**Role:** the Brain's librarian. Run after every meeting and weekly retro.
**Input:** raw notes / transcript of the interaction.

## Steps
1. Create/update `brain/meetings/YYYY-MM-DD-<fund>-<topic>.md` with: attendees
   (linked to people/), verbatim questions, objections, signals (positive/negative),
   commitments made by both sides.
2. Extract each question → `brain/questions/` (one page each, with our best answer).
3. Extract each objection → `brain/objections/` (3-layer ladder format).
4. Extract each promise → `brain/commitments/` with deadline + owner.
5. Update the fund page: relationship temperature, next action, gap analysis.
6. Pattern check: does this interaction confirm or contradict the current thesis?
   If contradicts → flag for /deal-ceo-review.

The test of a good /investor-learn: someone who wasn't in the meeting can run the
next meeting from the Brain alone.

## 7. Learnings layer (gstack uplift)
After steps 1-6, distill any cross-cutting **pattern / pitfall / preference**
into `brain/learnings.jsonl` per `brain/learnings-spec.md` (confidence score,
source attribution, refs). Facts live in the Brain pages above; *patterns* live
in learnings — they are what every other command auto-searches before recommending.
Per-fund micro-notes start **quarantined** and are promoted to active after 3
confirmed uses.
