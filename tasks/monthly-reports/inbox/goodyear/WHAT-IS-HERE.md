# Goodyear (entity 731) monthly report files

Pulled 2026-09-08 out of the mixed upload folders `07.26/` and `08.26/` at the top of the
repo. Those folders hold three properties at once (731 Goodyear, 801 Greenfield Gateway,
803 ABI Properties / Roosevelt Commons). Every file below was opened and confirmed to be
Goodyear before it was copied here. The originals are untouched.

Athena's entity number for Goodyear is **731**. The reports print the owner as
**GOODYEAR RETAIL I, LLC** (Roman numeral I). CLAUDE.md records it from Emma as
"Goodyear Retail 1, LLC" (numeral 1). Emma to confirm which is right.

---

## July 2026 - complete

| File | What it is | How it was confirmed |
|---|---|---|
| `Goodyear Retail I, LLC July 2026  Monthly Report.pdf` | **The bound July report, 35 pages** | p1 title page reads "Goodyear / July 2026 / Monthly Report" |
| `731 - 7.26 Executive Summary - New Format.pdf` | July executive summary, 4 pages | Named 731 |
| `731 - 7.26 Executive Summary - New Format.xlsx` | Same, working file, 6 tabs | Title Sheet B6 "Goodyear", B9 "July 2026" |
| `731 - Goodyear VARIANCE - 07.26.xlsx` | Tenant budget vs cash receipts, 13 tabs | Variance tab A1 = 731, Summary tab "Date Revised 7/31/2026" |
| `731-07-26 Good Year Month End Schedule.xls` | Month end schedules | Named 731 |
| `14. Bank Reconciliation (731).pdf` | Bank rec, 5 pages | Account line reads "12598 731OP BELL BANK" |
| `Title Page - Goodyear July 2026.pdf` | Cover page | Reads "Goodyear / July 2026" |
| `Title Page - Goodyear June 2026 (stale).pdf` | Cover page for the wrong month | Reads "Goodyear / **June** 2026" |
| `Journal Entries/055735 - CITY COUNTY TAX.pdf` | JE backup, $904.97 | Both lines post to entity 731 |
| `Journal Entries/055914 - UTILITY INCOME.pdf` | JE backup, $286.67 | Both lines post to entity 731 |

The 35 page bound report contains: title page, rent roll (2p), comparative income statement
(2p), aged delinquencies, CM receivables ledger (3p), budget forecast (2p), balance sheet,
income statement (2p), trial balance, general ledger (9p), security deposits ledger, cash
detail, deposit recap, bank reconciliation (2p), check images (3p), check register (2p),
loan note page.

**It does not include the executive summary.** That is the separate 4 page PDF above.
Emma to say whether the summary is supposed to be bound in.

## August 2026 - not complete

| File | What it is |
|---|---|
| `731 - Goodyear VARIANCE - 08.26.xlsx` | Real August data. Summary tab "Date Revised 8/31/2026" |
| `731 - 08.26 Executive Summary - New Format (July numbers inside).xlsx` | See the warning below |
| `Title Page - Goodyear July 2026 (stale).pdf` | Cover page still says July 2026 |

### The August executive summary is a shell, not August

Athena's file `08.26/731 - 7.26 Executive Summary - New Format.xlsx` has the Title Sheet
month updated to "August 2026" (cell B9) but the body was never touched:

- Executive Summary tab cell A4 still reads "July 2026"
- Every figure on rows 12 to 17 is identical to July's file, to the cent. Total Income
  $31,004.57, Total Operating Expenses $7,629.10, Gross Cash Flow $23,375.47, Total Owners
  Expense $5,688.12, Total Interest Expense $11,514.00, Net Income $6,173.35
- The cash line, the variance commentary and the delinquency tab are all July's words
- Tenant Delinquency tab still shows Planet Fitness $15,437.96, which is the July balance

Same thing happened on Bell Medical Center's August file, and **this is the documented
process, not a mistake.** Athena's "Preparing Monthly Reports" procedure opens the Complete
Executive Summary section with "go to the prior month's folder and save a copy of the Excel
version of the Executive Summary into the current month's Monthly Report folder". The copy is
where the work starts. Corrected 2026-09-08 after reading the procedure.

### Where the income statement actually lives (checked 2026-09-08, Emma's steer)

Emma said the income statement is in the variance spreadsheet. Part of it is. Here is exactly
what is where, all of it opened and tied out.

**1. The full income statement is the `IS` tab of the month end schedule.**
`731-07-26 Good Year Month End Schedule.xls` has 59 tabs and one of them is `IS`. It reads
"Comparative Income Statement / ENTITY: 731 / GOODYEAR RETAIL I, LLC". Every one of the six
lines on the executive summary comes straight off it, to the cent:

| Executive Summary row | IS tab row | July MTD actual | July MTD budget |
|---|---|---|---|
| 12 Total Income | 20, TOTAL INCOME | $31,004.57 | $30,771 |
| 13 Total Operating Expenses | 31, TOTAL COMMON AREA EXPENSE | $7,629.10 | $8,785 |
| 14 Gross Cash Flow | 33, GROSS CASH FLOW | $23,375.47 | $21,986 |
| 15 Total Owners Expense | 45, TOTAL OWNER EXPENSES | $5,688.12 | $1,838 |
| 16 Total Interest Expense | 51, TOTAL INTEREST EXPENSE | $11,514.00 | $13,000 |
| 17 Net Income | 58, NET INCOME | $6,173.35 | $7,148 |

