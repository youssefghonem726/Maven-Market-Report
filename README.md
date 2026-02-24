# Maven Market Retail Sales & Performance Dashboard (Power BI)

---

## Project Overview

Maven Market is a fictional multi-national grocery retail chain operating across the United States, Canada, and Mexico.

This project delivers an end-to-end Business Intelligence solution built in Power BI to analyze transactional retail data and provide executive-level visibility into sales performance, profitability, return behavior, and regional contribution.

The objective was to transform raw CSV data into a structured analytical model and interactive dashboard to support data-driven decision-making.

---

## Business Objectives

The dashboard was designed to answer critical business questions:

- Which brands generate the highest transaction volume?
- How do current month transactions, profit, and returns compare to last month?
- Which countries and store locations drive the most sales?
- How is revenue trending over time?
- Is actual revenue exceeding performance targets?
- Which products present return risk?

---

## Data Sources & Data Modeling

The data model was built using 8 raw CSV files:

- Transactions (1997–1998)
- Returns
- Products
- Customers
- Stores
- Regions
- Calendar

A **Star Schema** was implemented with `Transaction_Data` as the central fact table, connected to dimension tables:

- Products
- Customers
- Stores
- Regions
- Calendar

The calendar table was enhanced with additional date intelligence fields:

- Start of Week
- Start of Month
- Month Name
- Quarter
- Year

This structure ensures scalability, optimized relationships, and clean analytical filtering.

---

## Data Preparation (Power Query)

Data transformation steps included:

- Merging historical transaction files
- Data type standardization
- Removing inconsistencies
- Creating calculated columns (e.g., Price Tier classification)
- Building full store address fields
- Enhancing calendar intelligence fields

Power Query was used to prepare the dataset for reliable analytical reporting.

---

## DAX & Performance Measures

Custom DAX measures were developed to support KPI tracking and executive reporting:

- Total Revenue
- Revenue Target
- Revenue Gap
- Total Transactions
- Total Profit
- Profit Margin
- Return Rate
- YTD Revenue
- 60-Day Revenue
- Month-over-Month comparisons

These measures enabled dynamic performance monitoring and target evaluation.

---

## Key Business Insights

- Overall revenue exceeded target by **$34.15K**, indicating strong aggregate performance.
- The United States generated the highest transaction volume across all regions.
- Plato delivers the highest profit margin but shows elevated return rates in Canada, posing potential profitability risk.
- Horatio records the highest return rate in the USA, suggesting possible product quality concerns.
- High Top experienced a sharp month-over-month increase in returns, signaling a recent operational shift.

These findings highlight both revenue opportunities and product risk factors requiring management attention.

---

## Tools & Technologies

- Power BI Desktop
- Power Query (ETL & Data Transformation)
- DAX (Advanced KPI Calculations)
- Star Schema Data Modeling
- CSV Data Integration

---

## Dashboard Screenshots

### Topline Performance Dashboard
![Dashboard Overview](Screenshots/dashboard_overview.png) 
### Key Performance Highlights
![Performance Insights](Screenshots/insights_page.png)
--- 
## Data Model
![Data Model](Screenshots/data_model.png) 
--- 
## Power Query Transformations
![Power Query](Screenshots/power_query.png)

---

## Conclusion

This project demonstrates the ability to design and implement a structured retail Business Intelligence solution using Power BI.

Through star schema modeling, custom DAX logic, and interactive dashboard design, the solution delivers:

- Clear KPI monitoring
- Regional performance comparison
- Brand-level profitability analysis
- Return behavior tracking
- Target vs actual evaluation

The dashboard translates transactional retail data into actionable business insights, reflecting practical, job-ready Business Intelligence capability.
