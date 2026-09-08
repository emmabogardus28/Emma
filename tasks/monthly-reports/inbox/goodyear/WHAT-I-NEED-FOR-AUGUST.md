# Goodyear August 2026 executive summary: what is still needed

Worked out 2026-09-08 by taking the finished July summary apart cell by cell and tracing
every filled cell back to the report it came from. Entity 731, GOODYEAR RETAIL I, LLC.

## Short version

Five reports. One of them, the month end schedule, covers most of the workbook on its own.

| # | Report | Period | Fills |
|---|---|---|---|
| 1 | **Month end schedule** `731-08-26 Good Year Month End Schedule.xls` | 08/26 | The six line money table **and** all of the expense commentary |
| 2 | **Balance sheet** | Jul 2026 close through Aug 2026 | The ending cash balance line |
| 3 | **Aged delinquencies** | 08/26 | The whole Tenant Delinquency tab |
| 4 | **Rent roll with lease options** | as of 8/31/2026 | Square feet, percent leased, the Leasing section |
| 5 | **Mortgage statement** for the Goodyear loan | August | The Loan Status line |

Already in hand: `731 - Goodyear VARIANCE - 08.26.xlsx`. It gives the income side of the
commentary and the entire budget column. Nothing more is needed from Athena for that part.

---

## The long version, cell by cell

### 1. Month end schedule, `IS` tab. The big one.

The `IS` tab is a Comparative Income Statement headed "ENTITY: 731 / GOODYEAR RETAIL I, LLC".
It fills two separate things.

**The six line table, rows 12 to 17 of the Executive Summary tab.** Straight lift:

| Executive Summary row | IS tab row |
|---|---|
| 12 Total Income | 20, TOTAL INCOME |
| 13 Total Operating Expenses | 31, TOTAL COMMON AREA EXPENSE |
| 14 Gross Cash Flow | 33, GROSS CASH FLOW |
| 15 Total Owners Expense | 45, TOTAL OWNER EXPENSES |
| 16 Total Interest Expense | 51, TOTAL INTEREST EXPENSE |
| 17 Net Income | 58, NET INCOME |

Columns B/C/D/E are month actual, budget, variance, percent. F/G/H/I are the year to date
equivalents.

**The expense commentary, rows 25, 26, 28 and 29.** Every bullet is a GL line off the same
tab. Checked against July:

- "-$18.9K Common Area Association" is IS row 23, YTD variance $18,902.00
- "-$4K General Maintenance" is IS row 25, YTD variance $4,000.00
- "Offset by: -($1.8K) Fire Protection Repairs" is IS row 27, YTD variance -$1,819.14
- "-($1.8K) Utilities Expense" (month) is IS row 40, month variance -$1,847.01
- "-($15.5K) Utilities Expense" (year) is IS row 40, YTD variance -$15,455.81
- "-($8.8K) Legal Fees" is IS row 37, YTD -$8,755.00
- "-($3.2K) Other Professional Fees" is IS row 38, YTD -$3,179.97
- "-($2.8K) General Repairs & Maint" is IS row 36, YTD -$2,795.30
- "-($2.1K) HVAC Repair/Labor, City Sales Tax" is IS rows 43 and 44, -$1,350.00 and -$758.03

A comparative income statement printed for entity 731, period 08/26, does the same job if the
schedule is not available. The schedule is better, it is the source the rest comes from.

### 2. Balance sheet, for the cash line

July reads "This month's ending operating cash balance is $535,214.84". That is the
**TOTAL CURRENT ASSETS** line on the balance sheet, page 12 of the bound July report:
CASH-OPERATING $564,697.59, SUSPENSE ($40,882.75), MISCELLANEOUS DEPOSITS $11,400.00,
total $535,214.84.

Worth asking Emma: the sentence says "operating cash balance" but the number is total current
assets. Cash operating on its own is $564,697.59. Two different numbers, and only one of them
is what the sentence claims to be.

The month end schedule's `TB` tab carries $564,697.59 but not the $535,214.84, so the balance
sheet is a separate ask.

### 3. Aged delinquencies, for the Tenant Delinquency tab

Tenants with balances over $2,000 only. July had one: Planet Fitness $15,437.96, which is
$14,988.31 prior year CAM charged 4/4/2025 plus $449.65 sales tax. The action note beside it
is written by Athena, not pulled from a report.

### 4. Rent roll with lease options

Feeds three things:

- Square Feet, cell H7. July said 51,159. The rent roll said 50,394. Unresolved, see below.
- Percent Leased, cell H8. July said 44.12%, which is Planet Fitness alone, 22,235 / 50,394.
- The Leasing section, row 43. July's SuperPlay entry (10 year term, expiring 3/31/2037, rent
  $29,369.79 commencing April 2027, two 5 year options at 4/1/2037 and 4/1/2042) matches the
  rent roll's option rows exactly. The 210 to 360 day notice window is not on the rent roll,
  that came off the lease itself.

### 5. Mortgage statement

July reads "Loan is current and the ending statement balance is $2,138,006.57". That is the
Ending Statement Balance on the Midland Loan Services statement, page 35 of the bound July
report. The same figure appears on the general ledger as account 25300 NOTES PAYABLE.

Note the loose `Mortgage Statement.pdf` in both the 07.26 and 08.26 uploads is **Greenfield
Gateway**, not Goodyear. The Goodyear statement only exists inside the bound July report.

---

## Not reports. These have to come from Emma.

The July file carries last month's words in all of these. They are not pulled from anything
and they will be wrong for August unless Emma replaces them:

| Section | July said |
|---|---|
| Tenant Issues | "None at this time" |
| Operational Issues | "None at this time" |
| Renewals (12 months out) | "None at this time." |
| Legal | "None at this time." |
| Property Highlights and Trends | "None." |
| Capital Projects / Tenant Improvements | "None. " |
| Photos tab | Empty. The note on it says "Paste photos of any recent work, slurry, tree trimming, paint, new tenants, etc" |
| Tenant COI Tracking tab | Evgo Services, LLC yes/yes. Planet Fitness on file yes, in compliance **no**, "Missing Additional Insurance - tenant has been contacted". Needs checking, that note is a month old |
| Tenant Maintenance Tracking tab | Headers only, nothing filled in |

---

## Errors found in the July file, carry these forward carefully

**The income commentary is a month stale.** Row 23 says "YTD Income is over budget by
$22,940.75 or 12.43%". The table directly above it, row 12, says the YTD variance is
$23,174.32, or 10.76%. The difference is exactly $233.57, which is July's own month variance.
So the sentence is June's number, never updated when July was written. June's YTD budget was
$184,518 and $22,940.75 against it is 12.43%, which confirms it. **For August the correct
figures are $23,175.24 and 9.42%**, from the Variance tab row 16, columns BK, BL and BM.

**Square feet does not match the rent roll.** Summary says 51,159, rent roll says 50,394. The
same 51,159 is sitting on Bell Medical Center's summary too, whose rent roll says 12,476.

**Percent leased contradicts itself inside the same workbook.** The Executive Summary,
Tenant Delinquency, Photos and Maintenance tabs all say 44.12%. The Tenant COI Tracking tab
says 100%. The rent roll's own totals line says 100.00% occupied with 0 vacant, while its
detail shows the 28,159 sq ft box empty until SuperPlay starts 4/1/2027.
