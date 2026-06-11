# Sondos Financial Truth Pack — 2026-06-11

> Source of truth: `Sondos_Investor_Financials` Google Sheet, last modified 2026-06-11.  
> Rule: any metric without evidence must remain tagged as unverified.  
> The older April 14 file is context-only and must not be used for current financial metrics.  
> **Important clarification:** MRR below is **contracted/current MRR**, not necessarily cash collected. شركة تقدير is included in contracted MRR but has **not paid yet** as of the latest founder clarification; payment is expected soon.

## Source links

- Current official financial model: https://docs.google.com/spreadsheets/d/1UR1mGf8HFn8b2bOUlQgVrmu3eKBMWJ6d3nxfZdVtLCk/edit
- Historical context-only file: https://docs.google.com/spreadsheets/d/1S3JbcEwtIABEmZTgWDfufUUFy56Ojbdq/edit

---

## Current investor summary

| Metric | Current value | Status | Note |
|---|---:|---|---|
| Paying customers / active contracted customers | 4 | Unverified | Must be linked to contracts/invoices before investor send. |
| Contracted MRR | 40,791.5 SAR | Unverified | Includes شركة تقدير 12,900 SAR even though not collected yet. |
| Collection-adjusted MRR excluding تقدير until paid | 27,891.5 SAR | Internal caution | Use only if we want a conservative cash-collected view. |
| ARR from contracted MRR | 489,498 SAR | Unverified | Formula: 40,791.5 x 12. |
| ARPU from contracted MRR | 10,197.875 SAR | Unverified | Formula: 40,791.5 divided by 4 active contracted customers. |
| Collected revenue — last 6 months | 56,886 SAR | Confirmed in sheet | Cash collected, not invoices sent. |
| Fixed monthly expenses | 48,250 SAR | Unverified | Needs final finance evidence. |
| Monthly burn | 48,250 SAR | Unverified | Gross monthly spend. |
| Net burn vs contracted MRR | 7,458.5 SAR | Unverified | Formula: burn minus contracted MRR. |
| Cash on hand | Missing | Unverified | Required for runway. |
| Runway | Not meaningful yet | Unverified | Requires cash balance. |
| Unit Gross Margin | 85.6%–88.0% | Confirmed in sheet | Based on minute economics. |
| Accounts receivable | 30,291.5 SAR | Unverified | Includes uncollected amounts; at minimum تقدير 12,900 SAR is not paid yet. |

---

## MRR by active contracted customer

| # | Customer | Sector | MRR | Start date | Collection status | Investor treatment |
|---:|---|---|---:|---|---|---|
| 1 | الاناة الطبية | طبي | 17,391.5 SAR | 2026-04-28 | Needs proof / reconcile with A/R sheet | Count in contracted MRR only after evidence pack is linked. |
| 2 | جمعية زمزم | جمعية خيرية | 5,400 SAR | 2026-03-03 | Needs proof | Count in contracted MRR; verify invoice/payment evidence. |
| 3 | شركة تقدير | عقاري | 12,900 SAR | 2026-02-04 | **Not paid yet; likely soon** | Count as contracted MRR / A/R, not as collected cash. |
| 4 | جمعية اعادة الحياة | طبي | 5,100 SAR | 2026-05-20 | Needs proof | Count in contracted MRR; verify invoice/payment evidence. |

**Contracted MRR:** 40,791.5 SAR.  
**Collection-adjusted MRR excluding تقدير until paid:** 27,891.5 SAR.  
**Rule:** do not present contracted MRR as cash collected.

---

## Customer concentration

| Rank | Customer | Monthly revenue | Share of contracted MRR |
|---:|---|---:|---:|
| 1 | الاناة الطبية | 17,391.5 SAR | 42.6% |
| 2 | شركة تقدير | 12,900 SAR | 31.6% |
| 3 | جمعية زمزم | 5,400 SAR | 13.2% |
| 4 | جمعية اعادة الحياة | 5,100 SAR | 12.5% |

Investor note: the top two customers represent approximately 74.2% of contracted MRR. This is normal for an early-stage company but must be disclosed clearly.

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

Important distinction: collected revenue is historical cash received. Contracted MRR is current recurring revenue entitlement/relationship. Do not mix them in Gross Margin calculations.

---

## Unit economics — minute gross margin

| Item | Value | Status |
|---|---:|---|
| Cost per minute | 0.36 SAR | Confirmed in sheet |
| Sell price per minute — low | 2.50 SAR | Confirmed in sheet |
| Sell price per minute — high | 3.00 SAR | Confirmed in sheet |
| Gross margin at 2.50 SAR/min | 85.6% | Confirmed in sheet |
| Gross margin at 3.00 SAR/min | 88.0% | Confirmed in sheet |
| Investor-facing Unit GM | 85.6%–88.0% | Confirmed in sheet |

Formula: `(selling price per minute - cost per minute) / selling price per minute`.

---

## Historical/context-only file — April 14

The historical file includes useful structure only: customer contracts, customer categories, older executive summary, competitor analysis framework, and older spending/growth planning.

Do not use current numbers from that file. It contains old metrics such as 11 active customers, 532,800 SAR expected annual revenue, and an 850,000 SAR spending plan. These are superseded by the 2026-06-11 financial model.

---

## Open finance gates before investor send

- [ ] Confirm the 4 active contracted customer records against contracts and invoices.
- [ ] Confirm whether each MRR line is paid, invoiced, contracted-only, or overdue.
- [ ] Confirm تقدير payment date; until paid, show it as contracted MRR / A/R, not collected cash.
- [ ] Add cash on hand to calculate real runway.
- [ ] Attach bank or receipt evidence for collected revenue.
- [ ] Confirm expense evidence for all burn categories.
- [ ] Confirm accounts receivable status and expected collection dates.
- [ ] Decide whether the deck shows contracted MRR, collection-adjusted MRR, or both.

Recommended investor wording:

> Sondos currently has 40.8K SAR in contracted/current MRR across 4 active customers, with 489.5K SAR implied ARR. One customer, تقدير, representing 12.9K SAR MRR, is not collected yet and is treated as accounts receivable until payment. The voice unit economics are strong: minute cost is approximately 0.36 SAR while resale price ranges from 2.5 to 3.0 SAR, implying 85.6%–88.0% unit gross margin. These numbers remain subject to final finance evidence linking contracts, invoices, and collection proof.
