# Monthly reports, in plain English

Emma's guide. Written 2026-09-08 off the Bell Medical August 2026 run.

There is a second file next to this one called `WORKFLOW.md`. That one is CC's technical checklist.
This one is for you.

---

## What this report actually is

Once a month the owner of each property gets a package. The heart of it is a four page
**Executive Summary** that answers one question:

> "You own this building. Here is what it earned this month, here is what it cost, here is why
> that is different from what we told you to expect, and here is what is going on."

The owner already gets the raw financial statements. They do not want to read them. The Executive
Summary is where a person explains the numbers.

**The budget is the promise. The report explains the gap between the promise and reality.**

---

## The four pages

| Page | What it holds |
|---|---|
| 1 | The financial table, then written commentary on income, operating expenses and owner expenses. Then tenant issues and operational issues. |
| 2 | Renewals coming up, new leases signed, legal, property highlights, capital projects |
| 3 | Tenant delinquency, anyone owing over $2,000 |
| 4 | Insurance certificate tracking (COI) |

---

## The financial table

Six lines, and they stack. Each one flows into the next:

```
   Total Income                     what came in
 - Total Operating Expenses         running the property (landscaping, janitorial, utilities)
 ─────────────────────────
 = Gross Cash Flow

 - Total Owners Expense             costs charged to the owner, not the tenants
 - Total Interest Expense           the mortgage interest
 ─────────────────────────
 = Net Income                       what the owner actually made
```

Every line shows six things: this month's **Actual**, this month's **Budget**, the **Variance**
between them, the **% Change**, and then the same three for the **year to date**.

**Sanity check you can do in your head.** Income minus operating expenses must equal gross cash
flow. Gross cash flow minus owner expenses minus interest must equal net income. If it does not,
something is wrong. Do not send it.

### The one thing that trips people up: which sign is good

For **income**, Actual minus Budget. Collecting more than budget is positive and good.

For **expenses**, Budget minus Actual. Spending *less* than budget is positive and good.

So a positive number is always good news and a negative number in parentheses is always bad news,
no matter which row you are looking at. Parentheses mean "this hurt the owner."

---

## Writing the commentary

This is the actual work, and it is the same move three times: for income, for operating expenses,
and for owner expenses. Each gets an MTD (month) paragraph and a YTD (year to date) paragraph.

**The shape, every time:**

```
[MTD or YTD] [Income / Operating Expenses] is [over/under] budget by [$X.XK] due to:
-($X.XK) The biggest reason
-($X.XK) The next biggest reason
-($X.XK) The one after that

Offset by:
-$X.XK The thing that went the other way
```

### What "offset by" means

The headline is a total. Underneath it, individual tenants or expense lines push in opposite
directions. **"Offset by" is where you list the ones pushing the good way**, partially cancelling
the bad ones.

August income is the clean example:

| | Budget | Paid | Effect |
|---|---|---|---|
| Vacant suites | 15,426.24 | 0.00 | (15,426.24) |
| AZ Sports & Spine | 5,028.64 | 3,448.43 | (1,580.21) |
| AZ Trim Clinic | 0.00 | 2,633.30 | **+2,633.30** |
| OMBI | 15,046.72 | 15,105.15 | **+58.43** |
| **Total** | **35,501.60** | **21,186.88** | **(14,314.72)** |

The vacancies and the short payment are the damage. AZ Trim Clinic paying $2,633 that was never
budgeted (they moved in during June, after the budget was written) is the offset. Without it the
month would have missed by $17K instead of $14.3K.

### The rule that keeps you honest

**Your bullets have to add up to your headline.** Roughly, in thousands, but they have to get
there. If they do not, you have missed a driver and the owner will find it.

Small items under a few hundred dollars can be left off, they round to nothing at this scale. Just
know why your bullets are a little short and be able to say so.

### Where the reasons come from

You do not have to invent them. Athena's own spreadsheet already has them.

Open `802 Bell Medical - MM.YY.xlsx`, tab **`Variance`**. There is a column block per month, and
inside each one a **Comments** column where the accounting team has already written things like
"BAS $2,602.57 & NNN $380.51 05/26 & 06/26 Past due paid". Your job is to translate those into the
report's format, not to work them out from scratch.

