# Investor Brain — Schema

> gbrain's lesson applied to fundraising: a self-wiring knowledge graph with typed
> pages and typed edges. Plain markdown files; the structure IS the intelligence.

## Page types (one folder per type)

```
brain/
├── funds/          one page per fund        (stv.md, impact46.md, shorooq.md…)
├── people/         one page per partner/analyst
├── meetings/       one page per meeting     (YYYY-MM-DD-fund-topic.md)
├── questions/      every question ever asked, with our best answer
├── objections/     every objection, with the 3-layer response
├── claims/         every investor-facing claim + tag + proof link
├── commitments/    everything we promised anyone, with deadline
└── theses/         our investment thesis versions (dated)
```

## Typed edges (write as wiki-links inside pages)

| Edge | Example |
|---|---|
| works_at | `[[people/sara]] works_at [[funds/stv]]` |
| attended | `[[people/sara]] attended [[meetings/2026-06-15-stv-intro]]` |
| asked | `[[meetings/...]] asked [[questions/unit-economics-voice-cost]]` |
| raised | `[[meetings/...]] raised [[objections/global-players-will-copy]]` |
| promised | `[[meetings/...]] promised [[commitments/send-financial-model]]` |
| supports | `[[data-room/...asset]] supports [[claims/no-show-reduction]]` |

## Page template (every page, top of file)

```yaml
---
type: fund | person | meeting | question | objection | claim | commitment | thesis
status: active | closed | stale
updated: YYYY-MM-DD
tags: []
---
```

## The synthesis rule (gbrain's killer feature, done manually or by an agent)
Before any meeting, an agent (or you) must be able to answer from these files alone:
"What do we know about this fund/person, what's open between us, and **what do we
NOT know yet**?" — the gap analysis is mandatory, not optional.
