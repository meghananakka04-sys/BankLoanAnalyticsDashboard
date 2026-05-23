# Bank Loan Analytics Dashboard
> What separates a profitable lending portfolio from a risky one? This project transforms raw loan data into a structured decision-making system that reveals hidden borrower patterns, portfolio vulnerabilities, and lending concentration risks.

---

## The Problem Nobody Talks About

Banks approve loans. They collect payments. But they rarely ask the right question:

**Are we lending to the right people?**

Most lending dashboards show totals — total funded, total repaid, total loss. But totals hide everything.

A $500M portfolio that's 95% concentrated in one region looks healthy until that region faces an economic downturn. A lending book with 60% of loans going to self-employed borrowers looks profitable until employment becomes unstable. A portfolio with high average interest rates looks strong until you realize you're only getting those rates because you're lending to higher-risk borrowers.

This project investigates what's actually hidden inside lending data.

---

## What This Dashboard Does Differently

Rather than displaying loan metrics in isolation, this project builds a **connected intelligence system** where each dashboard layer answers a specific business question:

| Dashboard Layer | Core Question | Business Impact |
|---|---|---|
| **Portfolio Health** | Are we making money or losing it? | Track funded vs repaid, identify early warning signs in charge-offs |
| **Borrower Segmentation** | Who are we actually lending to? | Understand concentration risk, identify borrower instability signals |
| **Risk Concentration** | Where is our money at risk? | Quantify regional exposure, employment-type dependency, purpose-driven volatility |

---

## Inside the Dashboard

### Layer 1 · Portfolio Command Center
![Summary Dashboard](assets/Summary_dashboard.png)

The first dashboard functions as the operational nerve center.

Rather than overwhelming users with 50 metrics, it isolates the **8 KPIs that actually matter for portfolio health:**
- Funded amount (liquidity deployed)
- Repayment rate (cash flow health)
- Charge-off rate (portfolio quality deterioration)
- Interest rate (yield on risk)
- Debt-to-income ratio (borrower stability)
- Application volume (demand signal)
- MTD movement (month-to-date trends)
- Status segmentation (healthy vs at-risk loans)

**What makes this layer different:** The dashboard separates **charged-off loans from healthy ones**. Most dashboards treat all loans equally. This one asks: *Where is the portfolio actually breaking?* By isolating charged-offs as a distinct layer, you can see whether problem loans concentrate in specific borrower types, regions, or purposes.

---

### Layer 2 · Pattern Recognition Through Segmentation
![Overview Dashboard](assets/Overview_dashboard.png)

The second dashboard shifts from "how much" to "how distributed."

This is where insights emerge.

**Borrower Stability Signals:**
- Employment length (job tenure predicts repayment stability)
- Home ownership (collateral = skin in the game)
- Debt-to-income ratio (financial breathing room)

**Lending Behavior Patterns:**
- Purpose distribution (some loan purposes have inherently higher default rates — personal loans vs home improvement)
- Regional concentration (geographic clustering of risk)
- Loan term trends (shorter terms = lower default risk, but lower yield)
- Monthly lending movement (seasonal patterns reveal market timing)

**Why this matters:** A portfolio that looks balanced overall might have 70% of its funded amount concentrated in three states. A lending book that shows strong repayment rates might hide the fact that 65% of loans are to employed borrowers — meaning economic recession = portfolio collapse.

---

### Layer 3 · The Backend Intelligence System
![Backend Design](assets/Design_sheet.png)

Behind the dashboards sits the analytical engine that powers them.

Rather than building dashboards in isolation, this workbook architecture separates:

**Data layer** → Raw loan records  
**Calculation layer** → Pivot aggregations, KPI formulas, risk scoring  
**Insight layer** → Dashboards that interpret the calculations  

This separation meant:
- Adding a new metric doesn't break existing dashboards
- Slicers in the dashboard automatically trigger recalculation across all dependent metrics
- Portfolio comparisons (MTD vs MoM, charged-off vs healthy) are built into the backend, not manually calculated

---

## What the Data Revealed

### Finding 1: Concentration Risk Is Real
Regional lending concentration determines portfolio stability. A portfolio spread across 50 states is more resilient than one concentrated in 5.

### Finding 2: Employment Type Predicts Stability
Employed borrowers have measurably different repayment patterns than self-employed. A portfolio that skews toward one group has structural risk.

### Finding 3: Purpose Matters More Than Loan Amount
A $50K personal loan defaults at a different rate than a $50K home improvement loan. Loan type drives risk, not just size.

### Finding 4: The Interest Rate Paradox
Higher interest rates attract riskier borrowers. A portfolio with 15% average interest rates isn't healthier — it's riskier. You're compensating for risk exposure with higher yield, which is fine only if default rates stay constant. They usually don't.

---

## Why This Project Matters

**For a lending business:** This dashboard structure separates operational reporting from strategic intelligence. You can track activity daily (Layer 1) while understanding structural portfolio risk quarterly (Layers 2 + 3).

**For the analyst:** Building this taught me that dashboards aren't about pretty charts. They're about asking hard questions and organizing data so the answers become visible.

**For portfolio managers:** This is how you move from "we're profitable" to "we're profitable because we understand our risk."

---

## The Technical Reality

What made this interesting wasn't the Excel formulas — it was the architecture.

Most Excel projects are dashboards bolted onto flat data. This one was different:
- Relational logic between borrower attributes and lending outcomes
- Risk-weighted aggregation (not all loans are equally important)
- Temporal analysis (comparing periods to identify trends)
- Segmentation-driven interpretation (the same $1M portfolio looks different when viewed by region, purpose, and employment type)

The backend contains hundreds of formulas, but the user sees only clean dashboards because the complexity is hidden where it belongs — in the calculation layer.

---

## The Bigger Picture

This project was an early exploration of how **raw data becomes intelligence**.

Raw data: "We funded $500M in loans."  
Interpreted data: "We funded $500M in loans, 65% to employed borrowers in 5 states, with 8% charge-offs concentrated in personal loan purposes."

One is a number. The other is a decision.