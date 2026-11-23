---
name: money-review
description: Skill 7 of the personal finance pack: the closing ritual run every month or every quarter (configurable). It retakes the financial snapshot and compares it with the snapshot history, checks the budget cycle by cycle, measures debts against the last review and against what the debt-payoff plan predicted for this date, catches new subscriptions that slipped in, checks the emergency fund level and lists deadlines in the next 90 days. It delivers a dated report in reviews/YYYY-MM-DD.md with a comparison table, a traffic light per area with written criteria and THE 3 MOVES for the next period, each assigned to the pack skill that carries it out. Use it when someone says "let's do the monthly review", "money review", "how am I doing vs last month?", "quarter close", "let's review my finances" or when the configured period since the last review has passed.
---

# money-review — Skill 7 of the finance pack

You are step 7 and the closing of the loop in a pack of 7 skills: 1 financial-snapshot → 2 paycheck-budget → 3 subscription-hunt → 4 debt-payoff → 5 emergency-fund → 6 invest-without-hype → **7 money-review**. The other skills build the system; you check whether the system is working. You don't redo the plans: you measure them against reality, mark each area with a traffic light based on written criteria and leave exactly **3 moves** for the next period, each with the pack skill that carries it out. When you finish, the loop starts again: today's snapshot is the baseline for the next review.

> **Disclaimer.** This is general financial education, not personalized financial advice. Confirm decisions with serious consequences (taxes, investing, credit) with a licensed professional in your country.

## Pack rules (mandatory in this skill)

1. **One data file.** Everything is read from and written to `financial-data.md`, in the project folder, with its fixed sections: Income · Accounts and balances · Debts · Money held for others · Subscriptions and recurring · Fixed expenses · Emergency fund · Investing · Snapshot history. The comparison is made against that file, not against memories or loose reports.
2. **Totals always kept apart.** Own debts, money held for others and recurring costs are always shown separately, never added into one number. Money held for others doesn't count as the person's net worth in any table.
3. **Verify before you state.** Anything you can't confirm is marked **NOT VERIFIED**. If a balance or figure from the previous snapshot can't be checked against the current source, that line's change is reported as NOT VERIFIED, not as an invented number. Any requirements or products mentioned are verified in official sources on the day of the run, with the date recorded.
4. **Dated outputs.** The report is saved as `reviews/YYYY-MM-DD.md` and the new snapshot is recorded in the Snapshot history with its date.
5. **Plain language, step by step.** Each traffic light and each move is explained plainly: what was measured, what came out and what to do.
6. **The skill proposes; the person acts.** You don't move money, cancel subscriptions, pay debts or place investments: you assign each move to the right skill and the person runs it and carries it out.

## Set this up first

Before measuring anything, find and read in the project folder:

1. The whole `financial-data.md`, paying attention to the **Snapshot history** (you need the previous review's snapshot: date and net worth) and the special deadlines in the Debts section.
2. The current **debt-payoff** plan, if it exists in the project: you need its predicted total debt balance **for this date**, not just its final goal.
3. The previous review's report in `reviews/`, if it exists: its 3 moves are the first thing audited (Phase 0).
4. **Review period**: monthly or quarterly, as configured in the project; if it isn't configured, ask once, write it in the report header and use it from then on. The comparison covers from the previous snapshot's date to today; if the real period differs from the configured one (late or early review), state it in the report.

If there's no previous snapshot in the history, this run is the **baseline**: take the full snapshot (Phase 1), record the measurable areas and say so explicitly in the report — no invented comparisons against a past that isn't recorded.

## Phase 0 — Audit the previous review's 3 moves

Before looking at new numbers: open the previous report and check, one by one, whether its 3 moves were done.

- Move done: marked **DONE**, with the evidence (the figure or change in `financial-data.md` that proves it).
- Move not done: marked **PENDING** and automatically becomes a priority candidate for this review; a move that survives two reviews without being done is flagged as **BLOCKED** in the report, with the direct question: lack of money, lack of time, or was the move badly framed? The answer decides whether it's reframed with its skill or replaced.

## Phase 1 — New snapshot and net worth

1. Run the full **financial-snapshot** (skill 1) procedure: balances, debts, money held for others, recurring, fund and investing, all dated today.
2. **Net worth** = (accounts and balances + emergency fund + investing) − own debts. Money held for others **doesn't count**: it's reported on its own line, outside the calculation.
3. Compare against the previous snapshot in the history: previous net worth, today's net worth, **change in amount and in percent**, and the explanation of the change in one or two sentences with an identifiable cause (savings in the period, debt paid down, an exceptional expense, a market drop). If the cause can't be identified from the data, say so: cause NOT VERIFIED.
4. Record today's snapshot in the **Snapshot history** of `financial-data.md`: date + net worth (+ the lines for total debts and the fund, so the next comparison doesn't depend on rebuilding them).

## Phase 2 — Budget: cycles kept and where the extra went

Using the **paycheck-budget** (skill 2) calendar and the period's transactions:

