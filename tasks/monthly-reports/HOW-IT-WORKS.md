# Monthly reports: how to do one yourself

Emma's guide. Written 2026-09-08, rewritten 2026-09-09 as a hands on procedure.
Worked examples use Bell Medical, August 2026.

`WORKFLOW.md` next door is CC's technical checklist. **This** one is yours.

---

## Part 1: What the report is

Once a month the property owner gets a package. The heart of it is a four page **Executive
Summary** that answers one question:

> "You own this building. Here is what it earned, what it cost, why that differs from what we
> told you to expect, and what is going on."

The owner already receives the raw financial statements and does not want to read them. The
Executive Summary is where a person explains the numbers.

**The budget is the promise. The report explains the gap between the promise and reality.**

### The four pages

| Page | Tab in the workbook | What it holds |
|---|---|---|
| 1 | Executive Summary | Financial table, then written commentary. Then tenant and operational issues. |
| 2 | Executive Summary (lower) | Renewals, new leases, legal, property highlights, capital projects |
| 3 | Tenant Delinquency | Anyone owing over $2,000 |
| 4 | Tenant COI Tracking | Insurance certificate compliance |

### How the financial table stacks

```
   Total Income                  what came in
 - Total Operating Expenses      running the property (landscaping, janitorial, utilities)
 ─────────────────────────
 = Gross Cash Flow

 - Total Owners Expense          costs charged to the owner, not recovered from tenants
 - Total Interest Expense        mortgage interest
 ─────────────────────────
 = Net Income                    what the owner actually made
```

### Variance, positive and negative: the whole thing in one rule

**Variance** means the difference between what you expected and what happened. That is the whole
word. You expected $35,502 in rent, you got $21,187, the gap is about $14,300. That gap is the
variance.

There is exactly one rule to remember:

> ## Positive is good news. Parentheses are bad news.

Every row. Both columns. If you see `(14,315)` something went wrong. If you see `139` something
went right.

**You do not have to work out whether more is good or less is good on each line.** The spreadsheet
already handled that. Your job is reading the sign, not calculating it.

For the curious, here is why it needs handling at all. For rent, *more* is good. For expenses,
*less* is good. Two opposite ideas. So the sheet subtracts in opposite directions:

| | Formula | Example |
|---|---|---|
| Income | Actual − Budget | Collected 21,187, expected 35,502, so **(14,315)**, bad |
| Expenses | Budget − Actual | Budgeted 11,728, spent 13,068, so **(1,340)**, bad |

Both came out negative. Both are bad. The formula flips so the *meaning* does not. That awkward
math exists precisely so you never have to think about it.

---

## Part 2: Before you start

Have these five things open:

| # | File | You need it for |
|---|---|---|
| 1 | `802 - MM.YY Executive Summary.xlsx` | This is what you are filling in |
| 2 | `03.Comparative Income Statement.pdf` | Every number in the financial table |
| 3 | `802 Bell Medical - MM.YY.xlsx`, **Variance** tab | The reasons behind the income numbers |
| 4 | `04.Aged Delinquencies.pdf` | Page 3 |
| 5 | `02.Rent Roll with Lease Options.pdf` | Checking lease dates and rents |

**If #2 is missing** (it was for August), the same report lives on the **`IS` tab** of
`Bell Medical Monthly Schedules MM.YY.xlsx`. Open that tab and you will see it calls itself
"Comparative Income Statement" right in the header. Same report, different container.

---

## Part 3: The cell map

Every place you type, and nowhere else.

### Tab: Executive Summary

| Cell | What goes in it |
|---|---|
| `A4` | The month, e.g. `August 2026` |
| `B12` `C12` `F12` `G12` | Total Income: MTD actual, MTD budget, YTD actual, YTD budget |
| `B13` `C13` `F13` `G13` | Total Operating Expenses, same four |
| `B14` `C14` `F14` `G14` | Gross Cash Flow, same four |
| `B15` `C15` `F15` `G15` | Total Owners Expense, same four |
| `B16` `C16` `F16` `G16` | Total Interest Expense, same four |
| `B17` `C17` `F17` `G17` | Net Income, same four |
| `A22` | Income commentary, MTD |
| `A23` | Income commentary, YTD |
| `A25` | Operating expenses commentary, MTD |
| `A26` | Operating expenses commentary, YTD |
| `A28` | Owner expenses commentary, MTD |
| `A29` | Owner expenses commentary, YTD |
| `A32` | Tenant Issues |
| `A35` | Operational Issues |
| `B38` | Renewals, first tenant block |
| `B39` | Renewals, second tenant block |
| `B41` | New Leases / Completed Renewals |
| `A43` | Legal (usually `N/A`) |
| `A46` | Property Highlights and Trends |
| `A49` | Capital Projects / Tenant Improvements |

