# Monthly Reports

Owner executive summary commentary.

Started 2026-09-08. First real run: Bell Medical (BMC), August 2026, using July 2026 as the pattern.

---

## What comes in

Emma uploads a folder per month, named `MM.YY` (for example `08.26`), into
`tasks/monthly-reports/inbox/`. Everything is exported from **ATHENA**, Athena Property
Management's accounting system. Bell Medical is **entity / building 802**.

A complete month looks like July 2026 did, 24 files:

| File | What it is | Needed for the summary? |
|---|---|---|
| `00.Title Page - MM.YY.pdf` | Cover page | Package only |
| `02.Rent Roll with Lease Options.pdf` | Suites, sq ft, base rent, expirations, options | **Yes** |
| `03.Comparative Income Statement.pdf` | Actual vs budget, MTD and YTD | **Yes, this is the core** |
| `04.Aged Delinquencies.pdf` | Past due by tenant and bucket | **Yes** |
| `05.CM Receivables Ledger.pdf` | Charges and receipts by tenant | Backup |
| `06.Budget Forecast.pdf` | Forecast | Package |
| `07.Balance Sheet.pdf` | Balance sheet | Package |
| `08.Standard Income Statement.pdf` | Income statement | Package |
| `10.Trial Balance.pdf` | Trial balance | Package |
| `11.General Ledger.pdf` | GL detail | Backup for variances |
| `12.Security Deposits Ledger.pdf` | Deposits held | Package |
| `13.Cash Detail.pdf` / `14.Check Register.pdf` | Cash and checks | Package |
| `Bank Reconciliation.pdf` | Bank rec | Package |
| `Mortgage Statement.pdf` | Loan statement | Package |
| `JE BACKUP/` | Journal entry support | Backup |
| `802 - MM.YY Executive Summary.xlsx` | **The deliverable template** | **Yes** |
| `802 Bell Medical - MM.YY.xlsx` | Tenant level budget vs payment, with Athena's own comments | **Yes** |
| `Bell Medical Monthly Schedules MM.YY.xlsx` | 60+ tabs of schedules, includes an `IS` tab | **Yes** |

**August 2026 arrived with only 10 of these.** Do not assume a full package. Check what is
actually there before starting, and say plainly what is missing.

## What goes out

A filled in copy of `802 - MM.YY Executive Summary.xlsx`, written to
`tasks/monthly-reports/outbox/` as `YYYY-MM-DD-BMC-<month>-executive-summary.xlsx`, plus a
review notes markdown file alongside it listing every unresolved question.

The workbook has 7 tabs: Title Sheet, Executive Summary, Tenant Delinquency, Photos,
Tenant COI Tracking, Tenant Maintenance Tracking, COI Tab. The month appears in a header on
almost all of them and every one needs updating.

Emma reviews, then it becomes a PDF and goes into the bound package
(`<Owner> <Month> <Year> Monthly Report.pdf`). **CC never sends it.**

## Steps

1. **Inventory the folder first.** Compare against the table above and note what is missing.
2. **Find the income statement.** If `03.Comparative Income Statement.pdf` is absent, the same
   data lives on the **`IS` tab** of `Bell Medical Monthly Schedules MM.YY.xlsx`. That is where
   August's came from.
3. **Check the open period warning.** The IS header says "Report includes an open period.
   Entries are not final" when accounting is still posting. Always flag this to Emma.
4. **Patch the workbook, never rebuild it.** See "Things learned" below, this matters.
5. **Map the IS rows into the Executive Summary table:**

   | Executive Summary row | Comes from IS row |
   |---|---|
   | 12 Total Income | 23, TOTAL INCOME |
   | 13 Total Operating Expenses | 54, TOTAL COMMON AREA EXPENSE |
   | 14 Gross Cash Flow | 56, GROSS CASH FLOW |
   | 15 Total Owners Expense | 63, TOTAL OWNER EXPENSES |
   | 16 Total Interest Expense | 69, TOTAL INTEREST EXPENSE |
   | 17 Net Income | 76, NET INCOME |

   Columns map straight across: B/C/D/E are MTD actual, budget, variance, percent; F/G/H/I are
   the YTD equivalents. D, E, H and I are formulas, so refresh their cached values too.
6. **Prove the arithmetic.** Income minus operating expenses must equal gross cash flow. Gross
   cash flow minus owner expenses minus interest must equal net income. Both MTD and YTD. If it
   does not tie, stop and find out why.
7. **Commentary thresholds.** Athena's procedure says to comment on significant variances,
   "typically greater than $2,500 or 5%". It is an either/or, so a small account with a large
   percentage swing still qualifies. On top of that, Emma's rule: **no bullet under $1K**.
   Group small accounts together until the line clears $1,000 and name every account in the
   group. Grouping, never dropping, the bullets still have to sum to the headline.
