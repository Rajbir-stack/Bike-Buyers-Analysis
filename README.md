# Bike Buyers Analysis Dashboard (Excel)

An Excel-based analysis of customer demographics and bike-purchasing behaviour. The workbook uses cleaned customer data, PivotTables, PivotCharts, and a dashboard to explore patterns across age groups, income, gender, commute distance, and region.

## Workbook contents

- **bike_buyers** – original customer dataset.
- **Working Sheet** – cleaned working copy with standardized categorical values and an `Age_Bracket` field.
- **Pivot Table** – summary analyses built with PivotTables and charts.
- **Dashboard** – visual summary of the analysis.

## Questions explored

1. How does bike purchasing vary by age bracket?
2. How does average income differ between customers who purchased a bike and those who did not?
3. How does commute distance relate to bike-purchase patterns?
4. How do purchase counts compare across customer groups?

## Selected findings

Based on the workbook's PivotTables:

- 481 of 1,000 customers purchased a bike (48.1%); 519 did not (51.9%).
- The **Middle Age** bracket had 372 purchases out of 685 customers (about 54.3%).
- The **Adolescent** bracket had 39 purchases out of 110 customers (about 35.5%).
- The **Old** bracket had 70 purchases out of 205 customers (about 34.1%).
- Customers with a commute distance of **2–5 miles** had 95 purchases out of 162 customers (about 58.6%).
- Customers with a commute distance of **more than 10 miles** had 33 purchases out of 111 customers (about 29.7%).
- Average income was 55,760 among customers who purchased a bike, compared with about 51,084.91 among customers who did not.

These are descriptive patterns in this dataset; they do not establish that any one factor causes a customer to purchase a bike.

## Excel skills used

- Data cleaning and standardizing categorical values
- Nested `IF` logic to create age brackets
- PivotTables and PivotCharts
- Comparing counts and averages across customer segments
- Dashboard layout and interactive filtering where slicers are connected

## Files

- `Bike_Buyers_Analysis.xlsx` – Excel workbook containing the data, working sheet, PivotTables, charts, and dashboard.
- `README.md` – project overview and selected findings.
- `Screenshots/` – add a PNG screenshot of the finished Dashboard here so the dashboard can be previewed directly in the repository.

## How to view

Download `Bike_Buyers_Analysis.xlsx` and open it in Microsoft Excel. For the best experience, use Excel desktop so PivotTables, PivotCharts, and slicers can be explored interactively. Refresh PivotTables if Excel prompts you to update the workbook's data.

## Credit

This project is inspired by the Bike Buyers Excel tutorial by [Alex The Analyst](https://github.com/AlexTheAnalyst). The dataset/tutorial inspiration is credited to the original creator; this repository contains my own workbook practice and analysis.
