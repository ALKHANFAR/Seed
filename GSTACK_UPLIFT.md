# GSTACK UPLIFT — Everything Else From gstack, Translated

> Seed was built on gstack's surface (named agents, slash commands, weekly loop).
> This uplift imports the rest: the deep ethos, the meta-protocols, and 9 skills
> that had no fundraising equivalent yet. Drop these files into the repo as-is.

## The full translation table (programming → fundraising)

| gstack concept | Seed translation | File |
|---|---|---|
| ETHOS: Boil the Ocean | Boil the Ocean of Proof — completeness is cheap now; score it X/10 | core-os/03 |
| ETHOS: Search Before Building | Search Before Pitching — 3 Layers of Knowledge, Eureka Moments | core-os/03 |
| ETHOS: User Sovereignty | Founder Sovereignty — models recommend, founder decides, AI never sends | core-os/03 |
| Compression table (100x boilerplate) | Compression table for fundraising tasks | core-os/03 |
| /careful (rm -rf, DROP TABLE warnings) | Destructive-send patterns table + one-way/two-way doors | core-os/04 |
| /freeze (edit lock to one dir) | Scope lock to one fund's playbook during a crisis | core-os/04 |
| /guard | Full safety mode for negotiations + post-meeting 48h | core-os/04 |
| Confusion Protocol | STOP on high-stakes ambiguity: name it, 2-3 options, ask | core-os/05 |
| 3-failed-fixes → question architecture | 3 failed rebuttals → question the narrative, not the wording | core-os/05 |
| Continuous checkpoint (WIP + [gstack-context]) | Same-day touch logging with [seed-context] blocks | core-os/05 |
| 10-15 parallel sprints (Conductor) | 10-15 parallel fund tracks; simultaneity = leverage | core-os/06 |
| Smart review routing | Per-artifact gate routing (don't run the gauntlet on a thank-you) | core-os/06 |
| Review Readiness Dashboard | Send Readiness Dashboard with blocking vs informational gates | core-os/06 |
| Browser handoff (CAPTCHA → human → resume) | Stuck-track handoff to founder → resume | core-os/06 |
| /investigate (Iron Law, 4 phases) | /investigate-pass — root cause of passes/ghosts, pass taxonomy | commands/12 |
| /cso (OWASP+STRIDE, 8/10 gate, exploit scenarios) | /diligence-redteam — fundraising OWASP 10, kill scenarios, FP exclusions | commands/13 |
| /codex (second opinion, cross-model overlap) | /second-opinion — blind dual review; overlap = truth | commands/14 |
| /design-shotgun + taste memory (5%/wk decay) | /pitch-shotgun — 3 strategy variants, taste profiles per fund, decay | commands/15 |
| AI-slop detection | Founder-slop detection (revolutionizing, 1%-of-TAM, no-competitors) | commands/15 |
| /ship (sync, test, version, PR; test bootstrap) | /investor-send — sync truth, run gates, version, send; playbook bootstrap | commands/16 |
| /land-and-deploy (merge→deploy→verify) | /close-and-verify — term sheet → docs → MONEY IN ACCOUNT → 30d canary | commands/16 |
| /canary (post-deploy monitoring cycles) | /post-meeting-canary — 24h/72h/7d/14d cycles vs per-fund baselines | commands/17 |
| /benchmark (Core Web Vitals baselines) | /funnel-benchmark — meeting-conversion baselines; before/after every change | commands/17 |
| Greptile triage (VALID/FIXED/FP + batting avg) | /feedback-triage — advisor feedback triage + advisor batting average | commands/18 |
| /context-save + /context-restore | Deal-state snapshots + 60-second briefings, co-founder handoffs | commands/19 |
| /learn (confidence, attribution, prune) | brain/learnings.jsonl — auto-applied prior learnings, pruning, export | brain/learnings-spec |
| Domain skills (quarantine → active after 3 uses) | Per-fund micro-notes with quarantine promotion | brain/learnings-spec |
| gbrain trust tiers (rw/ro/deny) | Per-company brain trust tiers for OS reuse | brain/learnings-spec |

## Updated pipeline (was: RAW INFO → … → DATA-ROOM ASSET)

```
RAW INFO → CLAIM → PROOF GATE → SLIDE → /second-opinion → SEND READINESS DASHBOARD
   → /investor-send → /post-meeting-canary → /feedback-triage → LEARNING (brain)
   → (pass?) /investigate-pass → (3 strikes?) narrative rebuild
   → (yes?) /close-and-verify → MONEY IN ACCOUNT → 30-day canary
```

**No claim without a gate. No send without QA. No silence without a canary.
No pass without a root cause. No week without a retro. No lesson learned twice.**

## Voice triggers (from gstack's voice-friendly aliases)

Say it naturally — the right command activates:
- "why did they pass" / "ليش انسحبوا" → /investigate-pass
- "attack my deck" / "اهجم على العرض" → /diligence-redteam
- "show me options" / "أعطني نسخ" → /pitch-shotgun
- "is it ready to send" / "جاهز للإرسال؟" → Send Readiness Dashboard
- "where were we" / "وين وقفنا" → /context-restore
- "be careful" / "انتبه" → /careful

## Install

Copy these folders into the repo root (paths match Seed's existing map):

```
core-os/03-fundraising-ethos.md
core-os/04-guardrails.md
core-os/05-confusion-protocol-and-3-strikes.md
core-os/06-parallel-tracks.md
commands/12-investigate-pass.md
commands/13-diligence-redteam.md
commands/14-second-opinion.md
commands/15-pitch-shotgun.md
commands/16-investor-send-and-close.md
commands/17-canary-and-benchmark.md
commands/18-feedback-triage.md
commands/19-context-save-restore.md
brain/learnings-spec.md
```

Then update README's command count (11 → 19) and add the ethos to `00_START_HERE.md`
step 1: read `core-os/03-fundraising-ethos.md` before anything else.
