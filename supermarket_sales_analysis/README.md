# Supermarket Sales Analysis

## Project Overview
This project analyzes supermarket transaction data using Python to identify peak recorded transaction periods, revenue drivers, and product performance.  
The analysis focuses on understanding when recorded transaction activity is relatively higher in the dataset and whether revenue peaks are driven by customer volume (transaction count) or spending per transaction (ATV).

## Dataset
Public supermarket sales dataset (CSV format, ~1000 transactions).  
The dataset was obtained from publicly available sources and used for educational and portfolio purposes.  
This is a sample transaction dataset for analytical practice, not a full production POS dataset.

## Tools and Libraries
- Python
- pandas
- matplotlib
- seaborn
- Jupyter Notebook

## Analysis Steps

### 1. Weekday vs Weekend Recorded Transactions
Calculated average recorded transaction counts per day by branch to avoid bias from unequal numbers of weekdays and weekends.

### 2. Peak Time Identification
Created a heatmap of transaction counts by day and hour to identify the busiest time slots.

### 3. Revenue Decomposition
Analyzed whether peak revenue periods were driven primarily by:
- Higher customer volume (traffic), or  
- Higher average transaction value (ATV)

Compared peak values with overall averages to quantify the impact.

### 4. Product Performance During Peak Hour
Identified which product lines contributed most to revenue during peak traffic periods.

## Key Findings
- The busiest period occurs on Saturday afternoon.
- Revenue peaks are primarily driven by higher customer volume rather than significantly higher spending per customer.
- Certain product categories contribute disproportionately to peak-hour revenue.

## Example Outputs

### Weekday vs Weekend Recorded Transactions

![Weekday vs Weekend Recorded Transactions](images/weekday_weekend_recorded_transactions.png)

### Recorded Transactions Heatmap

![Recorded Transactions Heatmap](images/recorded_transactions_heatmap.png)

### Transaction Count and Average Transaction Value by Day and Hour

![Transaction Count and Average Transaction Value by Day and Hour](images/transaction_count_and_avg_value_by_day_hour.png)

### Top Product Lines at Peak Hour

![Top Product Lines at Peak Hour](images/top_product_lines_peak_hour.png)

## Business Implications
- Increase staffing during peak traffic periods.
- Optimize product placement for high-performing categories during peak hours.
- Consider targeted promotions during off-peak hours to balance demand.

## Project Structure
supermarket_sales_analysis/

├── data/  
│    supermarket_sales.csv  

├── images/  
│    weekday_weekend_recorded_transactions.png  
│    recorded_transactions_heatmap.png 
     transaction_count_and_avg_value_by_day_hour.png
│    top_product_lines_peak_hour.png  

├── supermarket_sales_analysis.ipynb  

└── README.md

## Author
Hannah Yu
