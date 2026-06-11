# D10 Ammunition Extract — Investor Truth Baseline

> Original extraction: 2026-06-10 from siyadah-ai-os archive.  
> Updated: 2026-06-11 after current financial model, founder customer list, old Sondos dashboard review, and enterprise pipeline clarification.  
> Every investor-facing claim must carry a gate: **VERIFIED / PARTIAL / MISSING / SUPERSEDED**.  
> **Important clarification:** Current MRR means monthly-equivalent current revenue. شركة تقدير is a **12,900 SAR annual contract**, so its MRR-equivalent is **1,075 SAR**, not 12,900 SAR monthly.  
> **Pipeline clarification:** The old `Sondos Ai dashborad` file is historical pipeline evidence. It shows many trials and campaigns, not current paying customers.  
> **Enterprise pipeline clarification:** SAICO is a pipeline opportunity worth **57,000 SAR/month** and **684,000 SAR/year**, but it is not counted in MRR/ARR yet.

---

## 0) Current source of truth — finance

**Authoritative current file:** `company-layer/FINANCIAL_TRUTH_PACK_2026-06-11.md`

Current finance numbers supersede all older deck/Mem/April-file/dashboard numbers.

| Metric | Current value | Gate |
|---|---:|---|
| Active revenue customers | 4 | PARTIAL — needs evidence linked |
| Current MRR | 28,966.5 SAR | PARTIAL — includes تقدير as annual-contract MRR equivalent |
| Current ARR | 347,598 SAR | PARTIAL — 28,966.5 x 12 |
| ARPU | 7,241.625 SAR | PARTIAL — 28,966.5 / 4 customers |
| Collected revenue, last 6 months | 56,886 SAR | PARTIAL/CONFIRMED IN SHEET — needs bank proof |
| Monthly burn | 48,250 SAR | PARTIAL — needs expense evidence |
| Net burn vs current MRR | 19,283.5 SAR | PARTIAL |
| Cash on hand | MISSING | BLOCKER for runway |
| Runway | MISSING / not meaningful | requires cash balance |
| Raw Unit Gross Margin | 87% | VERIFIED-INTERNAL — cost/min 0.36 SAR, sell/min 2.5–3.0 SAR |
| Accounts receivable | 30,291.5 SAR | PARTIAL — needs reconciliation |
| SAICO enterprise pipeline | 57,000 SAR/month potential | PIPELINE — not current MRR |
| SAICO annual potential | 684,000 SAR/year potential | PIPELINE — not current ARR |

**Do not use older numbers** such as 14 paying customers, 11 active customers, ~18K MRR, 40.8K MRR, 489.5K ARR, 532.8K expected annual revenue, 850K spending plan, or dashboard customer/trial counts as current metrics. They are historical/context only or superseded by the current model.

---

## 1) Company identity

- Founder: Abdulrahman Fahad Alkhanfari — CEO / founder — VERIFIED-INTERNAL.
- Investor-facing group name: **Ten Dimensions — Infrastructure for the Autonomous Enterprise** — VERIFIED-INTERNAL.
- First fundraising use case: D10 Group, with **Sondos as current revenue wedge** and **Siyadah as memory/execution moat**.
- Legal/group structure and subsidiary ownership: **MISSING** — must be documented before investor diligence.

---

## 2) Siyadah — investment thesis

- Siyadah thesis: an intelligent operating system for companies that identifies where money leaks, builds digital employees to close the gap, and proves impact with numbers — VERIFIED-INTERNAL as thesis.
- Investor framing: we do not replace employees; we replace the gap between systems and management where money leaks — VERIFIED-INTERNAL.
- Vision: URL/company identity intake → truth mirror/report → “fix this for me” → digital employees → measured ROI — VERIFIED-INTERNAL as vision; not all features are fully launched.
- Loop: sees → understands → decides → executes → measures ROI — VERIFIED-INTERNAL.
- Metaphor: **Siyadah = the nervous system of the company** — VERIFIED-INTERNAL.
- Current commercial status: Siyadah is still pre-commercial/early product; current revenue proof comes from Sondos. Narrative: **Sondos revenue today, Siyadah moat tomorrow.**

---

## 3) Siyadah — technical status

- E2E proof: Chat → build_dynamic_flow → flow_id → digital_employees → Dashboard — VERIFIED-INTERNAL from previous production/log proof.
- 18 digital employees and 19 Activepieces connections existed in founder/test environment — VERIFIED-INTERNAL, not customer metric.
- Architecture: Next.js + FastAPI orchestrator + Activepieces + Postgres + Redis/Railway — VERIFIED-INTERNAL.
- Launch state: not investor-ready as fully commercial product; requires proof gates and demo readiness.
- Internal operating system with command/review agents: CEO review, QA, ship, retro, etc. — useful “we are our first customer” proof.

---

## 4) Sondos — current commercial truth

### 4.1 Active revenue customers used for MRR

