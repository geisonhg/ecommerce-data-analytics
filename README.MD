# E-commerce Data Analytics Pipeline (Python & pandas)

## Overview
This project demonstrates an end-to-end data analytics workflow for e-commerce data using Python (pandas).
The goal is to clean, validate, and enrich transactional data to produce analysis-ready datasets and support business decision-making.

The pipeline focuses on data quality, feature engineering, and profitability analysis rather than revenue alone.

---

## Dataset
The project works with structured e-commerce data split into the following tables:

- orders: transactional sales data
- customers: customer attributes and identifiers
- products: product catalog including cost information

---

## Key Steps
- Data quality checks (missing values, invalid records, inconsistent formats)
- Safe date parsing and type validation
- Standardization of categorical fields
- Fact and dimension merging (orders + product cost)
- Feature engineering:
  - revenue
  - cost
  - profit
  - margin percentage
- Exploratory aggregation to evaluate product performance

---

## Outputs
The pipeline exports cleaned and analysis-ready datasets to the `/data` directory:

- clean_orders.csv
- clean_customers.csv
- clean_products.csv
- product_performance.csv

---

## Business Insights
- Product performance is evaluated using total profit and average margin, not revenue alone.
- Strict validation rules reduce record count but significantly improve data reliability.
- The aggregation logic is reusable and scalable as additional data becomes available.

---

## Project Status
Work in progress.

Initial data cleaning, validation, and feature engineering are complete.  
Next steps include deeper exploratory data analysis (EDA), customer-level insights, and dashboard visualisation.

---

## Tools & Technologies
- Python
- pandas
- Jupyter Notebook
- CSV-based data pipeline

---

## How to Run
1. Open the notebook:
   notebooks/data_cleaning.ipynb
2. Run all cells top to bottom to reproduce the cleaned datasets and exports.

