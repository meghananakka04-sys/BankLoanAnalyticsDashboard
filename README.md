# Bank Loan Analytics Dashboard
> What separates a profitable lending portfolio from a risky one? This project transforms raw loan data into a structured decision making system that reveals hidden borrower patterns, portfolio vulnerabilities, and lending concentration risks.

---

## The Problem Nobody Talks About

Banks approve loans. They collect payments. But they rarely ask the right question: Are we lending to the right people?

Most lending dashboards show totals. Total funded, total repaid, total loss. But totals hide everything that matters.

A $500 million portfolio that's 95 percent concentrated in one region looks healthy until that region faces an economic downturn. A lending book with 60 percent of loans going to self employed borrowers looks profitable until employment becomes unstable. A portfolio with high average interest rates looks strong until you realize you're only getting those rates because you're lending to higher risk borrowers.

This project investigates what's actually hidden inside lending data.

---

## What This Dashboard Does Differently

Rather than displaying loan metrics in isolation, this project builds a connected intelligence system where each dashboard layer answers a specific business question.

The first dashboard functions as the operational command center. The second reveals borrower concentration patterns. The third sits in the backend, powering the entire analytical structure through relational logic and risk segmentation.

Most dashboards show what happened. This one helps you understand why it happened and what it means for the portfolio.

---

## Inside the Dashboard

### Layer 1: Portfolio Command Center

The first dashboard functions as the operational nerve center. Rather than overwhelming users with 50 metrics, it isolates the 8 KPIs that actually matter for portfolio health:

Funded amount (liquidity deployed), repayment rate (cash flow health), charge off rate (portfolio quality deterioration), interest rate (yield on risk), debt to income ratio (borrower stability), application volume (demand signal), MTD movement (month to date trends), and status segmentation (healthy vs at risk loans).

What makes this layer different: The dashboard separates charged off loans from healthy ones. Most dashboards treat all loans equally. This one asks where the portfolio is actually breaking down. By isolating charged offs as a distinct layer, you can see whether problem loans concentrate in specific borrower types, regions, or purposes.

---

### Layer 2: Pattern Recognition Through Segmentation

The second dashboard shifts from "how much" to "how distributed." This is where insights emerge.

Borrower stability signals matter because employment length predicts repayment behavior. Home ownership indicates skin in the game. Debt to income ratio shows financial breathing room.

Lending behavior patterns reveal concentration. Purpose distribution shows that some loan types have inherently higher default rates. Personal loans default more frequently than home improvement loans at the same size. Regional concentration means that geographic clustering of risk can spike quickly. Loan term trends show that shorter terms carry lower default risk but lower yield.

Why this matters: A portfolio that looks balanced overall might have 70 percent of its funded amount concentrated in three states. A lending book that shows strong repayment rates might hide the fact that 65 percent of loans are to employed borrowers, which means economic recession equals portfolio collapse.

---

### Layer 3: The Backend Intelligence System

Behind the dashboards sits the analytical engine that powers them. Rather than building dashboards in isolation, this workbook architecture separates data layer from calculation layer from insight layer.

The data layer contains raw loan records. The calculation layer builds pivot aggregations, KPI formulas, risk scoring. The insight layer interprets through dashboards.

This separation meant that adding a new metric doesn't break existing dashboards. Slicers in the dashboard automatically trigger recalculation across all dependent metrics. Portfolio comparisons built into the backend work seamlessly rather than through manual calculation.

---

## What the Data Revealed

### Finding 1: Concentration Risk Is Structural

Regional lending concentration determines portfolio resilience. A portfolio spread across 50 states is fundamentally more stable than one concentrated in 5 states, regardless of how profitable the concentrated region looks in good years.

### Finding 2: Employment Type Predicts Stability

Employed borrowers have measurably different repayment patterns than self employed borrowers. A portfolio that skews toward one group has built in structural risk that compounds during economic cycles.

### Finding 3: Purpose Matters More Than Loan Amount

A $50,000 personal loan defaults at a different rate than a $50,000 home improvement loan. Loan type drives risk intensity, not just the size of the capital deployed.

### Finding 4: The Interest Rate Paradox

Higher interest rates attract riskier borrowers. A portfolio with 15 percent average interest rates isn't healthier. It's riskier. You're compensating for risk exposure with higher yield, which is fine only if default rates stay constant. They rarely do.

---

## Why This Project Matters

For a lending business, this dashboard structure separates operational reporting from strategic intelligence. You can track activity daily while understanding structural portfolio risk on a quarterly basis.

For the analyst, building this taught me that dashboards aren't about pretty charts. They're about asking hard questions and organizing data so the answers become visible.

For portfolio managers, this is how you move from "we're profitable" to "we're profitable because we understand our risk."

---

## The Technical Reality

What made this interesting wasn't the Excel formulas. It was the architecture.

Most Excel projects are dashboards bolted onto flat data. This one was different because it contained relational logic between borrower attributes and lending outcomes. It used risk weighted aggregation so not all loans are equally important. It built temporal analysis to compare periods and identify trends. It implemented segmentation driven interpretation so the same $1 million portfolio looks different when viewed by region, purpose, and employment type.

The backend contains hundreds of formulas, but the user sees only clean dashboards because the complexity is hidden where it belongs in the calculation layer.

---

## The Bigger Picture

This project was an early exploration of how raw data becomes intelligence.

Raw data says: We funded $500 million in loans.

Interpreted data says: We funded $500 million in loans, 65 percent to employed borrowers in 5 states, with 8 percent charge offs concentrated in personal loan purposes.

One is a number. The other is a decision.