| # | Customer | Sector | Revenue treatment | Monthly-equivalent MRR | Gate |
|---:|---|---|---|---:|---|
| 1 | الاناة الطبية | طبي | Current MRR | 17,391.5 SAR | PARTIAL |
| 2 | جمعية زمزم | جمعية خيرية | Current MRR | 5,400 SAR | PARTIAL |
| 3 | شركة تقدير | عقاري | Annual contract 12,900 SAR/year | 1,075 SAR | PARTIAL |
| 4 | جمعية اعادة الحياة | طبي | Current MRR | 5,100 SAR | PARTIAL |

**Current MRR:** 28,966.5 SAR  
**Current ARR:** 347,598 SAR  
**ARPU:** 7,241.625 SAR  
**Rule:** Do not present تقدير as 12,900 SAR monthly. It is annual-contract MRR equivalent only.

### 4.2 Enterprise pipeline — not counted in MRR

| Account | Sector | Monthly potential | Annual potential | Stage | Treatment |
|---|---|---:|---:|---|---|
| SAICO | Insurance / Enterprise | 57,000 SAR | 684,000 SAR | Enterprise pipeline | Pipeline only; not counted in current MRR/ARR. |

SAICO is strategically important because one enterprise account could exceed the current full MRR base. But it must stay separate from current revenue until revenue activation.

### 4.3 Historical pipeline dashboard — mostly trials, not MRR

Source: old `Sondos Ai dashborad` Google Sheet, modified 2026-02-13.

Dashboard summary showed:

| Metric | Dashboard value | Investor use |
|---|---:|---|
| Campaigns | 25 | Historical go-to-market activity |
| Meetings | 25 | Historical pipeline activity |
| Trials | 16 | Trial traction only |
| Customers | 1 | Historical dashboard customer, not current MRR |
| Revenue | 995 SAR | Historical dashboard revenue only |

Campaign channels/names include **email campaigns (حملة إيميلات)**, WhatsApp AI campaigns, and call/voice AI campaigns. These are acquisition motions, not customer names.

The dashboard is useful to prove early sales motion and trials, but **not** current MRR/ARR. Current finance source remains `FINANCIAL_TRUTH_PACK_2026-06-11.md`.

### 4.4 Customer universe — historical / previous / trial / current

This list is the broader customer universe. It must not be confused with current revenue customers. Most names here should be treated as **trial/pipeline/historical** unless later linked to a paid contract or invoice.

| # | Customer | Sector | Classification |
|---:|---|---|---|
| 1 | حصيف | تحصيل | Historical dashboard customer / paid-trial or small paid conversion; not current MRR unless revalidated |
| 2 | سعودي كو / SaudiCo | برمجيات | Trial/pipeline — dashboard shows SaudiCo in trials and not converted |
| 3 | مرن | خدمات HR | Trial/pipeline — dashboard shows trial ended, not converted |
| 4 | Hall Simplify / Hal Simplify Solutions | برمجيات / حلول تقنية | Historical/pipeline, status TBD |
| 5 | الورود | عقاري | Historical/pipeline, status TBD |
| 6 | ساعي تقني | عقاري | Historical/pipeline, status TBD |
| 7 | فانا | عقاري | Historical/pipeline, status TBD |
| 8 | جمعية زمزم | جمعية خيرية | Current revenue customer |
| 9 | جمعية اعادة الحياة | طبي | Current revenue customer |
| 10 | فليتيك | برمجيات | Historical/pipeline, status TBD |
| 11 | الاناة الطبية | طبي | Current revenue customer |
| 12 | شركة تقدير | عقاري | Annual contract / 1,075 SAR MRR-equivalent |
| 13 | SAICO | تأمين / Enterprise | Enterprise pipeline — 57K monthly potential, not current MRR |
| 14 | عميل غير متذكر 1 | MISSING | To identify |
| 15 | عميل غير متذكر 2 | MISSING | To identify |

**Investor rule:** use this as market traction breadth and evidence of sales experiments, not as current customer count or revenue unless status and evidence are confirmed.

### 4.5 Sondos proof assets

- Use case: Arabic/Saudi voice agent for hospitals, clinics, real estate, collections, HR/services, insurance, and software/operations companies — PARTIAL.
- Shared moat: “Sondos voice inside Siyadah” creates a voice-data wedge and memory moat — VERIFIED-INTERNAL as strategic thesis.
- Raw Unit Gross Margin: **87%** — based on cost/minute 0.36 SAR and sell/minute 2.5–3.0 SAR.
- Historical pipeline proof: email campaigns / WhatsApp AI / call AI → meetings → trials → limited conversion — PARTIAL. Useful for showing learning velocity, not financial scale.
- Enterprise pipeline proof: SAICO shows potential enterprise ACV expansion — PARTIAL until fully converted.

---

## 5) Pricing and business model

