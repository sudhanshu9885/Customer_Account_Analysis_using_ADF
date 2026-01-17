# Customer_Account_Analysis_using_ADF

**Customer Account Data Pipeline  
**Scalable Azure Data Lake Pipeline for Reliable Customer Account Analytics**  

**Build a robust ETL pipeline to deliver accurate, up-to-date customer account data for analytics and reporting.**

---

## Tools & Technologies
- **Data Platform:** Azure Data Factory (ADF), Azure Data Lake Storage (ADLS), Azure SQL Database  
- **Data Formats:** Delta, Parquet  
- **Security & Governance:** Azure Key Vault  
- **Architecture & Documentation:** Draw.io  

---

## Key Features

- **Data Ingestion (Bronze Layer):**  
  Designed and executed ADF pipelines to ingest raw customer account data from backend Azure Storage into the Bronze layer of ADLS. Multiple source files including accounts, customers, loans, transactions, and loan payments were efficiently copied using ADF Copy Activities.

- **Data Cleaning & Transformation (Silver Layer):**  
  Applied data quality checks and transformations using ADF Mapping Data Flows. Performed deduplication, null validation on primary keys, and schema standardization before storing curated datasets in Delta format for reliable downstream processing.

- **ETL Processing & Data Modeling (Gold Layer):**  
  Built end-to-end ETL workflows to prepare analytics-ready datasets by reading Silver-layer Delta files and loading them into Azure SQL Database. Implemented Slowly Changing Dimension Type-1 (SCD-1) logic to upsert records, ensuring existing records were updated and new records inserted accurately.

- **Data Pipeline Architecture:**  
  Architected a scalable Bronze–Silver–Gold data pipeline following modern data lake best practices. Designed and documented the solution using Draw.io for maintainability, integrity, and seamless data flow.

- **Security & Governance:**  
  Secured sensitive credentials, storage keys, and SQL connection strings using Azure Key Vault. Integrated Key Vault with ADF pipelines to dynamically retrieve secrets, eliminating hardcoded credentials and enhancing compliance.

---

## Business Impact
Delivered a robust and production-ready data pipeline that ensures accurate, up-to-date customer account data for downstream analytics and reporting. Validated upsert functionality by simulating real-world data changes, enabling trusted data consumption for business decisions.