> ### Do not type in columns D, E, H or I
>
> Those four calculate themselves. `D12` is `=+B12-C12`, `E12` is `=IF(C12=0,"N/A",D12/C12)`,
> and H and I do the same for the YTD side. **You fill in B, C, F and G. The variance and the
> percentage appear on their own.** If you type over them you break the sheet for every future
> month.

### The other tabs, month header only

| Tab | Cell |
|---|---|
| Title Sheet | `B9` |
| Tenant Delinquency | `A4` |
| Photos | `A4` |
| Tenant COI Tracking | `A4` |
| Tenant Maintenance Tracking | `A3` |

### Tab: Tenant Delinquency

| Cell | What goes in it |
|---|---|
| `A14` | Tenant name |
| `B14` | Balance owed |
| `C14` | What is being done about it |
| `B15` | Total. **This is a formula**, `=SUM(B14:B14)`. Leave it. Widen the range if you add rows. |

---

## Part 4: Doing it, step by step

### Step 1. Make your working copy

Copy **last month's** Executive Summary workbook. Rename it for the new month.

Then **open it and look at the month inside**. In August the file was named `08.26` but was a
byte for byte copy of July's and still said "July 2026" on every tab. The rename is not the work.

### Step 2. Change the month on all seven tabs

Use the cell map above. Seven tabs, easy to miss one. Click each tab and check.

### Step 3. Fill in the financial table

Open the Comparative Income Statement next to the workbook. Six lines to find:

| Type into row | Find this line on the income statement |
|---|---|
| 12 | TOTAL INCOME |
| 13 | TOTAL COMMON AREA EXPENSE |
| 14 | GROSS CASH FLOW |
| 15 | TOTAL OWNER EXPENSES |
| 16 | TOTAL INTEREST EXPENSE |
| 17 | NET INCOME |

Note row 13. On the income statement it is called **TOTAL COMMON AREA EXPENSE**, but on the
report it is labelled **Total Operating Expenses**. Same thing, different name. This is the one
people get wrong.

For each line, type four numbers: current period actual and budget into B and C, year to date
actual and budget into F and G. Watch the variance and percentage fill themselves in.

**August, so you can check yourself:**

| Row | | MTD actual | MTD budget | YTD actual | YTD budget |
|---|---|---|---|---|---|
| 12 | Total Income | 21,186.88 | 35,502 | 163,909.73 | 220,747 |
| 13 | Total Operating Expenses | 13,067.63 | 11,728 | 132,475.76 | 90,609 |
| 14 | Gross Cash Flow | 8,119.25 | 23,774 | 31,433.97 | 130,138 |
| 15 | Total Owners Expense | 1,672.74 | 1,034 | 32,691.11 | 6,430 |
| 16 | Total Interest Expense | 4,368.22 | 4,508 | 34,556.98 | 35,642 |
| 17 | Net Income | 2,078.29 | 18,232 | (35,814.12) | 88,066 |

### Step 4. Prove it before you go further

Two checks, on a calculator, both columns:

```
  Total Income  -  Total Operating Expenses  =  Gross Cash Flow
      21,186.88  -  13,067.63                =  8,119.25       ✓

  Gross Cash Flow - Owner Expenses - Interest  =  Net Income
      8,119.25    -  1,672.74      -  4,368.22 =  2,078.29     ✓
```

Do the same for YTD. **If either does not tie, stop.** You have a wrong number and everything
downstream inherits it.

### Step 5. Write the six paragraphs

Same move six times. The shape never changes:

```
[MTD or YTD] [Income / Operating Expenses] is [over/under] budget by [$X.XK] due to:
-($X.XK) The biggest reason
-($X.XK) The next biggest
-($X.XK) The one after that

Offset by:
-$X.XK The thing that went the other way
```

**Full worked example follows in Part 5.** Read that before writing your first one.

### Step 6. The delinquency page

