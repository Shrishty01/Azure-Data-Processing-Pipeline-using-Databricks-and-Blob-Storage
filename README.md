# Azure Data Processing Pipeline using Databricks and Blob Storage

## Overview
This project demonstrates how to upload, clean, and process CSV files using Azure services like Blob Storage, Databricks, and SQL Database.

## Steps Performed

### 1. Azure Setup
- Created a Storage Account for storing CSV files.
- Set up a Databricks Workspace for data processing.
- Configured Azure SQL Database for storing cleaned data.

### 2. Uploading Data
- Uploaded multiple CSV files to the Blob Storage container.
- Verified file formats and contents before processing.

### 3. Data Cleaning in Databricks
- Connected to Blob Storage using wasbs protocol.
- Loaded CSV files into Spark DataFrame.
- Cleaned data by:
  - Removing unwanted characters (like "$").
  - Casting columns to proper data types.
  - Formatting dates to yyyy-mm-dd.
  - Dropping rows with nulls, invalid data, or duplicates.

### 4. Writing Cleaned Data
- Saved the cleaned data back to storage or to Azure SQL Database.

### 5. Resource Management
- Set Auto-Termination for clusters.
- Deleted unused services to avoid unnecessary charges.
- Reviewed billing information to monitor resource usage.

## Technologies Used
- Azure Storage Account
- Azure Databricks
- PySpark
- Azure SQL Database

## Notes
- This pipeline is cost-efficient and scalable.
- Authentication using account keys or SAS tokens is required.