8. **Write the variance commentary** from the `Variance` tab of `802 Bell Medical - MM.YY.xlsx`.
   Athena already writes per tenant comments there (BAS, NNN, CAM, STX, LAT codes). Follow the
   house format: a headline, then `-($X.XK) Reason` bullets, then `Offset by:` and the favourable
   ones. Expense drivers come from the individual GL rows on the IS tab.
9. **Delinquency tab** from the aged report. Athena's procedure says balances **in excess of
   $2,500**. The column header inside the workbook says "Balances over $2,000". They disagree,
   the procedure wins, raise the header with Athena. Each line needs three things:
   what the balance represents, the most recent attempt to collect it, and whether it has been
   collected or paid down since the books closed.
10. **Renewals is not a judgement call.** The procedure defines it as any tenant within 12
   months of its lease expiration date. Read the rent roll, compare against the period end,
   and write what you find. "None" is an answer you prove, not one you carry forward.
11. **Carry forward the other narrative sections** (Tenant Issues, Gross Sales, Operational,
   Legal, Highlights and Trends, Capital Projects / Tenant Improvements) and tell Emma
   explicitly that they are last month's words and need hers.
12. **Spell check every tab.** The procedure calls for it after each one.
13. **Manager's review.** The report goes to the Property Manager, Danielle Cebrero, before it
   is packaged. Emma does not send it onward herself.
14. **Write the review notes file.** Every number cited to its source, every open question listed.
15. Move nothing out of `inbox/`. Save and push.

## Things learned

- **No variance bullet under $1K.** Emma flagged this on the Roosevelt Commons August draft,
  2026-09-08. The first draft carried six sub-$1K bullets, "-$0.1K Pest Control Maintenance,
  Sweeping" being the worst of them. Group small accounts up until the line clears $1,000 and
  list every account in the group. Athena's own summaries do exactly this.
- **Never open this workbook with openpyxl and save it.** A round trip destroys 99.7% of the
  file, all 14 embedded photos and the logo included, dropping it from 6.1 MB to 20 KB. Patch the
  sheet XML inside the zip instead, and rezip preserving the original entry order. Read values
  with openpyxl (`data_only=True`) all you like, just never save with it.
- Text cells reference `sharedStrings.xml`. Rewriting them as inline strings
  (`t="inlineStr"`) avoids touching the shared string table.
- Set `fullCalcOnLoad="1"` in `xl/workbook.xml` so Excel recalculates on open.
- **Pull figures programmatically, never retype them.** Owner facing money.
- **Athena's own files carry errors.** On the first run: square footage and percent leased on the
  summary matched no source report, two lease expiration dates contradicted the rent roll, and
  the COI tab was a year stale. Check, do not assume, and flag rather than silently correct.
- **The "August" file being an identical copy of July is not an error.** Corrected 2026-09-08
  after reading Athena's procedure. Step one of Complete Executive Summary is literally "go to
  the prior month's folder and save a copy of the Excel version of the Executive Summary into
  the current month's Monthly Report folder". The copy is the intended starting point. Filling
  it in is the job, not evidence that somebody forgot.
- **Do not change any cells that have formulas.** Straight from the procedure. Set the literal
  cells only and let the formulas recompute. Refreshing a formula's cached value is fine, the
  formula itself must survive.
- **Check net income twice.** The procedure calls for it by name: the Net Income on the
  spreadsheet must match the Net Income line on the Comparative Income Statement before you go
  any further.
- **COI Tracking is "JH Reports Only"** and comes from a Docutrax report. Ask Emma what JH
  means and which properties it covers. It may be why the COI tabs are stale on properties
  where it does not apply.
- The rent roll is the system of record for suites, square footage and lease dates. The
  Executive Summary header fields are hand typed and drift.
- Bell Medical tenants as of 08/26: **OMBI** (Suite 100A, 5,659 sq ft), **Arizona Sports & Spine
  Physicians** (101A, 1,967 sq ft), **Arizona Trim Clinic** (102B, 1,007 sq ft, took occupancy
  6/1/2026). Vacant: 100B (726), 101B (922), 103B (2,195).
- AZ Sports & Spine is the chronic delinquency. Partial payments, balance climbing.

---

## Standing rules that apply here

These come from CLAUDE.md and are not optional:

- **Read every line** of every statement. Quote the file and the row for every number reported.
  Never round, never estimate, never paraphrase a figure.
- **No em-dashes or en-dashes.** This goes to owners.
- **Full property names only**, never the in-house nicknames. Bell Medical Center, not Bell
  Medical. Goodyear, not Litchfield.
- **Owner-facing work needs Emma's eyes before it goes anywhere.** Flag it, do not bury it.
- Signature block on anything sent as an email or letter.