From the aged report. **Only tenants owing more than $2,000.** For each: name, balance, and a
sentence on what is being done.

Then compare against last month and say if it moved. August went from $8,400.96 to $10,100.71,
and an owner needs to be told that.

### Step 7. The narrative sections

Renewals, new leases, legal, property highlights, capital projects. **These come from you.** No
spreadsheet has them. What actually happened at the property this month?

Check renewals against the rent roll for real expiration dates and rents. The rent roll is
generated by ATHENA and is the source of truth. The summary is typed by hand and drifts.

If a section has not changed in months, ask whether it should still be there. The July report
still described a contractor dispute that closed in March.

### Step 8. Final pass, then hand it over

- All seven tabs say the right month
- Both arithmetic checks tie, MTD and YTD
- Every commentary paragraph's bullets add up to its own headline
- No em dashes or en dashes anywhere, this goes to an owner
- Property name written in full, never the in-house nickname

Save, then get a second set of eyes. **Owner facing work does not leave on one person's say so.**

---

## Part 5: Writing a commentary paragraph, worked all the way through

This is the part that feels like magic until you have done it once. It is not.

### What you are looking at

Open `802 Bell Medical - 08.26.xlsx`, tab **`Variance`**. It is wide. There is a block of columns
per month. For August, look at columns **AL, AM, AN, AO**: Budget, Payment, Variance, Comments.

Here is what those rows actually say:

| Tenant | Budget | Paid | Variance | Athena's comment |
|---|---|---|---|---|
| OMBI | 15,046.72 | 15,105.15 | +58.43 | SLS $58.44 Budget vs Pmt |
| AZ Sports & Spine | 5,028.64 | 3,448.43 | (1,580.21) | BAS $2,602.57 & NNN $380.51 05/26 & 06/26 Past due paid / LAT $200.00 received / BAS ($4,505.74) & NNN ($277.09) Short Pmt |
| AZ Trim Clinic | 0.00 | 2,633.30 | +2,633.30 | BAS $1,426.58 & NNN $1,206.72 Not Budgeted (NEW TT) |
| Vacant | 15,426.24 | 0.00 | (15,426.24) | BAS ($9,550.56) & NNN ($5,875.68) No Pmt - Vacant |
| **Total** | **35,501.60** | **21,186.88** | **(14,314.72)** | |

**The reasons are already written for you.** You are not working out why anyone paid short. You
are translating what accounting already wrote into the report's format.

### Now build the paragraph

**First, the headline.** Total variance is (14,314.72). Round to thousands: **($14.3K)**. It is
negative, so income is **under** budget.

> MTD Income is under budget by ($14.3K) due to:

**Second, sort the tenants biggest to smallest, and split them by direction.**

Hurting: Vacant (15,426.24), AZ Sports & Spine (1,580.21)
Helping: AZ Trim Clinic +2,633.30, OMBI +58.43

**Third, list the hurting ones, largest first**, with a short reason lifted from the comment:

> -($15.4K) Vacant - No Pmt - Vacant
> -($1.6K) Arizona Sports & Spine Physicians - Short Pmt

**Fourth, the helping ones under "Offset by".** This is the whole answer to your question about
offsetting. It is where you list what pushed the other way:

> Offset by:
> -$2.6K Arizona Trim Clinic - Not budgeted (NEW TT)

OMBI's $58 rounds to nothing at this scale, so it gets left off.

**Finished paragraph:**

```
MTD Income is under budget by ($14.3K) due to:
-($15.4K) Vacant - No Pmt - Vacant
-($1.6K) Arizona Sports & Spine Physicians - Short Pmt

Offset by:
-$2.6K Arizona Trim Clinic - Not budgeted (NEW TT)
```

### What "offset" actually means, the grocery version

Say you budget $500 for groceries and spend $560. You overspent by $60.

Now look inside that $60. Meat ran $100 over. Produce came in $40 under.

```
  meat        +100  over
  produce      -40  under      <- this offsets
  ──────────────────
  net           60  over
```

The produce **offset** part of the meat. If someone asked, you would say: *"I am $60 over, mostly
meat, offset by coming in under on produce."*

That is exactly what "Offset by" means in the report. Same idea, bigger numbers, other people's
money.

### Why it matters here

