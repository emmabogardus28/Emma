# Roosevelt Commons, August 2026 Executive Summary: review notes

Drafted 2026-09-08. Entity **803**, ABI Properties, INC. File:
`2026-09-08-RSC-august-2026-executive-summary.xlsx`.

**Do not send yet.** Seven things below need Emma. Everything else is sourced and checked.

---

## Where every number came from

The money table is a straight lift from the `IS` tab of
`803 ABI Monthly Schedules 08.26.xlsx`, headed "Comparative Income Statement / ENTITY: 803 /
ABI PROPERTIES, INC", through 8/31/2026.

| Summary row | IS tab row | MTD actual | MTD budget | YTD actual | YTD budget |
|---|---|---|---|---|---|
| 12 Total Income | 19 TOTAL INCOME | $249,844.02 | $208,168 | $549,799.76 | $416,336 |
| 13 Total Operating Expenses | 41 TOTAL COMMON AREA EXPENSE | $15,923.32 | $18,557 | $27,576.66 | $47,414 |
| 14 Gross Cash Flow | 43 GROSS CASH FLOW | $233,920.70 | $189,611 | $522,223.10 | $368,922 |
| 15 Total Owners Expense | 48 TOTAL OWNER EXPENSES | $50,000.00 | $5,077 | $50,000.00 | $10,154 |
| 16 Total Interest Expense | 53 TOTAL INTEREST EXPENSE | $0.00 | $0 | $0.00 | $0 |
| 17 Net Income | 60 NET INCOME | $183,920.70 | $184,534 | $472,223.10 | $358,768 |

Nothing was retyped. Every figure was read out of the file programmatically.

### Arithmetic proved four ways

1. **Down the statement, MTD.** $249,844.02 less $15,923.32 is $233,920.70. Then less
   $50,000.00 less $0.00 is $183,920.70. Both tie.
2. **Down the statement, YTD.** $549,799.76 less $27,576.66 is $522,223.10. Then less
   $50,000.00 is $472,223.10. Both tie.
3. **Down the budget column.** $208,168 less $18,557 is $189,611, less $5,077 is $184,534.
   YTD: $416,336 less $47,414 is $368,922, less $10,154 is $358,768. All tie.
4. **Across the months.** July's finished YTD plus August's month equals August's YTD, on
   every one of the six lines. Income: $299,955.74 plus $249,844.02 is $549,799.76. Operating
   expenses: $11,653.34 plus $15,923.32 is $27,576.66. And so on down.

### Delinquency tab

From `Aged report.pdf`, "ENTITY: 803 ABI PROPERTIES, INC / Period: 08/26". Tenants over
$2,000 only, which is three this month against five in July:

| Tenant | Balance | Current | 1 month |
|---|---|---|---|
| McDonald's | $26,052.40 | $13,026.20 | $13,026.20 |
| The Buffalo Spot | $17,583.10 | $9,283.40 | $8,299.70 |
| Heartland Dental | $3,151.70 | $34.08 | $3,117.62 |
| **Total** | **$46,787.20** | | |

**First Watch and Mattress Firm are gone from the report.** They owed $19,586.04 and
$18,486.63 in July and both cleared. I removed their rows. TA Nail Bar ($738.02) and Desert
Financial Credit Union ($65.96) are on the aged report but under the $2,000 threshold, so
they are not on the tab. Cross check: $46,787.20 plus $738.02 plus $65.96 is $47,591.18,
which is the entity total printed on the report.

### Header figures

From `Rent Roll.pdf`, "ROOSEVELT COMMONS / Bldg ID 803", **as of 8/31/2026**. 11 occupied
units, 54,885 sq ft, 100.00% occupied, 0 vacant, monthly base rent $180,148.84. I added up
all 11 suites: 3,466 + 3,676 + 3,843 + 25,000 + 3,800 + 1,800 + 1,899 + 2,500 + 3,900 +
1,201 + 3,800 is exactly 54,885, and the 11 base rents sum to exactly $180,148.84. The rent
roll is internally consistent and the summary's 54,885 and 100% were already right.

### Commentary

Income bullets come from the `Variance Analysis` tab of `803 ABI Properties Variance
08.26.xlsx`, August column, which carries Athena's own per tenant comments. Expense bullets
are the individual GL rows on the IS tab. Every bullet was checked to sum back to the
headline: MTD operating expense favourables total $6,787.00 against unfavourables of
$4,153.32, netting to the $2,633.68 on the table. YTD, $39,382.66 against $19,545.32, netting
to $19,837.34.

---

## Correction made 2026-09-08