Same mapping Bell Medical uses, just different row numbers. The IS tab also carries the
warning "Report includes an open period. Entries are not final."

**There is no month end schedule for Goodyear in the 08.26 upload.** July's is the only one.

**2. The variance workbook carries the income line and the whole budget.**

- `Variance` tab, **row 16**, is the income statement reconciliation. Cell BN16 literally
  says "i/s". For August: cell AK16 budget **$30,771**, AL16 actual **$30,771.92**, AM16
  variance **$0.92**. Year to date: BK16 budget **$246,060**, BL16 actual **$269,235.24**,
  BM16 variance **$23,175.24**.
  Checked against July, where AF16/AG16/AH16 read 30,771 / 31,004.57 / 233.57, which is
  exactly what the July executive summary shows on row 12. So this row is trustworthy.
- `Summary` tab is the 2026 operating budget, entity 731, "Date Revised 8/31/2026". It is
  where the whole budget column comes from. Tied out against July: TOTAL INCOME row 25
  ($30,771.94), SUBTOTAL COMMON AREA row 55 ($8,784.92 = the $8,785 budget), NET OPERATING
  INCOME row 73 ($21,987.02 = the $21,986 gross cash flow), TOTAL OWNER EXPENSE row 90
  ($14,837.81) less Interest Expense row 86 ($13,000) = $1,837.81 = the $1,838 owner expense
  budget. All six budget figures reconcile.
- The Summary tab holds **no actuals**. Every month January through December carries the same
  figure, because it is a budget spread across the year.

**3. So for August I have one actual line out of six.**

Total Income is settled: MTD $30,771.92 against a $30,771 budget, up $0.92. YTD $269,235.24
against $246,060, up $23,175.24, or 9.42%.

Operating expenses, gross cash flow, owner expenses, interest expense and net income have no
August actual anywhere in the upload. Those five cannot be written without the income
statement.

**4. What would unblock it: one file.**

`731-08-26 Good Year Month End Schedule.xls`, the August twin of the July one, or failing
that the 08/26 comparative income statement printed for entity 731. Either gives all six
lines.

Checked every other Excel file in the 08.26 upload. The only `IS` tab in there belongs to
`803 ABI Monthly Schedules 08.26.xlsx`, which reads "ENTITY: 803 / ABI PROPERTIES, INC".
That is Roosevelt Commons, not Goodyear.

### What is missing for August

Nothing else Goodyear was in the `08.26/` upload. Every other loose PDF in that folder was
opened and belongs to entity 803, Roosevelt Commons (aged report, CM ledger, rent roll,
SD ledger), except the mortgage statement, which is Greenfield Gateway.

Still needed to write August's summary:

- [ ] **The one that matters:** `731-08-26 Good Year Month End Schedule.xls`, for its `IS`
      tab. Or the 08/26 comparative income statement printed for entity 731
- [ ] Rent roll for 08/26
- [ ] Aged delinquencies for 08/26
- [ ] Goodyear month end schedule for 08.26
- [ ] Bank reconciliation for 08/26, account 731OP
- [ ] The bound August report PDF, if Athena has produced one

---

## Things worth a second look before anything goes to the owner

**Square footage does not agree.** The executive summary header (cell H7) says **51,159**
square feet. The July rent roll totals say **50,394**. The exact same 51,159 appears on
Bell Medical Center's summary too, whose rent roll says 12,476. It looks like a number that
got copied across templates and never corrected.

**Percent leased does not agree with the rent roll.** The summary (cell H8) says
**44.12% leased**. That equals Planet Fitness alone, 22,235 divided by 50,394. But the rent
roll's own totals line says **Occupied Sqft 50,394, 100.00%, Vacant 0**. Both cannot be
right.

**Suite 409-117, 28,159 sq ft, is in transition.** The July rent roll shows SPIRIT
HALLOWEEN with a lease that expired 11/17/2025, and SUPERPLAY under "New Leases" running
4/1/2027 to 3/31/2037 at $29,369.79 a month. So the big box sits empty until spring 2027.

**Planet Fitness is the delinquency.** $15,437.96 current as of the 07/26 aged report:
$14,988.31 prior year CAM charged 4/4/2025 plus $449.65 sales tax. Athena's July note reads:
"Outstanding charges for PYC ($15K - likely revised to $4K) and sales tax assessments ($500).
Working with Senior Accountant to satisfy PF's questions in order to make payment."
Last payment 7/30/2026, $28,917.09.

**Tenants on the 07/26 books:** PLANET FITNESS (suite 409-112, 22,235 sq ft, 1/10/2023 to
1/31/2033), SPIRIT HALLOWEEN (409-117, 28,159 sq ft, expired 11/17/2025), EVGO (parking
charge, no square footage, 2/26/2022 to 2/29/2032). SUPERPLAY signed for 409-117 starting
4/1/2027.

**Property manager fields on the summary:** Property Manager Danielle Cebrero, Assistant
Property Manager Jaie Benson. Same as Bell Medical's. Emma to confirm whether her own name
belongs on Goodyear.