- Current Sondos revenue model includes per-minute economics and customer packages — PARTIAL.
- Investor-facing raw GM: **87%** — use this as the clean number instead of 85.6%–88.0% range.
- Pricing conflicts from older notes remain SUPERSEDED unless re-approved: $25 starter, 199–999 SAR digital employee bundles, and previous 3K–10K ARPU language.
- Required before deck send: decide the exact pricing line shown to investors: subscription, per-minute, bundled package, or hybrid.

---

## 6) Market

- Internal market claims previously included: 4,839 medical complexes, 50,000+ SMEs in KSA, 200,000+ companies in GCC, and 1M+ in Arab world — PARTIAL.
- These market numbers require external source links before investor deck use.
- Strongest bottom-up wedge now appears to be sectors already touched by customers: healthcare, real estate, collections, HR/services, charities, insurance, and software/operations.

---

## 7) Investor targets and outreach

- Internal target funds: Shorooq, BECO, Global Ventures, MEVP, Wamda, STV, Raed, Vision Ventures, 500 Global, Flat6Labs, Impact46 — PARTIAL.
- Outreach rule remains: do not send deck first. Send hook + vision + current traction + ask for 20 minutes.
- Final prioritization still needs founder decision: STV/Impact46/Shorooq vs broader tier list.

---

## 8) Round and use of funds

- Founder direction from 2026-06-10: raise **$1,000,000**; valuation/equity open to negotiation — PARTIAL.
- Historical anchor 4M SAR for 10% / 40M valuation is SUPERSEDED unless explicitly re-approved.
- Previous use of funds: team 50%, marketing 30%, product 20% — PARTIAL; must be tied to current burn and 18-month model.
- 18-month targets should be rebuilt from current MRR + enterprise pipeline, not old 280-customer/9M ARR assumptions.

---

## 9) Team and legal

- Entity raising: Ten Dimensions / عشر أبعاد لخدمات الأعمال — PARTIAL/needs legal docs.
- Founder: Abdulrahman Alkhanfari — CEO/founder — VERIFIED-INTERNAL.
- Technical partner/founder reference: Abdulmalik Almunif — PARTIAL/needs final role confirmation.
- Team size, payroll, cap table, and legal ownership: MISSING/PARTIAL.

---

## 10) Ten ammunition items — current state

| # | Item | Current state |
|---:|---|---|
| 1 | MRR/ARR/growth | PARTIAL — current MRR/ARR captured; SAICO pipeline tracked separately |
| 2 | Customers/churn | PARTIAL — 4 active revenue customers; broader trial/pipeline universe captured; churn/status still TBD |
| 3 | Call/minute volume | MISSING — important for voice proof |
| 4 | ACV/pricing/margin | PARTIAL — 87% raw GM set; pricing line still TBD |
| 5 | CAC/channels | PARTIAL — old dashboard shows campaigns/meetings/trials, including email campaigns; no reliable CAC yet |
| 6 | Burn/runway | PARTIAL — burn captured; cash/runway missing |
| 7 | Round/valuation/milestones | PARTIAL — $1M direction; valuation/milestones need final model |
| 8 | Team | PARTIAL |
| 9 | Customer stories with numbers | MISSING/PARTIAL — need 2–3 quantified case studies |
| 10 | Market/sector sizing | PARTIAL — needs external sources |

---

## 11) Unexpected strong assets

- Scenario/system architecture documents can become an architecture/moat slide.
- Sovereign Red Team / internal proof discipline can become diligence confidence.
- Founder story: slow approvals / missed opportunities → “12 seconds instead of 48 hours” angle — strong Why-Now narrative.
- Customer/trial breadth across healthcare, real estate, collections, HR/services, charities, insurance, and software gives stronger wedge story than a single-sector pitch.
- SAICO creates a strong enterprise-upside story if handled carefully outside current MRR.

---

## 12) Blocking gates before investor send

- [ ] Identify the 2 missing historical customers.
- [ ] Tag every customer as: Current revenue / Annual contract / Enterprise pipeline / Past paid / Trial / Negotiation / Lost / Unknown.
- [ ] Link contracts, invoices, or proof for the 4 active revenue customers.
- [ ] Confirm SAICO status and only move it into MRR after revenue activation.
- [ ] Add cash balance to calculate runway.
- [ ] Add bank/receipt proof for collected revenue.
- [ ] Replace deck placeholders and remove old 14-customer / 18K-MRR / 40.8K-MRR claim.
- [ ] Update readiness score after deck and data-room cleanup.

---

## 13) One-line investor traction wording — current safe version

> Sondos has 29.0K SAR in current MRR across 4 active revenue customers, with 347.6K SAR implied ARR. Beyond current MRR, SAICO represents an enterprise pipeline opportunity worth 57K SAR/month and 684K SAR/year, not yet counted in revenue. Historical GTM evidence shows 25 campaigns, 25 meetings, and 16 trials, including email, WhatsApp AI, and call AI campaigns. The voice unit economics are strong at approximately 87% raw gross margin. Siyadah turns this voice-data wedge into a long-term memory and execution moat.
