# Sondos Financial Truth Pack — 2026-06-11

> Source of truth: `Sondos_Investor_Financials` Google Sheet, last modified 2026-06-11.  
> Rule: any metric without evidence must remain tagged as unverified.  
> The older April 14 file and old Sondos dashboard are context-only and must not be used for current financial metrics.  
> **Important clarification:** MRR below is current monthly-equivalent revenue. شركة تقدير is a **12,900 SAR annual contract**, so its MRR-equivalent is **1,075 SAR**, not 12,900 SAR monthly.  
> **Enterprise pipeline clarification:** SAICO is a high-value enterprise pipeline account at **57,000 SAR/month potential** and **684,000 SAR/year potential**, but it is **not counted in MRR/ARR until fully completed as revenue**.

## Source links

- Current official financial model: https://docs.google.com/spreadsheets/d/1UR1mGf8HFn8b2bOUlQgVrmu3eKBMWJ6d3nxfZdVtLCk/edit
- Historical context-only file: https://docs.google.com/spreadsheets/d/1S3JbcEwtIABEmZTgWDfufUUFy56Ojbdq/edit
- Historical pipeline dashboard: https://docs.google.com/spreadsheets/d/19A3EJP57igBV4TvDoE4yHnNbSTEQ3TAkndlg5wgDcq8/edit

---

## Current investor summary

| Metric | Current value | Status | Note |
|---|---:|---|---|
| Active revenue customers | 4 | Unverified | Must be linked to evidence before investor send. |
| Current MRR | 28,966.5 SAR | Unverified | Includes تقدير as annual-contract MRR-equivalent of 1,075 SAR. |
| Current ARR | 347,598 SAR | Unverified | Formula: 28,966.5 x 12. |
| ARPU | 7,241.625 SAR | Unverified | Formula: 28,966.5 / 4 active revenue customers. |
| Collected revenue — last 6 months | 56,886 SAR | Confirmed in sheet | Cash collected, not invoices sent. |
| Fixed monthly expenses | 48,250 SAR | Unverified | Needs final finance evidence. |
| Monthly burn | 48,250 SAR | Unverified | Gross monthly spend. |
| Net burn vs current MRR | 19,283.5 SAR | Unverified | Formula: burn minus current MRR. |
| Cash on hand | Missing | Unverified | Required for runway. |
| Runway | Not meaningful yet | Unverified | Requires cash balance. |
| Raw Unit Gross Margin | 87% | Confirmed internally | Single investor-facing raw GM number from minute economics. |
| Accounts receivable | 30,291.5 SAR | Unverified | Needs reconciliation with annual-contract vs collection evidence. |
| SAICO enterprise pipeline | 57,000 SAR/month potential | Pipeline only | Not counted in MRR/ARR yet. |
| SAICO annual potential | 684,000 SAR/year potential | Pipeline only | Enterprise upside, not current revenue. |

---

## MRR by active revenue customer

| # | Customer | Sector | Revenue treatment | Monthly-equivalent MRR | Start date | Investor treatment |
|---:|---|---|---|---:|---|---|
| 1 | الاناة الطبية | طبي | Current MRR | 17,391.5 SAR | 2026-04-28 | Count in current MRR after evidence is linked. |
| 2 | جمعية زمزم | جمعية خيرية | Current MRR | 5,400 SAR | 2026-03-03 | Count in current MRR after evidence is linked. |
| 3 | شركة تقدير | عقاري | Annual contract 12,900 SAR/year | 1,075 SAR | 2026-02-04 | Do not count as 12,900 SAR monthly; use annual-contract MRR equivalent only. |
| 4 | جمعية اعادة الحياة | طبي | Current MRR | 5,100 SAR | 2026-05-20 | Count in current MRR after evidence is linked. |

**Current MRR:** 28,966.5 SAR.  
**Current ARR:** 347,598 SAR.  
**ARPU:** 7,241.625 SAR.  
**Rule:** do not present تقدير as 12,900 SAR monthly.

---

## Customer concentration — current MRR only

| Rank | Customer | Monthly revenue / MRR | Share of current MRR |
|---:|---|---:|---:|
| 1 | الاناة الطبية | 17,391.5 SAR | 60.0% |
| 2 | جمعية زمزم | 5,400 SAR | 18.6% |
| 3 | جمعية اعادة الحياة | 5,100 SAR | 17.6% |
| 4 | شركة تقدير | 1,075 SAR | 3.7% |

Investor note: current MRR is still early and concentrated. Enterprise upside should be shown separately through pipeline, not mixed into current MRR.

---

## Enterprise pipeline — not counted in MRR

| Account | Sector | Monthly potential | Annual potential | Stage | Treatment |
|---|---|---:|---:|---|---|
| SAICO | Insurance / Enterprise | 57,000 SAR | 684,000 SAR | Enterprise pipeline | Pipeline only; not counted in current MRR/ARR. |

---

## Cash collected — last 6 months

| Month | Collected revenue | Status |
|---|---:|---|
| December 2025 | 8,751 SAR | Confirmed in sheet |
| January 2026 | 5,175 SAR | Confirmed in sheet |
| February 2026 | 11,613 SAR | Confirmed in sheet |
| March 2026 | 18,630 SAR | Confirmed in sheet |
| April 2026 | 5,115 SAR | Confirmed in sheet |
| May 2026 | 7,602 SAR | Confirmed in sheet |
| Total | 56,886 SAR |  |

Important distinction: collected revenue is historical cash received. Current MRR is the monthly-equivalent recurring revenue base. Pipeline is excluded.

---

## Unit economics — raw gross margin

| Item | Value | Status |
|---|---:|---|
| Cost per minute | 0.36 SAR | Confirmed internally |
| Sell price per minute | 2.50–3.00 SAR | Confirmed internally |
| Raw Unit Gross Margin | 87% | Investor-facing number |

Formula basis: `(selling price per minute - cost per minute) / selling price per minute`, normalized to one clean investor-facing number: **87% raw GM**.

---

## Historical/context-only files

The historical files include useful structure only: customer contracts, customer categories, older executive summary, competitor analysis framework, old dashboard campaigns, meetings, and trials.

Do not use current numbers from those files. They contain old metrics such as 11 active customers, 532,800 SAR expected annual revenue, 850,000 SAR spending plan, 16 trials, 1 customer, and 995 SAR dashboard revenue. These are historical/pipeline context only.

---

## Open finance gates before investor send

- [ ] Confirm the 4 active revenue customer records against contracts and invoices.
- [ ] Confirm whether each MRR line is paid, invoiced, revenue-active, or pending.
- [ ] Confirm تقدير annual contract evidence and payment/collection status.
- [ ] Confirm SAICO status and only move it into MRR after revenue activation.
- [ ] Add cash on hand to calculate real runway.
- [ ] Attach bank or receipt evidence for collected revenue.
- [ ] Confirm expense evidence for all burn categories.
- [ ] Decide whether the deck shows only current MRR or current MRR + enterprise pipeline.

Recommended investor wording:

> Sondos currently has 29.0K SAR in current MRR across 4 active revenue customers, with 347.6K SAR implied ARR. Separately, SAICO is an enterprise pipeline opportunity worth 57K SAR/month and 684K SAR/year, but it is not counted in MRR yet. The voice unit economics are strong, with approximately 87% raw gross margin based on minute cost of 0.36 SAR and resale price of 2.5–3.0 SAR.
