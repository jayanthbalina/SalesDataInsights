
In this Sales Data Analysis Project, I'm performing several key data engineering tasks to analyze sales data stored in Azure Blob Storage and derive meaningful insights using Databricks and Delta Lake. Here's a detailed description of what I'm achieving:

Data Mounting: I'm mounting the Azure Blob Storage container to Databricks using the specified mount_point, enabling easy access to the sales data stored in the cloud.

Data Ingestion: The sales data (from the CSV file sales.csv) is loaded into a Spark DataFrame for processing. This makes the data accessible for cleaning, transformation, and analysis.

Data Cleaning: I'm cleaning the data by:

Dropping missing values (dropna()).
Removing duplicates (dropDuplicates()).
Casting the transaction_date column to the correct date type.
Aggregating Sales by Region: I aggregate the sales data by region, calculating the total sales amount for each region using the groupBy and sum functions in Spark. The result is a summary of sales performance by geographical area.

Writing Data to Delta Lake: The cleaned and aggregated sales data is saved in Delta Lake format, providing a highly performant and reliable storage layer that supports ACID transactions and versioning.

Data Analysis: I perform analysis to identify the top-performing regions by total sales, ordering them in descending order of sales.

Visualization: I visualize the total sales by region to help stakeholders easily interpret the performance of each region.

SQL Table Creation: I register the aggregated sales data as a Delta table (sales_by_region) in Databricks, enabling me to query the data using SQL.

Stakeholder Insights: The SQL query I run allows me to provide answers about the regions with the highest sales, which is crucial for stakeholders who want to understand the geographical sales distribution and identify top-performing regions.

This project integrates data cleaning, aggregation, storage in Delta Lake, and SQL-based data analysis, providing a robust solution for analyzing and reporting sales data trends.
