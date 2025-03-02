# Azure-Databricks-Sales-Analyzer
This project is a sales analytics pipeline built on Databricks (Azure) using PySpark. It processes and analyzes large-scale sales data, cleans inconsistencies, and generates insights such as total sales per store, sales per square foot, and yearly trends.

## Dataset Information
The project uses two datasets:
sales_data.csv – Contains transactional sales data (sale_id, store_id, quantity, total_amount, sale_date).
store_data.csv – Contains store details (store_id, store_region, store_size).

# Key Features & Workflow
1. Data Loading
Read the sales and store datasets from Databricks FileStore into PySpark DataFrames.
2. Data Cleaning & Preprocessing
Handle Missing Values: Replace nulls in quantity and total_amount with 0.
Remove Duplicates: Ensures unique transactions.
Filter Out Invalid Data:
Drop records where sale_id, store_id, or sale_date is missing.
Remove negative or zero values in quantity and total_amount.
3. Data Transformation & Feature Engineering
Join Sales & Store Data using an inner join on store_id.
Extract Year from sale_date to analyze sales trends over time.
Compute Sales per Square Foot (total_amount / store_size) to measure store efficiency.
4. Aggregation Using Spark SQL
Create a temporary SQL table to run queries on the combined dataset.

# Compute:
Total Sales per Store
Total Quantity Sold per Store
Group results by store_id and store_region


# Technologies Used
Apache Spark (PySpark) – Scalable data processing
Databricks (Azure) – Cloud-based big data analytics
SQL for Data Aggregation – Querying structured data

