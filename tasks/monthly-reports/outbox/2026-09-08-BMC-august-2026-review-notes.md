# Bell Medical, August 2026 Executive Summary

**File:** `2026-09-08-BMC-august-2026-executive-summary.xlsx`
**Built:** 2026-09-08 by CC. Finalised 2026-09-09 with Emma's decisions.
**Status:** COMPLETE, awaiting Emma's review and send. Owner facing, so CC does not send it.

---

## The report at a glance

| | MTD actual | MTD budget | Variance | YTD actual | YTD budget | Variance |
|---|---|---|---|---|---|---|
| Total Income | 21,186.88 | 35,502 | (14,315.12) | 163,909.73 | 220,747 | (56,837.27) |
| Total Operating Expenses | 13,067.63 | 11,728 | (1,339.63) | 132,475.76 | 90,609 | see note |
| Gross Cash Flow | 8,119.25 | 23,774 | (15,654.75) | 31,433.97 | 130,138 | (98,704.03) |
| Total Owners Expense | 1,672.74 | 1,034 | (638.74) | 32,691.11 | 6,430 | (26,261.11) |
| Total Interest Expense | 4,368.22 | 4,508 | 139.78 | 34,556.98 | 35,642 | 1,085.02 |
| Net Income | 2,078.29 | 18,232 | (16,153.71) | (35,814.12) | 88,066 | (123,880.12) |

Arithmetic verified both directions, MTD and YTD:
income minus operating expenses equals gross cash flow; gross cash flow minus owner expenses
minus interest equals net income.

Tenant delinquency: **AZ Sports and Spine, $10,100.71**, up from $8,400.96 in July.

---

## How it was built

The July workbook was copied and its sheet XML patched in place, so all 14 embedded photos, the
styles, print areas and formulas survive untouched. Opening this file with a spreadsheet library
and re-saving destroys 99.7% of it, so that route was avoided (see `WORKFLOW.md`).

Every figure in the financial table was pulled programmatically from the August Comparative
Income Statement. Nothing was retyped by hand.

### Where every number came from

The financial table comes from the **`IS` tab** inside
`Bell Medical Monthly Schedules 08.26.xlsx`. That tab is the Comparative Income Statement for
entity 802, PARAGON PROPERTIES GROUP LLC, thru 8/31/2026, generated 9/7/2026 4:38 PM. The
standalone PDF was missing from the August package.

| Report line | IS tab row |
|---|---|
| Total Income | row 23, TOTAL INCOME |
| Total Operating Expenses | row 54, TOTAL COMMON AREA EXPENSE |
| Gross Cash Flow | row 56, GROSS CASH FLOW |
| Total Owners Expense | row 63, TOTAL OWNER EXPENSES |
| Total Interest Expense | row 69, TOTAL INTEREST EXPENSE |
| Net Income | row 76, NET INCOME |

- **Income variance commentary**: `Variance` tab of `802 Bell Medical - 08.26.xlsx`, August and
  YTD columns. Wording follows the per tenant comments Athena had already written there.
- **Expense drivers**: individual GL rows on the IS tab.
- **Delinquency $10,100.71 and the $3,448.43 payment on 8/6/2026**: `AGED REPORT.pdf`, period
  08/26, run 9/7/2026 4:44 PM.

---

## Emma's decisions, 2026-09-09

| Item | Decision |
|---|---|
| Renewals, Property Highlights, Capital Projects | **Carry forward unchanged.** Emma checked May, June and July; all three read the same every month. Nothing moved in August. |
| OMBI renewal | Tenant is exercising their option to renew. Wording stands. |
| Asphalt sealcoat | Did happen in March. Wording stands. |
| Lease expirations | **Keep 10/31/26** for both tenants. See the note below. |
| Square Feet | **Keep 51,159.** See the note below. |
| % Leased | **Keep 61.14%.** See the note below. |
| Property Manager | Danielle Cebrero, retained. |
| Assistant slot | **Emma Bogardus**, replacing Jaie Benson, on all six tabs. |
| That slot's label | Changed from "Assistant Property Manager" to **"Property Coordinator"** on all six tabs. |

Jaie Benson's name deliberately remains in the Operational Issues paragraph, which records a
meeting she attended on 19 January 2026. That is history, not a name slot.

### Three figures CC could not source

Raised, discussed, and decided to leave as they are. Recorded here so the reasoning is not lost,
not to reopen the decision.

**Lease expirations.** The report says both OMBI and AZ Sports & Spine expire 10/31/26. Both the
July and August rent rolls, generated from ATHENA, say **3/31/2027** and **3/15/2027**. CC
searched the entire August workbook and every July PDF: **10/31/26 appears in no
system-generated report at all.** The rent roll also shows OMBI's option starting 4/1/2027, the
day after its stated expiry, which is internally consistent.

**Square Feet, 51,159.** Appears in no Athena report for either month. It exists only inside the
Executive Summary workbook, hand typed across six tabs. The August rent roll says **12,476 total
square feet** across 6 units.

**% Leased, 61.14%.** Same. The August rent roll says **69.20% occupied**, 8,633 of 12,476 sq ft,
3 of 6 units. Vacant suites are 100B (726), 101B (922) and 103B (2,195). For context, 61.14% is
roughly what occupancy was *before* AZ Trim Clinic took Suite 102B in June 2026.

If any of these come up later, the rent roll is where to start.

### Two wording fixes CC made

Both in text going to an owner:
- "The are paying" corrected to "They are paying"
- "partial payments.Tenant indicates" given its missing space

---

## Still open, not blocking this report

**1. The August package is missing 14 files.** July had 24, August has 10. Missing: the
Comparative Income Statement PDF, Budget Forecast, Balance Sheet, Standard Income Statement,
Trial Balance, General Ledger, Cash Detail, Check Register, Bank Reconciliation, Rent Roll with
Lease Options, the JE BACKUP folder and the numbered title page.

The Executive Summary is complete without them, but the **bound package cannot be assembled**
the way July's was. Worth asking whoever runs the exports to re-run August, and asking why 14
files dropped off.

**2. "Report includes an open period. Entries are not final."** The August income statement says
this. So did July's, and July's report went out anyway, so it is probably boilerplate on every
Athena export. Worth one question to accounting sometime.

**3. Cell `H13` subtracts the wrong way round.** The YTD Operating Expenses variance uses the
income convention (Actual minus Budget) instead of the expense one, so the year's **$41,867
overspend displays as positive $41,867**, reading like good news. The MTD cell beside it, and both
other expense rows, do it correctly. July's report showed a $40,527 overspend as +40,527 for the
same reason.

Left untouched. This is Athena's standard template, so it affects every property, not just Bell
Medical. Not Emma's call alone.

**4. Old template debris in the Monthly Schedules workbook.** The `Stats Page` tab is a
statistical analysis for a property called **Bayside Center, twelve months ended June 30, 2010**.
The `Min Rent Plan` and `Min Rent Forecast` tabs are headed **"MINIMUM RENT VARIANCE REPORT
2009/2010"** and carry square footage (13,256 total, 12,056 occupied) that matches neither the
rent roll nor the Executive Summary. None of it feeds the report. It is sixteen year old residue
from whatever file this workbook was originally built from.

**5. The `COI Tab` header reads "August 2025",** a year stale. It was already wrong in July's
file, so it was left alone rather than guess whether that tab is still in use.

---

## Before it goes out

- [ ] Emma reviews the workbook
- [ ] Second set of eyes, owner facing work does not leave on one person's say so
- [ ] Save as PDF
- [ ] Assemble the bound package, blocked on the 14 missing files