Emma flagged that the first draft used bullets under $1K. Six of them: "-($0.6K) TA Nail Bar,
Panda Express", "-$0.8K Electric/Building, Electric/Common Area", "-$0.1K Pest Control
Maintenance, Sweeping", "-($0.9K) Janitorial, Building Lighting", "-$0.9K Electric/Building",
and "-($0.5K) On Site Management Fees, Janitorial, Building Lighting".

All six are gone. The small accounts are grouped into lines that clear $1,000, with every
account named, which is how Athena's own summaries are written. Nothing was dropped, and each
group was re-checked against its headline:

| Section | Bullets sum to | Headline |
|---|---|---|
| Income, month | $41,676.18 | $41,676.02 (16 cents of rounding inside Athena's variance workbook) |
| Operating expenses, month | $2,633.68 | $2,633.68 |
| Operating expenses, year | $19,837.34 | $19,837.34 |
| Owner expenses, month | ($44,923.00) | ($44,923.00) |
| Owner expenses, year | ($39,846.00) | ($39,846.00) |

The rule is now written into `HOW-IT-WORKS.md` and `WORKFLOW.md` so it holds next month.

## Checked against Athena's procedure

Emma sent "Preparing Monthly Reports" on 2026-09-08, saved to
`tasks/monthly-reports/reference/`. The draft was re-checked against it.

**Followed:**

- "Do not change any cells that have formulas." Only literal cells were written. Every formula
  survives, including the shared formulas in the % Change columns. Cached values were
  refreshed and `fullCalcOnLoad` is set so Excel recomputes on open.
- "Double check that the Net Income numbers on the spreadsheet match the Net Income line on
  the Comparative Income report." Done. $183,920.70 for the month, $472,223.10 year to date,
  matching IS row 60 exactly.
- "Variances and offsets should be entered as bullet points." Done, with an Offset by block.
- Delinquency comments say what the balance represents.

**One item closed by the procedure.** Renewals is defined as "any tenant within 12 months of
lease expiration date". Checked every lease on the 8/31/2026 rent roll against 8/31/2027. The
earliest expiration in the whole centre is **Mattress Firm on 9/30/2035**, nine years out.
So **"None" is correct and provable**, not a carried forward guess. That drops the narrative
sections needing Emma from seven to six.

**Two threshold questions for Emma.**

1. **The variance threshold.** The procedure says comment on variances "typically greater than
   $2,500 or 5%". Emma's instruction today was nothing under $1K. The draft currently uses the
   $1K floor with small accounts grouped upward. Note the procedure's test is an either/or, so
   a small account with a big percentage swing still qualifies, and most of Roosevelt's small
   accounts do: Trash Removal came in at $0 against a $1,100 budget, which is 100%. Say which
   rule governs and the commentary will be regrouped to match.

2. **The delinquency threshold.** The procedure says balances "in excess of $2,500". The
   column header inside the workbook says "Balances over $2,000". **This does not change
   August**, the three tenants on the tab are $26,052.40, $17,583.10 and $3,151.70, all clear
   of both, and the two left off are $738.02 and $65.96, below both. But the header and the
   procedure disagree and Athena should fix one of them.

**Two things the procedure asks for that are not done yet.**

- **Spell check on each tab.** Cannot be run from here. Please run it in Excel before this
  goes anywhere.
- **The delinquency comments are missing two of their three required parts.** The procedure
  wants what the balance represents, the most recent attempt to collect, **and** whether it
  has been collected or paid down since the books closed. The drafts have the first, and only
  partly the second. See item 3 below.

**Two things to ask about.**

- **COI Tracking is marked "JH Reports Only"** and comes from a Docutrax report. What is JH,
  and does it cover ABI Properties? If it does not, that may be why the COI tab has been
  carrying another property's data, and the tab may not belong in this report at all.
- **Gross Sales.** The procedure has a step for Gross Sales comments. Roosevelt's summary has
  no Gross Sales section and no gross sales report came in the August package. Coconut Grove
  has one. Does Roosevelt need one?

**One thing I got wrong earlier and have corrected.** I flagged the August summary file being
an identical copy of July's as an Athena error, on Bell Medical and again on Goodyear. It is
not. The procedure's first instruction under Complete Executive Summary is to save a copy of
the prior month's Excel summary into the current month's folder. The copy is the intended
starting point. Corrected in both sets of notes and in the workflow.

## Six things that need Emma

**1. The $50,000 in Other Professional Fees.** This is the single biggest item in the report.
GL 70230, $50,000.00 posted in August against a zero budget. It is the whole reason net
income came in flat against budget despite income running 20% ahead. The summary currently
says only "Other Professional Fees, nothing budgeted this period", which is true but tells
the owner nothing. **What was it?** It needs a real explanation before this goes to ABI.

**2. My note about the year to date comparison.** I added a paragraph to the YTD income
commentary that is not in Athena's usual format:

> "Year to date actual covers June through August. Year to date budget covers July and August
> only, since ownership closed June 8, 2026. June collections of $160,606.31 therefore sit in
> the actual column with no budget against them."

I added it because the YTD column shows income 32% over budget, and a reader would take that
as performance when a large part of it is a missing budget month. The $160,606.31 is July's
YTD actual of $299,955.74 less July's month actual of $139,349.43, and July's YTD budget of
$208,168 is exactly one month of budget, which is what confirms the budget year starts in
July. **Strike the paragraph if you would rather not raise it, it comes out cleanly.** Worth
confirming the reason with accounting either way.

**3. The three delinquency notes are mine, not a person's, and they are incomplete.** The
procedure wants three things in each: what the balance represents, the most recent attempt to
collect, and whether it has been collected or paid down since close of books. Mine cover the
first and only partly the second. The third is missing entirely, and only you know it. I wrote them from the aged
report detail because July's notes had gone stale. They are factual but they are not the
collection story:

- Heartland Dental: "Base rent current. Outstanding is July CAM, insurance, real estate tax
  and sales tax of $3,117.62 plus August CAM of $34.08. Last payment 8/31/2026, $21,179.06."
- McDonald's: "Tenant owes July and August in full, $13,026.20 each. Funds were approved for
  release the last week of August, not yet received."
- The Buffalo Spot: "Working with tenant on construction. July and August base rent and NNN
  outstanding, $9,283.40 current and $8,299.70 one month."

**McDonald's especially.** July's note said funds were approved for release the last week of
August and September would be on time. August closed with both months still owing. Whatever
the current status is, that sentence needs your words.

**4. The narrative sections are still July's words.** I did not touch them, and I am not
going to put words in your mouth. Renewals is now settled, see above. The rest need your read:

| Section | Currently says |
|---|---|
| Tenant Issues | "Buffalo Spot - working with tenant on construction. Will circle back on rent." |
| Operational Issues | The June 8 closing and transition paragraph, including "Security deposits totaling $70,080.08 transferred at closing." Three months old now |
| Renewals (12 months) | "None". **Confirmed correct**, earliest expiry is Mattress Firm 9/30/2035 |
| New Leases/Completed Renewals | "N/A" |
| Legal | "None" |
| Property Highlights and Trends | "Management conducts bi-monthly inspections and is working closely with vendors to maintain the center." |
| Capital Projects / Tenant Improvements | "No capital scheduled for this year. Buffalo Spot is only tenant under construction." |

**5. The Photos tab is empty.** Same as July.

**6. Two header fields I corrected.** Flagging because I changed them rather than only
reporting them:

- **Tenant Delinquency tab, Square Feet: was 51,159, now 54,885.** 51,159 is not Roosevelt's
  number, it is the same figure sitting on Bell Medical Center's and Goodyear's summaries.
  The Executive Summary tab already said 54,885 and the rent roll confirms it.
- **COI tab, Square Feet 64,702 and % Leased 95.56%, now 54,885 and 100%.** Those were
  another property's figures. 95.56% is Greenfield Gateway's July percentage.

**7. There is a hidden tab carrying another owner's tenant list.** The workbook has a sheet
called "COI Tab", hidden, which reads "COI Tracking / **Greenfield Gateway** / August 2025"
and lists 16 Greenfield tenants (Kachina Stained Glass, EOS Fitness, Bright Now Dental and so
on). None of them are Roosevelt tenants.

**I left it exactly as it was.** It is hidden so it will not print into the bound report, and
I was not going to rewrite a whole tab on my own. But it travels inside the file, and if this
workbook ever goes to ABI Properties as a spreadsheet rather than a PDF, another owner's
tenant list goes with it. Worth telling Athena so the template gets cleaned up.

---

## Also worth knowing

**The income statement carries the open period warning.** The IS tab says "Report includes an
open period. Entries are not final." Accounting may still be posting to August. Standard, but
it means these figures can move.

**Roosevelt Commons is fully leased and the rent roll is clean.** Unlike Goodyear's, this one
reconciles perfectly: 11 units, no vacancy, no expired leases still flagged active, and the
suite square footages add exactly to the stated total.

**How the file was edited.** The workbook was patched inside the zip, XML level, so the
embedded photos and the Athena logo survive untouched. Verified afterwards: all 57 zip
entries present in the original order, all 11 media files byte identical, 2.87 MB of images
intact, zip integrity clean, and the file reopens correctly. `fullCalcOnLoad` is set so Excel
recalculates every formula the moment it opens.
