# E-commerce Data Analytics Pipeline (Python + pandas)

## Overview
This project demonstrates an end-to-end workflow to clean, validate, and enrich e-commerce data using Python (pandas).  
The output includes analysis-ready tables and a product performance summary (revenue, profit, and margin).

## Dataset
Tables used:
- `orders` (transactions)
- `customers` (customer attributes)
- `products` (product catalog and cost)

## Key Steps
- Data quality checks (missing values, inconsistent formats)
- Date parsing with safe coercion
- Standardization of categorical fields
- Fact/dimension merge (orders + product cost)
- Feature engineering: revenue, cost, profit, margin %

## Outputs
Exported to `/data`:
- `clean_orders.csv`
- `clean_customers.csv`
- `clean_products.csv`
- `product_performance.csv`

## Business Insights
- Profitability was evaluated using both total profit and average margin, not revenue alone.
- Strict data validation reduced record count but improved reliability of results.
- The aggregation pipeline is reusable as more data becomes available.

## How to run
Open the notebook:
- `notebooks/data_cleaning.ipynb`
Run cells top to bottom to reproduce exports.