For expenses, the reasons are the individual line items on the income statement. Look for the rows
with the biggest gaps and name them.

### The shorthand codes

| Code | Means |
|---|---|
| BAS | Base rent |
| NNN | Triple net, the tenant's share of operating costs |
| CAM | Common area maintenance |
| STX | Sales tax |
| LAT | Late charge |
| SGN | Pylon sign charge |
| SDP | Security deposit paid |
| TT | Tenant |

---

## The step by step

### 1. Check what you actually have

Open the month's folder and see what is in it. A complete package is about 24 files. August 2026
arrived with 10. **Do not assume everything is there.** If something is missing, say so out loud
rather than quietly working around it.

### 2. Find the income statement

`03.Comparative Income Statement.pdf` is the one you want. Every number in the financial table
comes from it.

If it is not in the folder, it is also sitting on the **`IS` tab** of
`Bell Medical Monthly Schedules MM.YY.xlsx`. That is where August's came from.

### 3. Check the period is closed

Look at the top of the income statement. If it says:

> "Report includes an open period. Entries are not final."

then accounting is still posting to that month and your numbers will move. Ask before you build on
them. This is the single easiest way to send an owner a number that changes next week.

### 4. Fill in the financial table

Straight off the income statement, no retyping if it can be avoided:

| Report line | Income statement line |
|---|---|
| Total Income | TOTAL INCOME |
| Total Operating Expenses | TOTAL COMMON AREA EXPENSE |
| Gross Cash Flow | GROSS CASH FLOW |
| Total Owners Expense | TOTAL OWNER EXPENSES |
| Total Interest Expense | TOTAL INTEREST EXPENSE |
| Net Income | NET INCOME |

Then run the sanity check from above.

### 5. Write the six commentary paragraphs

Income MTD and YTD, operating expenses MTD and YTD, owner expenses MTD and YTD. Use the shape and
the sources described above. Check each one adds up.

### 6. Update the delinquency page

From `04.Aged Delinquencies.pdf` (or `AGED REPORT.pdf`). **Only tenants owing over $2,000.** For
each one, the balance and a sentence on what is being done about it.

Also compare against last month. If a balance grew, say so. August's grew from $8,400.96 to
$10,100.71 and that belongs in the report.

### 7. Update the narrative sections

Renewals, new leases, legal, property highlights, capital projects. These come from **you**, not
from a spreadsheet. What happened at the property this month?

Cross check renewals against `02.Rent Roll with Lease Options.pdf` for the real expiration dates
and rents. The rent roll is generated by the system and is the source of truth. The summary is
typed by hand and drifts.

### 8. Update the month on every tab

There are seven tabs and the month appears in a header on nearly all of them. Easy to miss one.

### 9. Have it reviewed before it goes out

Owner facing. Nothing leaves without a second set of eyes.

---

## Things to watch for

These all actually happened on the first run:

- **A file named for the new month that is last month's file renamed.** The August Executive
  Summary was a byte for byte copy of July's, still reading "July 2026" inside. Always open it and
  look.
- **Numbers in the header nobody can source.** Square feet and percent leased on the summary
  matched no report in either month's package. Check them against the rent roll.
- **Lease dates that disagree with the rent roll.** The summary said two tenants expired 10/31/26,
  the rent roll said March 2027. Trust the rent roll, confirm, then fix the summary.
- **Narrative sections quietly carried forward.** Text describing work that finished in March was
  still in the July report. If a section has not changed in five months, it probably should have.
- **A tab dated a year stale.** The COI tab still said August 2025.

None of this means anyone is careless. Reports get built from last month's copy and small things
ride along. Catching them is part of the job.

---

## Who does what

**CC** reads the files, builds the table, drafts all six commentary paragraphs, updates the
delinquency page, and lists anything that does not reconcile.

**Emma** supplies what happened at the property, resolves anything CC flags, reviews, and sends.

CC never sends anything to an owner.
