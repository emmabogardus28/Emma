# Coconut Grove, September 2026: Tenant Delinquency tab notes

Workbook: `2026-10-16-CGR-september-2026-executive-summary.xlsx`. Only the Tenant Delinquency tab was changed. Every other tab is exactly as Emma uploaded it.

Source for every number: `04. Aged Delinquencies.pdf`, ATHENA, Entity 165, COCONUT GROVE RETAIL XIII, LLC, Period 09/26, run 10/14/2026 9:11 AM, 6 pages.

## What's on the tab

The tab's own header says "Over $2,500", so that's the cutoff used. Sorted largest first.

| Tenant on tab | Name on aged report | Balance | Where it comes from (aged report) |
|---|---|---|---|
| Chong Qing Hot Pot | CHONG QING HOT POT | $61,502.13 | p.2: Current 28,214.34 / 1 Mo 28,214.34 / 2 Mo 28,214.34 / 3 Mo 5,642.87 / 4 Mo -28,783.76. Last payment 12/11/2025 |
| Humpy's | HUMPYS BIG ISLAND ALEHOUSE | $54,487.39 | p.3: all Current. Last payment 6/3/2026 |
| Foster's Kitchen | FOSTERS KITCHEN | $33,463.58 | p.4: Current 24,151.97 / 1 Mo 748.00 / 4 Mo 8,563.61. Last payment 2/27/2026 |
| Laverne's | LAVERNES (KOHOLA LLC) | $19,330.39 | p.3: all Current, incl. LAT 880.96. Last payment 8/13/2026 |
| Lucasie | LUCASIE LTD | $14,659.08 | p.1: Current 11,538.95 / 4 Mo 3,120.13. Last payment 9/29/2026 |
| Kona Heaven Coffee (Café Kona) | KONA HEAVEN COFFEE | $6,958.31 | p.5: PYC 5/1/2025, all 4 Mo. Last payment 9/29/2026 |
| **Total** | | **$190,400.88** | Formula =SUM(B13:B18) |

Checks run: every tenant's buckets add to its total, and all 11 tenants add to the report's Grand Total of $176,628.91. The tab total is higher than the grand total because credit balances are left off (below).

Left off:
- ABC STORE 75, -$14,828.09. Prepaid rent credit (p.4), not a delinquency.
- Under $2,500: Gecko Girlz $1,368.22, Kona Gear $1,822.26, Oceans -$1,860.11, SVC Hawaii -$274.25.

## Questions for Emma (please look before it goes out)

1. **Humpy's credit disappeared.** August's tab showed Humpy's at **-$39,301.31** ("2025 PYC reversal ... being deferred as part of the amendment"). September's aged report shows no credit at all, just $54,487.39 of September charges. The Tenant Issues text also says **$110,521.46** is deferred through 8/31/26, and that isn't on the aged report either. Ask accounting what happened to both before this goes to the owner.
2. **Payments, answered by the September general ledger.** The "$43K Humpy's & Laverne's paid prior month's rent" note on the Executive Summary is August's commentary carried forward (see below). The September ledger has no base rent receipt from Humpy's ($20,666.80), Laverne's ($7,408.00), Lucasie ($7,895.51), Foster's ($12,262.80) or Chong Qing ($13,000.00), which matches the aged report. Lucasie's "last payment 9/29/2026 $10,750.67" on the aged report is not in the September ledger, so it was probably posted in October. One question to accounting.
3. **Three tenants are new to the tab:** Foster's Kitchen, Laverne's, Kona Heaven Coffee. Kona Heaven's $6,958.31 dates to 5/1/2025, so it was probably left off on purpose last month. The renewal notes (Executive Summary B36) say Landlord agreed to waive that 2024 PYC. If you'd rather keep it off, delete row 18 and the total fixes itself.
4. **"Action Taken" comments are mine, built only from the aged report and the workbook's own notes.** I don't know what's actually been done this month (calls, notices, payment plans). Add anything real. Chong Qing's "continues to ignore requests for payment" comes from the New Leases note (B32).
5. **Tenant names.** I spelled out "Chong Qing Hot Pot" (August said "Chong Hot Pot"; the aged report says CHONG QING HOT POT). The New Leases section spells it "Chong Quin Hot Pot," which doesn't match either. Not on this tab, but worth fixing.

