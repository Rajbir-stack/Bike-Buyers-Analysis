# Bike Buyers Analysis Dashboard | Microsoft Excel

An Excel-based data analysis project exploring customer demographics and bike-purchasing behaviour. The workbook was created as a hands-on recreation and extension of the Bike Buyers Excel tutorial by **Alex The Analyst**.

The analysis examines how bike purchases vary across age groups, gender, income, and commute distance. The workbook uses a cleaned working sheet, formula-based age segmentation, PivotTables, PivotCharts, and an interactive dashboard with slicers.

## Project objective

Explore the customer data to answer questions such as:

- Which age group has the highest number of bike purchases?
- How does average income differ between customers who purchased a bike and those who did not?
- How do purchase patterns vary by commute distance?
- How do customer groups compare by gender and other demographic attributes?

## Workbook structure

| Sheet | Purpose |
|---|---|
| `bike_buyers` | Original source data imported for the project. |
| `working sheet` | Cleaned analysis-ready data, including standardized category labels and the derived `Age_Bracket` column. |
| `PIVOT TABLE` | PivotTable summaries and supporting PivotCharts used to compare customer segments. |
| `DASHBOARD` | Visual summary of the analysis with charts and slicer-based filtering. |

## Data preparation

The original sheet contains 1,026 data rows. The working sheet retains **1,000 unique customer records** after duplicate records were removed.

The preparation steps include:

- Removing duplicate records.
- Standardizing marital-status labels and gender capitalization.
- Creating an `Age_Bracket` field from the `Age` column.
- Preparing the cleaned data for PivotTable analysis.

### Age-bracket logic

The workbook groups ages using the following rules:

| Age | Age bracket |
|---:|---|
| Below 31 | Adolescent |
| 31–53 | Middle Age |
| 54 and above | Old |

The calculated column uses a nested `IF` formula similar to:

```excel
=IF(L2>=54,"Old",IF(L2>=31,"Middle Age",IF(L2<31,"Adolescent","Invalid")))
```

*Note: These labels follow the tutorial's grouping. “Adolescent” is the workbook's label for customers below 31, not a formal demographic definition.*

## Selected findings

The following figures are calculated from the 1,000-record cleaned working sheet:

- **481 customers (48.1%)** purchased a bike; **519 (51.9%)** did not.
- The **Middle Age** group contains 685 customers and accounts for 372 bike purchases (about 54.3% of that group).
- The **Adolescent** group contains 110 customers and accounts for 39 bike purchases (about 35.5%).
- The **Old** group contains 205 customers and accounts for 70 bike purchases (about 34.1%).
- Customers commuting **2–5 miles** have 95 purchases out of 162 customers (about 58.6%).
- Customers commuting **more than 10 miles** have 33 purchases out of 111 customers (about 29.7%).
- Average income is approximately **$57,963** for customers who purchased a bike and **$54,875** for customers who did not.

These are descriptive patterns in this dataset. They do not prove that age, income, or commute distance causes a customer to purchase a bike.

## Excel skills demonstrated

- Data cleaning and duplicate removal
- Standardizing categorical values
- Nested `IF` formulas and calculated columns
- PivotTables and PivotCharts
- Comparing counts, averages, and customer segments
- Dashboard design and slicer-based filtering

## How to use the workbook

1. Download `bike_buyers_dashboard.xlsx` from this repository.
2. Open it in Microsoft Excel desktop.
3. Use the slicers on the dashboard to filter the analysis by available customer categories.
4. Clear slicer filters to return to the full-dataset view. PivotTable totals can change when slicer selections are active.

## Credit

This project is inspired by the Bike Buyers Excel tutorial by [Alex The Analyst](https://github.com/AlexTheAnalyst) and the associated [YouTube tutorial](https://youtu.be/opJgMj1IUrc). The tutorial creator is credited for the learning resource and project inspiration. The workbook in this repository is my own practice/recreation and analysis based on that tutorial; it is not presented as Alex The Analyst's original completed workbook.
