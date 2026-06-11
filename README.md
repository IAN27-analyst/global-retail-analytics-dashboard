# Enterprise Cross-Border Retail Analytics Dashboard

## Project Overview
This project demonstrates an enterprise business intelligence workflow, transforming a raw, uncleaned cross-border retail dataset into an automated, high-fidelity executive dashboard. The pipeline architecture handles data ingestion, multi-stage cleaning, semantic data modeling, and interactive visualization across both Microsoft Excel and Power BI Desktop.

## Business Insights & Objectives
* **Geographic Market Analysis**: Identifying high-performing regions and distribution channels (with major market penetration highlighted in West Africa and North America).
* **Product Vertical Contribution**: Evaluating category performance to isolate revenue dominance (e.g., Electronics vs. Furniture & Office Supplies).
* **Operational Performance**: Tracking logistics metrics based on fulfillment and shipping statuses (*Delivered, Pending, Shipped, Cancelled*).

## Technical Architecture & Tools Used
* **Data Pipeline & ETL**: Power Query (Excel & Power BI) for structural transformation, schema validation, and missing value imputation.
* **Semantic Modeling**: DAX (Data Analysis Expressions) for explicit enterprise business metrics.
* **Visualization Matrix**: Power BI Desktop (High-fidelity, cross-filtered canvas leveraging dynamic tile-based slicer decks and executive KPI indicators).

## Core Data Metrics Engineered (DAX Formulas)
```DAX
Total Net Revenue = SUM('Clean Data'[Net Revenue])

Total Units Sold = SUM('Clean Data'[Quantity])

Total Transactions = COUNTROWS('Clean Data')