## Fixed from last month

- August's total formula was =SUM(B13:B14), which skipped the third tenant. It now covers every row.
- Print area extended to cover the new rows.

## Noticed, not touched

- The logo on the tab reads "JH Mangement" (missing an "a"). It's an image, so it can't be fixed here.
- The sales notes and narrative under the table (A41, A43) are outside the print area and were left alone.

## September reports cross-check (added after Emma sent the 09/26 rent roll, income statement, balance sheet and general ledger)

Everything on the delinquency tab ties:
- Balance sheet 9/30/2026: Accounts Receivable $221,528.72 less Prepaid Rent $44,899.81 = **$176,628.91**, the aged report's grand total.
- Income statement September late charges $2,204.60 = the three late charges on the aged report (Lucasie $525.87, Laverne's $880.96, Oceans $797.77).
- Rent roll 9/30/2026: Humpy's base rent is now $20,666.80 (was $25,000.00 on 8/31). Laverne's is unchanged at $7,408.00, so I took "full rent resumed" off Laverne's comment.
- September income statement shows no Rent Deferral or Prior Year CAM activity in September (both $0.00 MTD), so the ledger doesn't explain Humpy's missing -$39,301.31 credit. That question stands.

## NOT the delinquency tab, but please look: Executive Summary tab problems

1. **Two rows are swapped.** Comparing the Executive Summary tab to `01. Comparative Income Statement.pdf` (Sep 2026):

   | | Income statement says | Workbook shows |
   |---|---|---|
   | Total Operating Expenses, MTD actual | 162,881.50 (TOTAL COMMON AREA EXPENSE) | 171,697.25 |
   | Total Operating Expenses, MTD budget | 120,426.91 | 275,269.09 |
   | Net Operating Income, MTD actual | 171,697.25 | 162,881.50 |
   | Total Operating Expenses, YTD actual | 1,243,823.19 | 1,622,664.33 |
   | Total Operating Expenses, YTD budget | 1,365,548.29 | 1,591,987.71 |
   | Net Income, MTD | (58,016.54) | (66,832.29) |

   CC added up every expense line on the income statement: they total 162,881.50 MTD and 1,243,823.19 YTD, so the income statement is right and the workbook has NOI typed into the expense row. Net income on the income statement also ties to the balance sheet's current retained earnings (158,651.24 YTD).

2. **The variance commentary is August's.** The MTD notes say revenue is *over* budget ("$14K Parking Rent higher than anticipated") and expenses are *under* budget ("$12K Security"). September's income statement shows revenue **under** budget by (61,117.25), with parking (23,333.30) under, and expenses **over** budget by (42,454.59), with security (26,029.85) and food court security (17,569.97) over. The $14K parking and the YTD "$66K Parking" figures match August's income statement (parking +14,202.54 MTD, +65,950.10 YTD).

## Checked against the completed August report (added after Emma sent it)

Source: `CGR 08.26/04. Aged Delinquencies.pdf` (Period 08/26, run 9/11/2026) and `CGR 08.26/165 08.26 Coconut Grove Executive Summary.xlsx`.

- **Method matches.** August's tab used each tenant's net Total line: Lucasie 3,120.13 and Chong Qing 33,287.79 are exactly the Total lines on the August aged report. September does the same.
- **Humpy's -$39,301.31 was not on the August aged report.** Humpy's doesn't appear on it at all, so they had no balance at 8/31. The -$39,301.31 on August's tab was carried forward from an older month. There is no missing credit, and the question for accounting about it can be dropped.
- **August left off three tenants over $2,500:** Foster's Kitchen $9,311.61, Kona Heaven Coffee $6,958.31, Gecko Girlz $3,103.86 (all current). Emma to decide whether September follows that.
- **August's Executive Summary rows are in the right order** (expense budget 212,157.91 = TOTAL COMMON AREA EXPENSE budget), which confirms September's are swapped.
- **August's actuals come from a cash income statement.** August's workbook shows Total Income 397,197.44 and Operating Expenses 193,346.69. The accrual income statement for August shows 357,042.39 and 176,180.68. Budgets match either way. September's workbook currently has accrual figures, so September needs the **cash** income statement to fill in correctly.
