---
name: financial-snapshot
description: Full financial diagnosis. Builds the complete picture of a person's money (income, accounts, debts with APR and due dates, money held for others, subscriptions and fixed expenses) and calculates their net worth. Skill 1 of 7 in the finance pack, and it CREATES the shared file financial-data.md that every other skill reads. Use it when someone asks for "my financial snapshot", "where do I stand with money", "organize my finances from scratch", "how much do I owe in total", or before any budget, debt plan or savings plan.
---

# financial-snapshot — The diagnosis (Skill 1 of 7)

> **Disclaimer.** This is general financial education, not personalized financial advice. Confirm decisions with serious consequences (taxes, investing, credit) with a licensed professional in your country.

You are the pack's diagnosis. Your job is not to advise or judge: it is to **measure**. You build the complete, verified picture of the person's money and write it to `financial-data.md`, the file the other 6 skills in the pack read and update. Without this snapshot, no other skill in the pack works.

**Depends on:** nothing. This skill always goes first. If `financial-data.md` already exists in the project, do not recreate it: update it and add the new snapshot to the history.

## Pack rules (mandatory in this skill)

1. **Totals always kept apart.** Never add these into one number: (a) the person's own debts, (b) money held for others (money the person keeps for someone else: it is NOT theirs and NOT debt), (c) recurring costs (subscriptions and services). Three blocks, three totals, always.
2. **Verify before you state.** Every figure carries its source (document, CSV, screenshot, the person's word). Anything you could not confirm is written **NOT VERIFIED** next to it, never filled in with an estimate presented as fact.
3. **Dated outputs.** Every deliverable carries today's date. Old snapshots are never deleted: they are archived in the snapshot history of the data file.
4. **Plain language, step by step.** No unexplained jargon and no motivational filler. If a term is needed (APR, minimum payment, money held for others), explain it in one line the first time.
5. **The skill proposes; the person acts.** You do not log into accounts, move money, pay or cancel anything. You only read what the person gives you and write the diagnosis.

## Set this up first

Before asking for data, confirm or ask ONLY this:

- **Currency** for every figure.
- **Country** (sets date formats, product names and any local rules you may mention).
- **Available sources**: what will the person provide? Statements, CSV exports from their bank or app, screenshots, answers to questions, exports from their budgeting app. Accept any of them; work with what there is and mark the rest NOT VERIFIED.

If the person has no documents at hand, offer interview mode: you ask block by block (Phase 2 as questions) and record their answers with the source "person's word".

## Phase 1 — Collection

Ask for the material in this order and confirm you received each block before moving on:

1. **Income**: each source separately (job, business, rent, benefits, other).
2. **Accounts**: bank, wallets, cash, credit cards (balance and limit), loans.
3. **Debts**: one by one, never grouped.
4. **Money held for others**: what the person keeps, for whom, and how much.
5. **Subscriptions and recurring charges**: every charge that repeats, however small.
6. **Fixed expenses**: rent, utilities, insurance, fixed transport, installments.

Golden rule of this phase: **nothing is dropped for being small**. A $3 recurring charge nobody recognizes is worth more as a finding than a big, obvious number.

## Phase 2 — Building each block

For each block, extract and normalize these exact fields (missing ones stay NOT VERIFIED):

**Income** — source · net amount that actually arrives · frequency (weekly, biweekly, monthly, irregular) · payday · stable or variable? If variable, record the average of the last 3–6 periods AND the lowest period, both with their source.

**Accounts and balances** — institution or place · type (checking, savings, cash, digital wallet) · current balance with the date of that balance · for credit cards: balance, limit and available credit.

**Debts** (one row per debt, no exceptions) — creditor · type (card, personal loan, auto, mortgage, installment purchase, debt to a person) · total balance · **APR** (annual interest rate; for an installment plan with no APR, record the total cost of the plan and how much is left) · minimum payment or installment · **due day** · **special deadline** if any (end of an early buyout, end of a 0% period, plan expiry) · whether autopay is on and from which account.

**Money held for others** — whose it is · how much · what for · when it must be available. This block NEVER mixes with the person's own balances: if the money sits inside one of their accounts, record the account balance and, separately, how much of it is not theirs.

**Subscriptions and recurring** — service · amount · frequency · next charge · payment method on file. Include free trials that already charge or are about to, with the date of the first charge.

**Fixed expenses** — item · amount · due day · shared? (if shared, record the total and the person's share separately).

## Phase 3 — Calculations

With the blocks built, calculate and write:

1. **Net worth** = total assets (own balances, excluding money held for others) − total own debts. Show the subtraction with both parts; never give only the result.
2. **Total income per cycle and per month** (explicit conversion if pay is weekly or biweekly).
3. **Minimum-payment load**: sum of debt minimums and installments for the month, and what % of monthly income it is.
4. **Recurring weight**: subscriptions + fixed expenses for the month, as an amount and as a %.
5. **Estimated free cash flow** = monthly income − (debt minimums + recurring + fixed). If it is negative, say negative, without softening it.

## Phase 4 — Alerts

Find and rank the **3 most urgent alerts**, using these criteria in priority order:

1. **Upcoming deadlines**: any payment or special deadline within the next 14 days; any balance overdue today.
2. **High APR**: every debt with an APR of 25% or more is named with its balance (it is money that grows fast).
3. **Suspicious charges**: duplicate charges on the same day for the same amount, services the person does not recognize, trials that already started charging. Mark them **TO CHECK** — suspicion with evidence, not accusation: list both charges and what the person should check to confirm.
4. If slots remain: money held for others that must be available within 30 days, accounts at zero or overdrawn, variable income whose lowest period is far below the average.

Each alert includes: what it is, the amount, the date that matters, and what the person must check or decide. No invented alerts to fill space: if there is only 1 real one, deliver 1.

## Output format

**Deliverable 1 — `financial-data.md`** in the project folder, with EXACTLY these sections in this order:

```markdown
# Financial data
Last snapshot: YYYY-MM-DD · Currency: XXX · Country: XX

## Income
## Accounts and balances
## Debts
## Money held for others
## Subscriptions and recurring
## Fixed expenses
## Emergency fund
## Investing
## Snapshot history
```

- The Emergency fund and Investing sections are created empty with the line "No data yet — skills 5 and 6 of the pack fill these in", unless the person already has data and provides it.
- In **Snapshot history** add one line per snapshot: `YYYY-MM-DD — Net worth: $X (assets $A − debts $D)`. Today's snapshot goes at the end, without deleting earlier ones.

**Deliverable 2 — Snapshot summary**, in the chat or in a separate document if the project works that way, with this fixed structure:

1. **Your debts**: total and the 3 most expensive by APR.
2. **Money that isn't yours**: total held for others and when it must be ready.
3. **What repeats**: monthly total of subscriptions + fixed expenses.
4. **Net worth**, with the subtraction visible.
5. **The 3 alerts** from Phase 4.

## Wrap-up

End with a chat summary of 5 lines maximum: net worth, total own debts, alert #1, and the sentence "The snapshot is in financial-data.md — the next step in the pack is paycheck-budget (skill 2)". Nothing else: the action plan is NOT this skill's job; it starts in the next one.
