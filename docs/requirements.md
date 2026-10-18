# Requirements: Sales Controlling Dashboard

## Business context

The sales controlling team of Adventure Works, a fictional bicycle manufacturer selling through an online store and a reseller network, needs a monthly view of actual sales against budget. The report should show deviations by region early, explain them to management, and point to where margin is lost.

## Stakeholders

| Role | Need |
| --- | --- |
| Head of Sales | Is each region on plan this fiscal year? |
| Sales Controller | Which regions and months drive the variance? Is the year on track? |
| Product and Channel Managers | Which categories and channels earn margin, and which lose it? |

## Business questions

1. Are we ahead of or behind budget, in total and by region?
2. Is the year to date result on track to reach the annual plan?
3. How do sales and margin develop compared with the prior year?
4. Which product categories and sales channels contribute most to sales and to margin?

## KPI definitions

| KPI | Definition | Source |
| --- | --- | --- |
| Sales | Sum of sales amount of all order lines | Sales |
| Budget | Sum of planned sales by region and month | Budget |
| Variance | Sales minus budget, compared only in months that have a budget | Sales, Budget |
| Variance to Budget % | Variance divided by budget | Sales, Budget |
| Regions Ahead / Behind Plan | Number of regions with a variance of at least zero / below zero | Sales, Budget |
| Gross Margin % | (Sales minus product cost) divided by sales | Sales |
| Internet / Reseller Margin % | Gross margin % for one sales channel only | Sales, Sales Order |
| Sales YTD / Budget YTD | Cumulative value from 1 July to the selected period | Sales, Budget |
| Change vs. Prior Year | Change in sales against the same period of the prior year | Sales |

## Functional requirements

* Filter all pages by fiscal year; the selection is kept when switching pages.
* Filter the product page by sales channel (Internet, Reseller).
* Highlight regions ahead of plan and behind plan with consistent colors.
* Show the cumulative year to date trend of sales against budget.

## Data and assumptions

* Actual sales: Microsoft AdventureWorks sample, fiscal years 2018 to 2020.
* The fiscal year runs from July to June; amounts are in US dollars.
* A budget exists for fiscal years 2019 and 2020 at region and month level. Fiscal year 2018 has no budget, so variance measures are blank for it.
* The budget was created for this project from prior year actuals, since the sample contains no plan data.

## Out of scope

* Budget at product or channel level
* Forecasting and scenario planning
* Customer level analysis
