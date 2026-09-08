# Coconut Grove, August 2026 Executive Summary: review notes

Drafted 2026-09-08. Entity **165**, COCONUT GROVE RETAIL XIII, LLC, Kailua-Kona.
File: `2026-09-08-CGR-august-2026-executive-summary.xlsx`.

**Do not send yet.** One item at the top is serious and it is about July, not August.

---

## THE BIG ONE: July's report was built on the wrong income statement

Athena produces **two** income statements for this property every month, an **accrual** one and
a **cash** one, printed at the same moment. July's are both dated 8/14/2026 at 8:40 AM.

**July's executive summary was built on the accrual statement.** I checked all eight lines,
month and year to date, and every one matches the accrual figures exactly.

The summary itself says it should be the cash one. Cell A12 reads **"CASH"**, and the
commentary headings read **"Revenue (per cash income statement)"** and **"Operating Expenses
(per cash income statement)"**.

Athena's own variance workbook agrees that cash is correct. Its July cash receipts total
**$212,581.81**, which is exactly the cash statement's Total Income. The accrual statement says
$349,463.18.

The difference is not small:

| July 2026, month | On accrual (what was sent) | On cash (what the template asks for) |
|---|---|---|
| Total Income | $349,463.18 | $212,581.81 |
| Total Operating Expenses | $133,031.77 | $127,987.00 |
| Net Operating Income | $216,431.41 | $84,594.81 |
| Adjusted Net Operating Income | ($34,405.81) | ($166,242.41) |
| Interest Expense | $145,075.09 | $140,173.72 |
| **Net Income** | **($190,109.99)** | **($317,045.22)** |

**July's report understated the loss by $126,935.23.**

**August is drafted on the cash basis**, because that is what the template asks for, what
Athena's variance workbook reconciles to, and the only August statement that exists. There is
no August accrual statement in the upload.

**What this means for the year to date column.** August's YTD figures are cash. July's were
accrual. So August's YTD will not tie to what the owner saw last month. Emma needs to decide
whether to say something about that in the report, and Athena needs to know July went out
wrong.

---

## Where every August number came from

The money table is a straight lift from the `IS` tab of
`165_08.26 Coconut Grove Monthly Schedule.xlsx`, headed "Comparative Income Statement /
ENTITY: 165 / COCONUT GROVE RETAIL XIII, LLC / Cash", through 8/31/2026, printed 9/3/2026.

| Summary row | IS tab row | MTD actual | MTD budget | YTD actual | YTD budget |
|---|---|---|---|---|---|
| 13 Total Income | 28 | $397,197.44 | $345,519 | $2,481,097.10 | $2,561,840 |
| 14 Total Operating Expenses | 69 | $190,317.04 | $212,157.91 | $1,143,248.46 | $1,245,121.38 |
| 15 Net Operating Income | 71 | $206,880.40 | $133,361.09 | $1,337,848.64 | $1,316,718.62 |
| 16 Total Owners Expense | 84 | $71,937.25 | $7,325 | ($33,691.71) | $52,400 |
| 17 Adjusted Net Operating Income | 86 | $134,943.15 | $126,036.09 | $1,371,540.35 | $1,264,318.62 |
| 18 Corporate G&A Expenses | 91 | $14,183.85 | $18,712 | $125,505.37 | $139,570 |
| 19 Interest Expense | 98 | $145,075.09 | $160,833 | $1,149,461.75 | $1,286,664 |
| 20 Net Income after G&A & Interest | 102 | ($24,315.79) | ($53,508.91) | $96,573.23 | ($161,915.38) |

**Only five rows were typed in.** Rows 15, 17 and 20 are formulas in the workbook, so they
computed themselves. They came out at $206,880.40, $134,943.15 and ($24,315.79), matching the
income statement's own totals exactly. That is the strongest check available: the workbook's
formula chain independently reproduced the statement.

**Every commentary bullet was checked back to its headline.** Revenue, operating expenses and
owner expenses all reconcile, month and year to date, and no bullet is under $1K.

### Delinquency tab

From `AGED REPORT.pdf`, "ENTITY: 165 COCONUT GROVE RETAIL XIII, LLC / Period: 08/26". Balances
over $2,500, which the procedure requires and this template's own column header states:

| Tenant | Balance |
|---|---|
| Chong Qing Hot Pot | $33,287.79 |
| Foster's Kitchen | $9,311.61 |
| Kona Heaven Coffee | $6,958.31 |
| Lucasie Ltd | $3,120.13 |
| Gecko Girlz Shave Ice Shack | $3,103.86 |
| **Total** | **$55,781.70** |

