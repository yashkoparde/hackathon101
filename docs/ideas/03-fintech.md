---
title: Fintech
author: yashkoaprde
part_of: Yash Hackathon Guide
---

# Fintech

[← Back to Idea Index](00-IDEA-INDEX.md) · [← AI & Agents](02-ai-and-agents.md)

| Idea | Problem | MVP Demo | Advanced Scope | Anti-pattern |
|---|---|---|---|---|
| **Irregular Income Budgeting Tool** | Standard budgeting apps assume a steady paycheck : freelancers, gig workers, and commission-based earners are poorly served by "spend X per month" logic. | Input variable income history → calculate a safe "baseline" spending level using a rolling average/percentile approach → flag months that are meaningfully above/below baseline. | | Cut: bank account integration (use manual entry or CSV upload for the demo). Add if time allows: a "safe to spend today" daily number. |
| **Group Expense Splitter with Debt Simplification** | Splitting group expenses across many transactions (a trip, a shared house) creates a tangled web of who-owes-whom that's tedious to settle. | Log expenses per group → compute net balances → run a debt-simplification algorithm to minimize total settling transactions → show before/after transaction count as your "wow" number. | | Cut: real payment integration. Add if time allows: multi-currency support. |
| **Subscription Audit Agent** | People accumulate recurring subscriptions and lose track of what they're paying for, especially free trials that silently convert. | Parse a mock/sample transaction history → detect recurring charges → flag likely-forgotten subscriptions (e.g., low usage signal, first charge after a "free trial" pattern) → show total recoverable savings. | | Cut: real bank integration (use a realistic synthetic transaction CSV). Add if time allows: one-click cancellation instruction drafts per service. |
| **Microloan Readiness Score for the Unbanked/Underbanked** | Traditional credit scoring excludes people with thin or no formal credit history, even when they have consistent, demonstrable financial behavior (rent payments, utility bills, informal income). | Accept alternative data inputs (rent payment history, utility bills, informal income records) → compute a transparent, explainable readiness score → show exactly which factors drove the score, not a black box. | | Cut: real lender integration. Add if time allows: a "what would improve your score" recommendation engine. |
| **Small Business Cash Flow Forecaster** | Small business owners often don't see cash crunches coming until they're already in one : accounting software shows the past, not a forecast. | Input historical income/expenses (CSV or manual) → project forward using seasonality/trend → visually flag weeks where projected cash dips below a safety threshold. | | Cut: accounting software integration. Add if time allows: "what if" scenario sliders (e.g., delay a big purchase, add a new client). |

---
Maintained by [@yashkoaprde](https://github.com/yashkoaprde)