Without AZ Trim Clinic, August would have missed budget by about $17K. They are a new tenant who
moved into Suite 102B in June, after the budget was written, so every dollar they pay is money
nobody forecast. That $2,633 is why the month missed by $14.3K instead of $17K.

An owner reading only "we missed by $14.3K" learns nothing. An owner reading the offset learns:
*the vacancies are the problem, one tenant is struggling, and we filled a suite that is already
paying.* Same number, completely different message.

### The rule that keeps you honest

**Your bullets must add up to your headline.**

```
-15.4  -1.6  +2.6  =  -14.4   against a headline of -14.3   ✓ close enough
```

The $0.1K gap is OMBI's $58. If your bullets do not roughly reach the headline, **you have missed
a driver** and the owner will find it before you do.

Items under a few hundred dollars can be left off. Just know which ones you dropped and why.

### The expense paragraphs work identically

Only the direction flips. Over budget is bad, so "offset by" lists the lines that came in
**under** budget. The reasons come from the individual rows on the income statement instead of
the Variance tab. Find the biggest gaps and name them.

August operating expenses, for practice:

```
MTD Operating Expenses are over budget by ($1.3K) due to:
-($1.1K) Electric/Building
-($710) General Maintenance
-($325) Sweeping
-($260) Sidewalk Maintenance
-($193) Landscape - Sprinkler Repairs

Offset by:
-$840 Landscape - Tree Trimmings
-$335 HVAC Maintenance
```

### The shorthand codes

| Code | Means |
|---|---|
| BAS | Base rent |
| NNN | Triple net, the tenant's share of operating costs |
| CAM | Common area maintenance |
| STX | Sales tax |
| SLS | Sales |
| LAT | Late charge |
| SGN | Pylon sign charge |
| SDP | Security deposit paid |
| TT | Tenant |
| MTD / YTD | Month to date / year to date |

---

## Part 6: Things to watch for

All of these actually happened on the first run:

- **A file named for the new month that is last month's file renamed.** Open it and read the
  month inside before you trust it.
- **"Report includes an open period. Entries are not final."** If the income statement says this,
  accounting is still posting and your numbers will move. Ask before building on them.
- **Header numbers nobody can source.** Square feet and percent leased on the summary matched no
  report in either month. Check them against the rent roll.
- **Lease dates that disagree with the rent roll.** The summary said two tenants expired 10/31/26,
  the rent roll said March 2027. Believe the rent roll, confirm, then fix the summary.
- **Narrative that quietly carried forward.** Text about work finished in March was still there
  in July.
- **A tab dated a year stale.** The COI tab still said August 2025.
- **A short package.** August arrived with 10 files instead of 24. Count before you start.
- **One variance cell subtracts the wrong way round.** On the Operating Expenses row, the MTD
  variance (`D13`) correctly uses Budget minus Actual, but the YTD variance (`H13`) uses Actual
  minus Budget. The two expense rows right below it, Owner Expense and Interest Expense, both do
  it correctly. So on the July report a $40,527 overspend for the year showed as **positive**
  $40,527, reading like good news.

  **If that line ever seems to break the "positive is good" rule, the rule is fine and the cell is
  wrong.** Raised 2026-09-09, not yet decided. It affects Athena's standard template, so it is not
  a Bell Medical question, it is a whole company question.

None of this means anyone is careless. Reports get built from last month's copy and small things
ride along. Catching them is the job.

---

## Part 7: How Emma and CC split this

Emma had never done a monthly report before September 2026. The point of this guide is that she
can do one without CC, and can tell whether CC got it right.

**Always Emma's:** what actually happened at the property (renewals, highlights, capital
projects, tenant conversations), every judgment call, the review, and the sending.

**Always CC's:** reading every page of every file so Emma is not squinting at PDFs, pulling the
figures out with their source cited, checking the arithmetic ties, and flagging anything that
does not reconcile or contradicts another document.

**Negotiable, and it should shift over time:** the typing and the commentary drafting. Early on
CC drafts and Emma corrects. Once the shape is familiar, Emma writes and CC checks. Say which
you want on any given month.

**Never CC's:** sending anything to an owner.

### Good ways to use CC while learning

- "Pull me the six figures for September and tell me where each one came from." Then type them
  in yourself and see if your variances match.
- "I wrote the income paragraph, check my bullets add up."
- "Walk me through the operating expense paragraph before I write it."
- "What changed between last month and this month?"
