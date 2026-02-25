# Supermarket Sales SQL Analysis (DuckDB)

## Project Overview
This project analyzes supermarket sales data using SQL executed through DuckDB in Python.

The goal is to demonstrate SQL skills for business analysis, including aggregation, time-based analysis, and identifying revenue drivers.

DuckDB allows SQL queries to run directly on pandas DataFrames.

## Dataset
Supermarket transaction dataset (CSV format).

Loaded into pandas and registered as a DuckDB table.

## Tools
- Python
- DuckDB
- SQL
- pandas
- Jupyter Notebook

## Analysis Tasks

### 1. Weekday vs Weekend Traffic
Calculated average daily transaction counts per branch.

Used CTE structure:

- base layer
- feature layer
- aggregation layer

### 2. Peak Time Slot Identification
Identified busiest day-hour combinations using:
COUNT(DISTINCT Invoice ID)

Measured:

- traffic
- revenue
- ATV

### 3. Peak vs Baseline Comparison
Compared peak slot values to overall averages.

Calculated:

- traffic ratio
- ATV ratio

This helps determine whether peaks are traffic-driven or spending-driven.

### 4. Ranking Analysis
Used window functions such as:
ROW_NUMBER()

to identify top traffic and top ATV periods.

## Key Findings
- Saturday afternoon shows the highest traffic.
- Traffic increases more significantly than ATV during peak periods.
- Revenue peaks are mainly driven by customer volume.

## SQL Concepts Demonstrated
- CTE (WITH clause)
- Aggregation (COUNT, AVG, SUM)
- Date/time parsing
- Window functions
- Ranking
- Business metric calculation

## Project Structure
supermarket_sales_sql_analysis/
│
├── data/
│ └── supermarket_sales.csv
│
├── supermarket_sales_sql_analysis.ipynb
│
└── README.md

## Author
Hannah Yu
