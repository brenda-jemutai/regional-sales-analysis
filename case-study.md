# Case Study: Regional Sales Performance Analysis

## Background

As part of building my data analyst skill set, I set out to complete an end-to-end project that mirrors real workplace tasks: taking a raw sales dataset and turning it into decision-ready insights using SQL, Excel, and Power BI.

## The Dataset

The dataset contains 150 sales records across four regions in Kenya — Nairobi, Nakuru, Mombasa, and Kisumu — with the following fields: Date, Region, Product, Salesperson, and Amount.

## The Business Questions

I approached this project the way a business stakeholder would frame it:

1. Which regions and salespeople are driving the most revenue?
2. How does performance break down by product?
3. How do sales trend over time?

## Step 1: SQL — Exploring and Ranking Performance

I used SQL to query the raw data and answer performance-ranking questions, including:
- Aggregating total sales by region and by salesperson
- Using window functions (RANK) to identify top performers
- Using CASE WHEN logic to categorize performance tiers
- Joining and filtering data to isolate specific segments

This gave me a first look at which regions and individuals were leading in revenue.

## Step 2: Excel — Cleaning and Exploratory Analysis

In Excel, I built out PivotTables and PivotCharts to explore the data interactively, using:
- XLOOKUP and INDEX/MATCH for cross-referencing values
- SUMIF/COUNTIF for conditional aggregation
- PivotTables to summarize sales by region, product, and salesperson

This step helped validate the SQL findings and surface any data quality issues before moving to visualization.

## Step 3: Power BI — Building an Interactive Dashboard

The final step was building a dashboard that stakeholders could explore themselves, without needing to write queries:

- **Data modeling:** Created a dedicated Date table using `CALENDAR()`, linked to the sales data, to support time-based calculations
- **DAX measures:** Built a Total Sales measure (`SUM`) and a Sales YTD (Year-to-Date) measure using `TOTALYTD`, enabling cumulative performance tracking
- **Visuals:** A clustered bar chart comparing Total Sales by Region, and a detailed table breaking down Region, Salesperson, Product, and Total Sales
- **Interactivity:** A Region slicer lets users filter the entire dashboard down to a single region with one click

## Key Findings

- **Nairobi** leads in total sales among the four regions, with **Nakuru** and **Mombasa** close behind — these three appear to be the strongest markets.
- **Kisumu** records the lowest total sales, pointing to an opportunity for targeted sales support, promotions, or further investigation into what's holding performance back there.
- The Sales YTD measure gives a running view of cumulative performance, useful for tracking progress against targets throughout the year.

## What This Project Demonstrates

- Ability to work across the full analytics stack — from raw data (SQL) to exploratory analysis (Excel) to a polished, interactive deliverable (Power BI)
- Practical DAX skills, including time intelligence functions
- Data modeling fundamentals (star-schema-style Date table)
- Translating a business question into a structured analysis and clear takeaways

## Files

- `sql/` — SQL queries used for the analysis
- `excel/` — Excel workbook with PivotTables and formulas
- `powerbi/` — Power BI dashboard file (`regional-sales-analysis.pbix`) and dashboard screenshots

---
**Brenda Jemutai** — Aspiring Data Analyst | Nairobi, Kenya
[brendajemutai28@gmail.com](mailto:brendajemutai28@gmail.com)
