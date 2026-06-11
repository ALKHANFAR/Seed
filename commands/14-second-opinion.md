# /second-opinion — Cross-Model Review

> Translation of gstack's `/codex`. Different model, different training, different
> blind spots. The overlap tells you what's definitely real. The unique findings
> are where you find the deal-killers neither reviewer catches alone.

## The principle: two doctors, same patient

Run the same artifact (deck, memo, objection rebuttal, term-sheet summary) through
a **completely independent** second reviewer — a different LLM, or a human advisor
given zero context about the first review. The second review must be blind: it
never sees the first reviewer's findings.

## Three modes

**Review** — independent pass/fail. The second model reads the artifact cold,
classifies findings P1 (deal-killer) / P2 (credibility risk) / P3 (polish), and
returns a verdict. **Any P1 = FAIL = artifact does not ship.**

**Challenge** — adversarial mode at maximum effort. The second model role-plays
the most hostile partner in the target fund and actively tries to break the
narrative: edge cases in the model, assumptions that fail under questioning, the
one comparison to a portfolio company that embarrasses you. A penetration test
for your story.

**Consult** — open conversation with session continuity. "Am I thinking about
the round structure correctly?" Follow-ups keep context. For strategy moments,
not artifact gates.

## Cross-model analysis

When both the in-house review (skeptical-vc agent) and /second-opinion have run
on the same artifact:

```
OVERLAP (high confidence — fix immediately):
  Both flagged the GCC TAM derivation as unsupported.

UNIQUE TO SECOND OPINION (blind spot of reviewer 1):
  The "no real competitors" framing reads as naivety to anyone who knows
  the regional CCaaS market.

UNIQUE TO IN-HOUSE (blind spot of reviewer 2):
  Slide 9's cohort chart contradicts the metrics pack.
```

Overlap = ground truth. Unique findings = exactly why you run two reviewers.

## Founder Sovereignty applies

When both reviewers agree on a change that alters the founder's stated direction
(drop the valuation, cut a product line from the story, change the lead-investor
target): **present the recommendation, explain why both reviewers believe it,
state what context the models might be missing, and ask. Never act.**
Agreement is signal, not proof.
