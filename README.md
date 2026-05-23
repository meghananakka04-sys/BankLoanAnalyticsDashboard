# Bank Loan Analytics Dashboard
> What separates a profitable lending portfolio from a risky one? This project transforms raw loan data into a structured decision-making system that reveals hidden borrower patterns, portfolio vulnerabilities, and lending concentration risks.

## The Problem Nobody Talks About

Banks approve loans. They collect payments. But they rarely ask the right question:

**Are we lending to the right people?**

Most lending dashboards show totals. Total funded, total repaid, total loss. But totals hide everything.

A $500M portfolio that's 95% concentrated in one region looks healthy until that region faces an economic downturn. A lending book with 60% of loans going to self-employed borrowers looks profitable until employment becomes unstable. A portfolio with high average interest rates looks strong until you realize you're only getting those rates because you're lending to higher-risk borrowers.

This project investigates what's actually hidden inside lending data.

## What This Dashboard Does Differently

Rather than displaying loan metrics in isolation, this project builds a **connected intelligence system** where each dashboard layer answers a specific business question:

| Dashboard Layer | Core Question | Business Impact |
|---|---|---|
| **Portfolio Health** | Are we making money or losing it? | Track funded vs repaid, identify early warning signs in charge-offs |
| **Borrower Segmentation** | Who are we actually lending to? | Understand concentration risk, identify borrower instability signals |
| **Risk Concentration** | Where is our money at risk? | Quantify regional exposure, employment-type dependency, purpose-driven volatility |

## Inside the Dashboard

### Layer 1 · Portfolio Command Center
![Summary Dashboard](assets/Summary_dashboard.png)

The first dashboard functions as the operational nerve center.

Rather than overwhelming users with 50 metrics, it isolates the **8 KPIs that actually matter for portfolio health:**

Funded amount represents liquidity deployed into the lending market.  
Repayment rate reflects overall cash flow health.  
Charge-off rate indicates deterioration in portfolio quality.  
Interest rate measures yield generated from lending risk.  
Debt-to-income ratio helps evaluate borrower stability.  
Application volume acts as a demand indicator.  
MTD movement tracks short-term lending trends.  
Status segmentation separates healthy loans from at-risk loans.

**What makes this layer different:** The dashboard separates **charged-off loans from healthy ones**. Most dashboards treat all loans equally. This one asks: *Where is the portfolio actually breaking?* By isolating charged-offs as a distinct layer, you can see whether problem loans concentrate in specific borrower types, regions, or purposes.

### Layer 2 · Pattern Recognition Through Segmentation
![Overview Dashboard](assets/Overview_dashboard.png)

The second dashboard shifts from "how much" to "how distributed."

This is where insights emerge.

**Borrower Stability Signals**

Employment length helps evaluate repayment stability through job tenure.  
Home ownership introduces a collateral perspective into borrower analysis.  
Debt-to-income ratio reflects financial breathing room available to borrowers.

**Lending Behavior Patterns**

Purpose distribution reveals how certain loan categories carry different default tendencies.  
Regional concentration highlights geographic clustering of lending risk.  
Loan term trends compare risk exposure across shorter and longer repayment durations.  
Monthly lending movement helps identify seasonal lending patterns and timing shifts.

**Why this matters:** A portfolio that looks balanced overall might have 70% of its funded amount concentrated in three states. A lending book that shows strong repayment rates might hide the fact that 65% of loans are to employed borrowers, meaning economic recession could severely affect repayment stability.

### Layer 3 · The Backend Intelligence System
![Backend Design](assets/Design_sheet.png)

Behind the dashboards sits the analytical engine that powers them.

Rather than building dashboards in isolation, this workbook architecture separates:

**Data layer** → Raw loan records  
**Calculation layer** → Pivot aggregations, KPI formulas, risk scoring  
**Insight layer** → Dashboards that interpret the calculations  

This separation meant the reporting structure remained modular and easier to maintain. New metrics could be added without disrupting existing dashboards. Dashboard slicers automatically triggered recalculation across dependent metrics. Portfolio comparisons such as MTD vs MoM and charged-off vs healthy loans were integrated directly into the backend architecture rather than calculated manually.

## What the Data Revealed

### Finding 1: Concentration Risk Is Real
Regional lending concentration determines portfolio stability. A portfolio spread across 50 states is more resilient than one concentrated in 5.

### Finding 2: Employment Type Predicts Stability
Employed borrowers have measurably different repayment patterns than self-employed. A portfolio that skews toward one group has structural risk.

### Finding 3: Purpose Matters More Than Loan Amount
A $50K personal loan defaults at a different rate than a $50K home improvement loan. Loan type drives risk, not just size.

### Finding 4: The Interest Rate Paradox
Higher interest rates attract riskier borrowers. A portfolio with 15% average interest rates isn't healthier. It's riskier. You're compensating for risk exposure with higher yield, which is fine only if default rates stay constant. They usually don't.

## Why This Project Matters

**For a lending business:** This dashboard structure separates operational reporting from strategic intelligence. You can track activity daily through the portfolio layer while simultaneously understanding deeper structural portfolio risks through segmentation and backend analysis.

**For the analyst:** Building this taught me that dashboards aren't about pretty charts. They're about asking difficult questions and organizing data so the answers become visible.

**For portfolio managers:** This is how you move from "we're profitable" to "we're profitable because we understand our risk."

## The Technical Reality

What made this interesting wasn't the Excel formulas. It was the architecture.

Most Excel projects are dashboards bolted onto flat data. This project focused more heavily on relationships between borrower attributes, lending outcomes, repayment behavior, and risk exposure.

The backend architecture integrates:
Relational logic between borrower attributes and lending outcomes  
Risk-weighted aggregation systems  
Temporal trend analysis across reporting periods  
Segmentation-driven interpretation across regions, purposes, and employment categories

The backend contains hundreds of formulas, but the user sees only clean dashboards because the complexity is hidden where it belongs — in the calculation layer.

## The Bigger Picture

This project was an early exploration of how **raw data becomes intelligence**.

Raw data: "We funded $500M in loans."  
Interpreted data: "We funded $500M in loans, 65% to employed borrowers in 5 states, with 8% charge-offs concentrated in personal loan purposes."

One is a number. The other is a decision.