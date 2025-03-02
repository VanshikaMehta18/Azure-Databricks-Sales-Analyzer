# Azure-Databricks-Sales-Analyzer
This project is a sales analytics pipeline built on Databricks (Azure) using PySpark. It processes and analyzes large-scale sales data, cleans inconsistencies, and generates insights such as total sales per store, sales per square foot, and yearly trends.

# Objective
Data Cleaning: Handle missing values, remove duplicates, and standardize date formats.
Data Transformation: Join sales and store data, create new metrics, and extract meaningful information.
Data Analysis: Identify top-performing stores and best-selling products.
Data Storage: Save results in Parquet format for efficient querying.

## Dataset Information
The project uses two datasets:
sales_data.csv – Contains transactional sales data (sale_id, store_id, product_id, quantity, total_amount, sale_date).
store_data.csv – Contains store details (store_id, store_region, store_size, open_date).

# Compute:
Total Sales per Store
Total Quantity Sold per Store
Group results by store_id and store_region


# Technologies Used
Apache Spark (PySpark) – Scalable data processing
Databricks (Azure) – Cloud-based big data analytics
SQL for Data Aggregation – Querying structured data

