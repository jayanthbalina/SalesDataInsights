# Sales Data Analysis Project

## Project Overview
In this project, I perform several key data engineering tasks to analyze sales data stored in Azure Blob Storage. Utilizing Databricks and Delta Lake, I derive meaningful insights to support stakeholders' decision-making processes.

## Key Achievements

### 1. Data Mounting
- **Objective**: Mount the Azure Blob Storage container to Databricks for easy access.
- **Method**: Used a specified `mount_point` to facilitate access to sales data in the cloud.

### 2. Data Ingestion
- **Objective**: Load sales data for processing.
- **Method**: Imported sales data from the CSV file `sales.csv` into a Spark DataFrame.

### 3. Data Cleaning
- **Tasks**:
  - Dropped missing values using `dropna()`.
  - Removed duplicates with `dropDuplicates()`.
  - Cast the `transaction_date` column to the correct date type.

### 4. Aggregating Sales by Region
- **Objective**: Analyze sales performance geographically.
- **Method**: Aggregated the sales data by region using Spark's `groupBy` and `sum` functions, producing a summary of total sales per region.

### 5. Writing Data to Delta Lake
- **Objective**: Store cleaned and aggregated data reliably.
- **Method**: Saved the aggregated sales data in Delta Lake format, leveraging its support for ACID transactions and versioning.

### 6. Data Analysis
- **Objective**: Identify top-performing regions.
- **Method**: Analyzed total sales by region, ordering results in descending order of sales.

### 7. Visualization
- **Objective**: Present sales data for stakeholder insights.
- **Method**: Visualized total sales by region to facilitate easy interpretation of performance metrics.

### 8. SQL Table Creation
- **Objective**: Enable SQL queries for data analysis.
- **Method**: Registered the aggregated sales data as a Delta table (`sales_by_region`) in Databricks.

### 9. Stakeholder Insights
- **Objective**: Provide actionable insights to stakeholders.
- **Method**: Executed SQL queries to identify regions with the highest sales, informing stakeholders about geographical sales distribution and performance.

## Conclusion
This project integrates data cleaning, aggregation, storage in Delta Lake, and SQL-based analysis, providing a robust solution for analyzing and reporting sales data trends. The methodologies employed ensure accurate and reliable insights that can significantly assist stakeholders in decision-making processes.

## Skills
- **Databricks** (Data engineering platform)
- **Delta Lake** (Storage layer for big data)
- **Apache Spark** (Data processing engine)
- **SQL** (Query language for data analysis)
- **Azure Blob Storage** (Cloud storage service)
