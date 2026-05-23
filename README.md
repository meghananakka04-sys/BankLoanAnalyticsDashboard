# Bank Loan Analytics Dashboard

Most banking dashboards summarize lending activity through static reports and isolated metrics. While working on this project, I wanted to explore how a raw financial dataset could be converted into something more interactive and interpretable from a portfolio analysis perspective.

The dataset included borrower information, funded amounts, repayment behavior, regional lending distribution, employment categories, loan purposes, and loan status classifications. Looking at these variables individually did not reveal much. The real challenge was organizing them into a system capable of showing lending trends, repayment quality, and portfolio performance in a more connected way.

The entire project was built inside Microsoft Excel using pivot-based reporting, dashboard design techniques, slicers, KPI calculations, and interactive filtering systems.

<br>

## Dashboard Structure

| Layer | Analytical Focus |
|---|---|
| Summary Dashboard | Portfolio-level KPI monitoring |
| Overview Dashboard | Borrower segmentation and lending distribution |
| Backend Design Sheet | Calculation logic and dashboard architecture |

<br>

## Summary Dashboard

![Summary Dashboard](assets/Summary_dashboard.png)

This dashboard acts as the main reporting layer of the project.

Instead of focusing on only aggregate values, the dashboard was designed to monitor the relationship between funded amounts, repayment collections, portfolio quality, borrower health indicators, and lending performance trends simultaneously.

One of the most important analytical sections was the separation between good loans and bad loans. This introduced a more risk-oriented perspective into the reporting structure rather than treating all lending activity equally.

The integration of MTD and MoM calculations also helped create a short-term trend monitoring system capable of tracking recent portfolio movement.

<br>

## Overview Dashboard

![Overview Dashboard](assets/Overview_dashboard.png)

The second dashboard focuses more heavily on segmentation analysis.

Rather than looking at lending activity only from a financial perspective, this section explores how borrower categories influence loan distribution patterns across:
employment length,
home ownership,
loan purpose,
regional concentration,
and loan term structures.

This gradually shifts the analysis from simple reporting into borrower-level interpretation.

<br>

## Behind the Dashboard

![Backend Design](assets/Design_sheet.png)

The backend layer contains the underlying dashboard architecture including:
pivot structures,
KPI aggregation workflows,
slicer connections,
comparative calculations,
and portfolio segmentation logic.

Separating the backend logic from the dashboard presentation layer made the reporting structure easier to maintain and visually cleaner to navigate.

<br>

## Reflection

This project became an important step in understanding that dashboards are not simply collections of charts.

The more interesting challenge was learning how to organize information in a way that supports interpretation, comparison, and decision-making.

Working through this project helped strengthen my understanding of:
financial KPI reporting,
interactive dashboard design,
portfolio segmentation,
and analytical storytelling using Excel.