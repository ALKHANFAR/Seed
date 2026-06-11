# Sondos Financial Truth Pack — 2026-06-11

> Source of truth: `Sondos_Investor_Financials` Google Sheet, last modified 2026-06-11.
> Rule: any metric without evidence must remain tagged as unverified.
> The older April 14 file is context-only and must not be used for current financial metrics.

## Source links

- Current official financial model: https://docs.google.com/spreadsheets/d/1UR1mGf8HFn8b2bOUlQgVrmu3eKBMWJ6d3nxfZdVtLCk/edit
- Historical context-only file: https://docs.google.com/spreadsheets/d/1S3JbcEwtIABEmZTgWDfufUUFy56Ojbdq/edit

---

## Current investor summary

| Metric | Current value | Status | Note |
|---|---:|---|---|
| Paying customers | 4 | Unverified | Must be linked to contracts/invoices before investor send. |
| MRR | 40,791.5 SAR | Unverified | Current recurring revenue from 4 paying customers. |
| ARR | 489,498 SAR | Unverified | Formula: MRR x 12. |
| ARPU | 10,197.875 SAR | Unverified | Formula: MRR divided by paying customers. |
| Collected revenue — last 6 months | 56,886 SAR | Confirmed in sheet | Cash collected, not invoices sent. |
| Fixed monthly expenses | 48,250 SAR | Unverified | Needs final finance evidence. |
| Monthly burn | 48,250 SAR | Unverified | Gross monthly spend. |
| Net burn | 7,458.5 SAR | Unverified | Formula: burn minus MRR, floored at zero. |
| Cash on hand | Missing | Unverified | Required for runway. |
| Runway | Not meaningful yet | Unverified | Requires cash balance. |
| Unit Gross Margin | 85.6%–88.0% | Confirmed in sheet | Based on minute economics. |
| Accounts receivable | 30,291.5 SAR | Unverified | Requires invoice and collection evidence. |

---

## MRR by paying customer

| # | Customer | MRR | Start date | Status |
|---:|---|---:|---|---|
| 1 | الاناة الطبية | 17,391.5 SAR | 2026-04-28 | Unverified |
| 2 | جمعية زمزم | 5,400 SAR | 2026-03-03 | Unverified |
| 3 | شركة تقدير | 12,900 SAR | 2026-02-04 | Unverified |
| 4 | جمعية اعادة الحياة | 5,100 SAR | 2026-05-20 | Unverified |

Total MRR: 40,791.5 SAR.

---

## Customer concentration

| Rank | Customer | Monthly revenue | Share of MRR |
|---:|---|---:|---:|
| 1 | الاناة الطبية | 17,391.5 SAR | 42.6% |
| 2 | شركة تقدير | 12,900 SAR | 31.6% |
| 3 | جمعية زمزم | 5,400 SAR | 13.2% |
| 4 | جمعية اعادة الحياة | 5,100 SAR | 12.5% |

Investor note: the top two customers represent approximately 74.2% of MRR. This is normal for an early-stage company but must be disclosed clearly.

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

Important distinction: collected revenue is historical cash received. MRR is current recurring revenue. Do not mix them in Gross Margin calculations.

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

- [ ] Confirm the 4 paying customer records against contracts and invoices.
- [ ] Confirm all 40,791.5 SAR MRR is active and billable today.
- [ ] Add cash on hand to calculate real runway.
- [ ] Attach bank or receipt evidence for collected revenue.
- [ ] Confirm expense evidence for all burn categories.
- [ ] Confirm accounts receivable status and expected collection dates.
- [ ] Decide whether the deck shows monthly Gross Margin, Unit Gross Margin, or both.

Recommended investor wording:

> Sondos currently shows 40.8K SAR MRR across 4 paying customers, with 489.5K SAR implied ARR. The voice unit economics are strong: minute cost is approximately 0.36 SAR while resale price ranges from 2.5 to 3.0 SAR, implying 85.6%–88.0% unit gross margin. These numbers remain subject to final finance evidence linking contracts, invoices, and collection proof.
