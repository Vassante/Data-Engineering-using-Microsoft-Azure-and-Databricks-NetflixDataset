# Netflix Data Engineering using Microsoft Azure and Databricks: End-to-End Data Engineering Project
## Introduction
This is a personal project to showcase an end-to-end Data Engineering project using Microsoft Azure and Databricks. This project demonstrates data ingestion using Azure Data Factory(ADF) and Databricks AutoLoader, processing the data through a Medallion Architecture(Bronze, Silver, Gold), and business reporting using PowerBI.
## Techstack
* SQL
* Python
* PySpark
* Azure Cloud Services (key components)
  * Azure Data Factory (ADF)
  * Azure Data Lake Storage Gen 2 (ADLS Gen2)
  * Azure Databricks
  * PowerBI
## Overview
### 1. Data Ingestion (Extraction)
* Dataset sourced from Kaggle, contains 5 datasets in CSV and JSON formats.
* Created 4 containers for data storage in ADLS Gen 2 - Raw, Bronze, Silver, Gold.
* 4 files were ingested directly from Github using API method and stored in the Bronze container- Incremental data loading using Databricks Autoloader.
* 1 file was manually uploaded to ADLS Gen 2 in the Raw container.
### 2. Medallion Architecture (Transformation)
### 3. Final Data for Analysis (Load)
## Key Learnings
## Conclusion
