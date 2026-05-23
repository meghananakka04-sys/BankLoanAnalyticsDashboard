# Bank Loan Analytics Dashboard

Financial dashboards often focus on displaying numbers without explaining the operational story behind them.

While working on this project, I wanted to explore how lending data could be transformed into something more interpretable than static spreadsheet reporting. The dataset contained information about loan applications, borrower profiles, repayment behavior, funded amounts, employment categories, regional distribution, and loan quality indicators. Individually, these fields did not reveal much. The challenge was building a system that could connect them into a meaningful lending performance narrative.

The project was developed completely in Microsoft Excel using dashboarding, KPI reporting, pivot analysis, slicers, and portfolio segmentation techniques.

Instead of designing isolated charts, the focus was placed on building a structured reporting experience capable of answering practical questions around lending performance and portfolio health.

<br>

## Dashboard Architecture

The workbook was divided into multiple analytical layers.

| Section | Purpose |
|---|---|
| Summary Dashboard | High-level monitoring of lending KPIs and repayment performance |
| Overview Dashboard | Trend analysis across borrower categories and lending segments |
| Backend Design Sheet | KPI calculations, pivot logic, slicer connections, and chart structuring |

<br>

## Dashboard Preview

### Summary Dashboard

![Summary Dashboard](assets/Summary_dashboard.png)

The summary dashboard was designed as an executive-level reporting layer focused on portfolio health monitoring. Key lending indicators such as total applications, funded amounts, repayment collections, interest rates, and debt-to-income ratios were combined into a centralized KPI reporting system.

A major analytical focus was placed on separating good loans from bad loans in order to better understand repayment quality and lending risk exposure.

The dashboard also integrates MTD and MoM calculations to observe short-term portfolio movement and lending growth trends.

<br>

### Overview Dashboard

![Overview Dashboard](assets/Overview_dashboard.png)

The overview dashboard focuses more heavily on segmentation and lending distribution analysis.

Instead of looking only at aggregate numbers, this section explores:
- regional loan concentration,
- borrower employment stability,
- home ownership categories,
- loan purposes,
- loan terms,
- and monthly lending trends.

The intention was to create a dashboard that moves gradually from high-level portfolio monitoring into deeper borrower-level interpretation.

<br>

## Analytical Direction

One of the most interesting parts of the project was understanding how financial datasets become significantly more useful once they are segmented properly.

For example:
- repayment analysis becomes more meaningful when compared against loan status,
- lending performance changes across borrower categories,
- and regional concentration patterns reveal operational lending priorities.

The dashboard therefore evolved from a simple Excel reporting exercise into a broader portfolio analytics project centered around financial performance interpretation.

<br>

## Backend Design Process

Behind the dashboard visuals, the workbook includes:
- pivot table structuring,
- KPI aggregation logic,
- slicer-based filtering systems,
- percentage calculations,
- comparative monthly analysis,
- and portfolio segmentation workflows.

The backend sheet was intentionally separated from the presentation layer in order to keep the dashboard interface cleaner and easier to interpret.

![Backend Design](assets/Design_sheet.png)

<br>

## What This Project Helped Me Understand

This project became an important step in understanding how business intelligence dashboards are not only about visualization, but also about structuring information in a way that supports interpretation and decision-making.

Working through the dashboard helped strengthen my understanding of:
- financial KPI reporting,
- interactive dashboard design,
- portfolio segmentation,
- Excel-based business intelligence,
- and storytelling through analytical reporting.