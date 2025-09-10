# Netflix Data Engineering using Microsoft Azure and Databricks: End-to-End Data Engineering Project
## Introduction
This is a personal project to showcase an end-to-end Data Engineering project using Microsoft Azure, Databricks, and Delta Live Tables(DLT). This project demonstrates data ingestion using Azure Data Factory(ADF) and Databricks AutoLoader, processing the data through a Medallion Architecture(Bronze, Silver, Gold), and business reporting using PowerBI.
## Techstack
* SQL
* Python
* PySpark
* Azure Cloud Services
  * **Azure Data Factory** – Orchestration & ingestion  
  * **Azure Databricks** – Transformations & Delta Live Tables  
  * **ADLS Gen2** – Scalable data lake storage  
  * **Azure Synapse Analytics** – Data warehouse  
  * **Power BI** – Business reporting & insights   
## Overview
### 1. Data Ingestion (Extraction)
* Dataset sourced from Kaggle, contains 5 datasets in CSV and JSON formats.
* Created 4 containers for data storage in ADLS Gen 2 - Raw, Bronze, Silver, Gold.
* 4 files were ingested directly from Github using API method and stored in the Bronze container- Incremental data loading using Databricks Autoloader.
* 1 file was manually uploaded to ADLS Gen 2 in the Raw container.
### 2. Medallion Architecture (Transformation)
* **Bronze** – Raw incremental data  
* **Silver** – Cleaned and conformed data  
* **Gold** – Aggregated, business-ready data (Star Schema) 
### 3. Final Data for Analysis (Load)
* Data is structured into **Star Schema models (Gold Layer)** for analytics and reporting.
* Processed data is sent to **Azure Synapse Analytics** for warehousing.
* **Power BI** connects to Synapse for **real-time reporting and dashboards**.
 <img width="768" height="105" alt="Delta_Live_Tables_Architecture_v2" src="https://github.com/user-attachments/assets/5e0067f3-5a00-4290-bc6b-89328012a0d8" />

## Key Learnings
This project highlights the power of **Delta Live Tables** in simplifying ETL pipelines, enabling automated data quality checks, and providing reliable streaming + batch ingestion for modern analytics.
