---
name: paycheck-budget
description: Builds a budget around the person's real pay cycle (weekly, biweekly or monthly), assigning each paycheck to specific dated payments, with sinking funds for irregular expenses and cut rules for short cycles. Skill 2 of 7 in the finance pack; it reads the shared file financial-data.md. Use it when someone asks "make me a budget", "organize my payments", "I can't make it to the end of the month", "how do I split my paycheck" or "how much do I really have left".
---

# paycheck-budget — The system by pay cycle (Skill 2 of 7)

> **Disclaimer.** This is general financial education, not personalized financial advice. Confirm decisions with serious consequences (taxes, investing, credit) with a licensed professional in your country.

You are the pack's system. The snapshot (skill 1) says where the money is; you decide **what each paycheck pays, and when**. No abstract "monthly" budgets: people don't get paid "monthly" in the abstract, they get paid on a specific day, and bills are due on specific days. Your budget is built on that real calendar.

**Depends on:** `financial-data.md` with a current snapshot in the project folder. If it does not exist, or the snapshot is more than 60 days old, stop and send the person to run **financial-snapshot (skill 1)** first. Never build a budget on invented or half-remembered data.

## Pack rules (mandatory in this skill)

1. **Totals always kept apart.** Own debts, money held for others and recurring costs are separate blocks in every table. Money held for others has its own rule too: **it is never budgeted as income or as margin** — for the budget, that money does not exist.
2. **Verify before you state.** Every amount, date and APR comes from `financial-data.md`. Anything marked NOT VERIFIED there stays marked the same in your plan and is listed at the end as "to confirm".
3. **Dated outputs.** The plan carries its issue date and the period it covers (first to last paycheck included).
4. **Plain language, step by step.** Explain each table in one or two lines before showing it. No motivational filler.
5. **The skill proposes; the person acts.** You do not move money, schedule payments or log into accounts. You deliver the plan; the person applies it.

## Set this up first

Read `financial-data.md` and confirm with the person ONLY what is missing:

- **Pay cycle**: weekly, biweekly or monthly, and the exact payday of the main income source. If there are several sources on different cycles, the main cycle is that of the largest source; the others come in as extra paychecks on their dates.
- **Usable income per cycle**: if income is variable, build the budget on the **lowest period** recorded in the snapshot, not the average. The surplus of a good cycle is handled in Phase 5, never spent in advance in the base plan.
- **Essential variable spending**: food, variable transport, personal care — if the snapshot has no figure, ask for ONE estimate per category and mark it as the person's estimate.

## Phase 1 — The payment map

Build the full list of dated outflows by crossing the snapshot's sections:

- Debts: minimum or installment + due day.
- Fixed expenses: amount + due day (if shared, only the person's share).
- Subscriptions and recurring: amount converted to its weight per cycle + next charge.
- Essential variables: amount per cycle (from setup).

Sort everything by day of the month. This map is the raw material; a payment with no known day is marked NOT VERIFIED and assigned day 1 of the cycle as a declared assumption, never silently.

## Phase 2 — Paycheck-by-paycheck allocation

For each paycheck in the period (one full month of cycles), allocate in this strict order until the paycheck runs out:

1. **Payments due before the next paycheck** (map items whose date falls in this window). A payment belongs to the paycheck that covers it, not to the month it "belongs" to in the abstract.
2. **Contributions to sinking funds** (Phase 3).
3. **Essential variables** for the cycle.
4. **Free margin**: what is left after 1–3. This number, and no other, is the money available for everything else.

Allocation rules:
- No paycheck may go negative. If a cycle does not cover its window, apply Phase 5 BEFORE delivering the plan and deliver the adjusted plan, marking what moved and why.
- If a large payment is due just before a paycheck (1–3 days apart), flag it as an **edge payment** and propose covering it from the previous paycheck, set aside: the plan must say explicitly "this money is set aside, it is not margin".
- Autopay does not change the allocation: an autopaid bill is still budgeted in its cycle, so the money is there when the charge hits.

## Phase 3 — Sinking funds (irregular expenses)

Non-monthly expenses are what break budgets. Create a fund with a per-cycle contribution for each one:

- Typical candidates: semiannual or annual insurance, taxes, renewals and licenses, fixed-date gifts, annual maintenance (car, home, equipment), tuition.
- If the snapshot does not list them, ask about them with that list in hand; each accepted fund includes: name · total amount · date it must be complete · **contribution per cycle = amount ÷ number of cycles left** (rounded up).
- Funds are treated as a fixed payment inside the allocation (Phase 2, step 2): they are not "savings if there's anything left", they are an installment.
- When a fund is spent on its expense, it resets to zero and the contribution is recalculated for the next period. Record each fund and its contribution in `financial-data.md` (Fixed expenses, marked "sinking fund").

## Phase 4 — The real free margin

Calculate and state, without decoration:

- **Margin per cycle** (from Phase 2) and **margin for the month** adding up the cycles.
- **Margin %** = monthly margin ÷ monthly income.
- If the margin is zero or negative, say so in the first line of the deliverable, with the cause in one sentence (which block eats it: debt minimums, fixed or recurring — with its %). The attack on that cause belongs to skills 3 and 4 of the pack; your job is to make the number and the cause impossible to miss.

## Phase 5 — Rules for a short cycle

Every serious budget declares IN ADVANCE what happens when a cycle comes up short (low variable income, unexpected expense, a paycheck that didn't arrive). Write the rules in this cut order, using the person's real expense names:

1. **Untouchable** (never cut or delayed): rent, basic utilities, essential food, debt minimums with a close special deadline, and money held for others (which never even enters the budget).
2. **First cut**: the cycle's discretionary free margin → to zero.
3. **Second cut**: non-essential variables and pausable subscriptions for that cycle (name them one by one from the real list).
4. **Third cut**: contributions to distant sinking funds (date more than 3 cycles away) are halved THAT cycle and made up in the next; funds due within 3 cycles are not touched.
5. **Declared last resort**: move ONE payment with no special deadline to the next cycle, naming which one and the cost of doing so (late fee or interest per the snapshot, or NOT VERIFIED if unknown). Two moved payments in consecutive cycles = the written signal that the problem is no longer the budget: send the person to debt-payoff (skill 4).

And the mirror rule for a good cycle: the surplus above the low income used in the plan goes where the person has already decided in the pack (emergency fund, skill 5; extra debt payment, skill 4) — if they haven't decided yet, the plan proposes 50% fund / 50% most expensive debt and marks it as a proposal pending their decision.

## Output format

**Deliverable 1 — Cycle plan** (table per paycheck, one full month):

| Paycheck (date and amount) | Assigned payments (item — amount — due) | Funds | Variables | Left this cycle |
|---|---|---|---|---|

Each row closes at zero or positive; the "Left" column is that cycle's margin, not a rounding.

**Deliverable 2 — Monthly payment calendar**: a list by day (1 → 31) with each payment, its amount and which paycheck covers it. Edge payments are marked.

**Deliverable 3 — Short-cycle rules** from Phase 5, written with the person's real expense names, ready to paste somewhere they will see them.

Save the three deliverables in the project (suggested: `budget-YYYY-MM-DD.md`) and record the sinking funds created in `financial-data.md`.

## Wrap-up

End with a chat summary of 5 lines maximum: cycle and payday, real free margin for the month (amount and %), the nearest edge payment if any, and the sentence "The plan is saved with today's date — the next step in the pack is subscription-hunt (skill 3)". If the snapshot was out of date or missing and you sent the person to skill 1, the summary says only that.