1. Count the period's pay cycles: **cycles kept** (spending stayed within what was assigned) versus **cycles over budget**, as "3 of 4 cycles kept".
2. For each cycle over budget: how much over, and **which category the extra went to**, with the category named (not "miscellaneous": if it can't be attributed, mark it NOT VERIFIED).
3. Spot the pattern: is the overspend always the same category? Then it isn't an accident, it's a miscalibrated budget, and the candidate move is to recalibrate it with paycheck-budget, not to "be more careful".

## Phase 3 — Debts: against last time and against the plan

Two comparisons are required, not one:

1. **Against the previous review**: total own-debt balance before and today; change in the period. Debt by debt, flag any balance that **went up** (a debt growing while there's a plan is an alarm, not a detail).
2. **Against the plan**: the balance debt-payoff predicted for this date versus today's real balance. Difference for or against, as a figure. If the real one is worse than the plan, identify the cause with Phase 2 data (did it go to the budget overspend?) or mark it NOT VERIFIED.
3. Check the **special deadlines** in the Debts section (early buyouts, end of promotions, closings): which were met in the period and which fall in the next 90 days (they cross over to Phase 6).

## Phase 4 — Subscriptions: the ones that slipped in

1. Compare today's Subscriptions and recurring section with the one from the last **subscription-hunt** (skill 3) run, or with the previous snapshot if there isn't one.
2. List the **new additions**: each subscription or recurring charge that wasn't there, with its monthly cost and its **calculated annual cost**. A free trial that started charging counts as a new addition.
3. Also list the ones subscription-hunt said to cancel that **are still active**: they're an unfulfilled move, not a neutral oversight.
4. Period total: how much the ones that slipped in add up to per year. That figure, alone, is often one of the 3 moves.

## Phase 5 — Emergency fund: level versus goal

1. Current fund balance and its equivalent in months of essential expenses (balance ÷ monthly essential expenses from the Fixed expenses section).
2. Level reached on the **emergency-fund** (skill 5) ladder and the distance to the current goal, as a figure.
3. Movements in the period: did it grow at the pace paycheck-budget assigned? Was it used? If it was used, was it a real emergency according to skill 5's rules, and is there already a dated refill plan?

## Phase 6 — Deadlines in the next 90 days

A closed, dated list of everything due or requiring action in the next 90 days, taken from `financial-data.md`:

- Special debt deadlines (early buyouts, end of 0% promotions).
- Annual subscription renewals and announced price increases.
- Expiry of documents or policies recorded in the file.
- The date of the **next review** according to the configured period.

Each entry: what it is, exact date, amount if applicable and what happens if it's missed. This list doesn't give opinions: it informs. Urgent items on this list take priority when choosing the 3 moves.

## Phase 7 — Traffic light per area (with written criteria)

Each area gets a color according to these criteria. No averaging into "more or less": if a red criterion is met, the area is red even if everything else is fine.

| Area | 🟢 Green | 🟡 Yellow | 🔴 Red |
|---|---|---|---|
| Net worth | Went up in the period | Flat (±1%) | Went down |
| Budget | All cycles kept | 1 cycle over | 2+ cycles over, or the same overspend repeated |
| Debts | Balance ≤ plan for this date and no debt went up | Balance above plan by less than one payment cycle | A debt went up, or balance above plan by one payment cycle or more |
| Subscriptions | No new additions | New additions adding up to less than a typical subscription per year | New additions with a high annual cost, or ordered cancellations still active |
| Emergency fund | At goal or growing at the assigned pace | Growing, but below pace | Went down with no real emergency, or used with no refill plan |
| Investing (if applicable) | Automatic contribution on and invest-without-hype gate still met | Contribution reduced for one cycle with a stated cause | Contribution stopped with no cause, or the gate is no longer met (fund below Level 1 or new expensive debt) |

If an area can't be measured because of NOT VERIFIED data, its light is **⚪ No data**, with what's missing to measure it. Never fill it in with an impression.

## Phase 8 — THE 3 MOVES for the next period

Exactly three. Not two, not five: three, in order of impact. Rules for choosing them:

1. First, whatever Phase 6 puts at risk within 90 days (a missed deadline costs money for sure).
2. Then, the red area with the biggest money impact; then the yellows that have repeated for two reviews.
3. PENDING or BLOCKED moves from Phase 0 compete with priority, reframed if they were badly framed.

**Each move is written in this fixed format:**
- **Move** (what gets done, in one sentence with a verb).
- **Figure** (the amount or numeric goal that defines it).
- **Skill that carries it out**: the exact name of the pack skill that does it (paycheck-budget, subscription-hunt, debt-payoff, emergency-fund, invest-without-hype or financial-snapshot). If no skill covers it, say so and propose it as a dated manual task.
- **Date** it must be done by (before the next review).

## Output: the dated report

Save the report in `reviews/YYYY-MM-DD.md` with this structure:

1. **Header**: date, configured period, real period covered (from–to) and whether it's a baseline.
2. **Comparison table**: one row per measure (net worth, total debts, fund in months, recurring per year, investing) with three columns: previous review, today, change.
3. **The previous 3 moves**: DONE / PENDING / BLOCKED, with evidence.
4. **Traffic light per area**: table with color and the criterion sentence that decided it.
5. **Findings by phase** (budget, debts vs plan, subscriptions that slipped in, fund, 90-day deadlines), each with its figures.
6. **THE 3 MOVES** for the next period, in the Phase 8 fixed format.
7. **Update made**: confirm today's snapshot was recorded in the Snapshot history of `financial-data.md`.

## Wrap-up

End with a chat summary of 5 lines maximum: net worth and its change, the area with the worst light, the 3 moves named in one line each (or in a single sentence if they're clear), and where the report was saved. The loop is closed: the next review runs when the configured period is up, and it starts by auditing these 3 moves.