**I had to restructure this tab.** The template has four tenant rows with the Total on row 17.
August has five qualifying balances, so row 17 became the fifth tenant and the Total moved to
row 18, reusing the blank row already there. Styles and row heights moved with them.

**And I fixed a bug in it.** July's Total was `=SUM(B13:B15)` while four tenants were listed in
rows 13 to 16. It silently omitted Chong Hot Pot's $5,073.45. July's tab showed a total of
($36,181.18) when the four balances actually came to ($31,107.73). The new total is
`=SUM(B13:B17)` and covers every row.

### Header

From `RENT ROLL.pdf`, "COCONUT GROVE MARKET PLACE / Bldg ID 165", as of 8/31/2026: 17 occupied
units, 48,065 sq ft, **94.14% occupied**, 1 vacant unit of 2,993 sq ft, **51,058 sq ft total**.
48,065 plus 2,993 is 51,058, and 48,065 divided by 51,058 is 94.14%, so the roll is internally
consistent.

**I corrected the square footage from 50,133 to 51,058.** The 94.14% the summary was already
carrying only works against 51,058, not against 50,133, so the two header fields disagreed with
each other. Emma to approve.

---

## Nine things that need Emma

**1. The July accrual/cash problem above.** Biggest item on this page.

**2. Humpy's has vanished from the delinquency report.** July showed a credit of
($39,301.31) with the note "Credit reflects 2025 PYC reversal. The balance is being deferred as
part of the amendment." August's aged report has no Humpy's line at all. The deferral presumably
went through, and the income statement's YTD Rent Deferral of ($65,479.31) looks related, but
nothing in the files says so. Worth a sentence in the report.

**3. Oceans Sports Bar and Grill has a credit of ($2,657.88)** on the August aged report. It
clears $2,500 in size, and July did show a credit (Humpy's) on the tab, so it arguably belongs.
I left it off because it is a credit rather than a balance and the tab was already restructured.
Say if you want it added.

**4. The three delinquency notes I wrote are factual, not collection notes.** The procedure
wants what the balance represents, the most recent attempt to collect, and whether it has been
paid down since close. Mine cover the first and part of the third. The collection story is
yours, Chong Qing Hot Pot especially, where the tenant is disputing its Rent Commencement Date
and has now missed three months, $33,287.79.

**5. All the narrative sections are July's words.** Untouched, and every one needs your read:
New Leases (Chong Quin Hot Pot), Executed Renewals (ABC Store 75, Kona Gear, Café Kona),
Renewals (Big Island Running, Gypsea Gelato), Gross Sales Reporting, Tenant Issues, **Foster's
Fire**, Operation Issues, Capital Projects.

**6. There is no August gross sales report.** July had one. The Gross Sales Reporting section
still carries July's tenant by tenant sales commentary and cannot be updated without the file.

**7. The Foster's Rebuild Costs tab is untouched and stale.** It still shows a balance of
($188,845.26) against $1,301,410.55 received and $1,490,255.81 of expenses paid and forecast.
Meanwhile August booked **$67,632.25 to Loss Against Insurance Claims**, which is the single
biggest swing in the month's owner expenses. That tab needs updating and I have no source for it.

**8. Two percentages will display with an odd sign.** On the Net Income row the budget is
negative, ($53,508.91). The template's formula is variance divided by budget, so a favourable
$29,193.12 variance shows as **-54.56%** rather than +54.56%. Same on the YTD column, -159.64%.
The dollars are right and the formula is Athena's, so I left it alone. Worth knowing before
anyone reads the percentage as bad news, because August actually beat budget.

**9. Spell check.** Has to be run in Excel, I cannot do it from here.

---

## Also worth knowing

**August was a good month and the report should say so.** Net income came in at ($24,315.79)
against a budgeted ($53,508.91), so $29,193.12 better than plan. Year to date is $96,573.23
against a budgeted loss of ($161,915.38), $258,488.61 ahead. Revenue beat budget by $51,678.44,
driven by past due rent finally arriving from Humpy's ($24.7K), Foster's ($18.7K) and Laverne's
($18.4K), plus parking running $14.2K over.

**Q Pot paid nothing**, ($27,672.53) against budget, base rent and NNN both missed.

**Parking is the standout for the year.** $65,950.10 over budget year to date, on a $240,000
annual budget.

**The income statement carries the open period warning.** "Report includes an open period.
Entries are not final."

**How the file was edited.** Patched inside the zip at XML level. All 58 entries present in
original order, the embedded logo byte identical, zip integrity clean, opens correctly, and
`fullCalcOnLoad` is set so Excel recomputes every formula on open.
