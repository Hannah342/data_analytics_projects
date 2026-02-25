# Supermarket Sales Data Cleaning and Validation

## Project Overview
This project demonstrates a structured data cleaning workflow for transactional retail data.  
The goal is to ensure data quality and reliability before performing business analysis.

The project focuses on validating numeric fields, handling missing values, and ensuring categorical and datetime consistency.

## Dataset
Supermarket sales dataset containing transactional records such as:

- Invoice ID
- Product line
- Unit price
- Quantity
- Total
- Rating
- Date and Time
- Payment method

## Tools
- Python
- pandas
- Jupyter Notebook

## Data Cleaning Workflow

### 1. Data Inspection
Checked dataset shape, column types, and initial structure.

### 2. Field Classification
Grouped columns into:
- Identifier fields
- Numeric fields
- Categorical fields
- Datetime fields

This helps define appropriate validation rules.

### 3. Numeric Type Enforcement
Converted numeric fields using:
pd.to_numeric(errors="coerce")


This exposes invalid entries as NaN.

### 4. Business Rule Validation
Validated logical constraints:

- Unit price > 0
- Quantity > 0
- Total > 0
- Rating between 0 and 10

No violations were found.

### 5. Missing Value Strategy
Rows with missing values in core numeric fields were removed to ensure analysis reliability.

Approximately 14–15% of rows were removed.

### 6. Categorical Consistency Check
Checked category values and corrected formatting issues such as leading/trailing spaces.

### 7. Datetime Parsing Validation
Confirmed that Date and Time fields could be successfully parsed.

### 8. Final Sanity Check
Verified:

- No remaining missing values in core fields
- Dataset ready for analysis

## Result
Produced a clean, analysis-ready dataset suitable for downstream analytics.

## Project Structure
supermarket_sales_data_cleaning/
│
├── data/
│ └── supermarket_sales_dirty.csv
│
├── supermarket_sales_data_cleaning.ipynb
│
└── README.md

## Author
Hannah Yu