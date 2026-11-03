# Healthcare-Data-Engineering-Project
End-to-end Healthcare Data Engineering ETL Pipeline using Azure Databricks, PySpark, SQL, and Delta Lake, following Medallion Architecture.
# Healthcare Data Engineering & Power BI Portfolio

## 1. Project Overview

This repository showcases my experience and technical skills in Healthcare Data Engineering and Business Intelligence.

It includes an independent end-to-end Healthcare ETL pipeline built using synthetic healthcare datasets, along with a summary of my professional experience in Power BI reporting, data loading, CI/CD deployments, Azure Databricks, and QA activities.

My objective is to build reliable data pipelines, transform data into meaningful insights, and develop interactive dashboards that support business decision-making.

## 2. Technical Skills

| Technology | Application |
|---|---|
| Azure Databricks | Data processing and job execution |
| PySpark | Data ingestion and transformation |
| SQL | Data extraction, transformation, and analysis |
| Delta Lake | Reliable data storage |
| Azure Data Factory | Data integration, where applicable |
| CI/CD Pipelines | Automated deployment and release processes |
| Power BI | Dashboard development and reporting |
| DAX | Measures and business calculations |
| Power Query | Data cleaning and transformation |
| QA Testing | Data validation and quality checks |
| GitHub | Code management and documentation |

## 3. Relevant Healthcare Project Experience

### Project 1: Healthcare Reporting and Analytics – CA D360

**Project Type:** Reporting and Business Intelligence

**Technologies:** Power BI, SQL, DAX, Power Query

**Responsibilities:**

- Worked on healthcare reporting and dashboard requirements.
- Developed and supported Power BI dashboards for business reporting.
- Worked on data preparation and transformation for reporting.
- Created visualizations to present meaningful business information.
- Supported reporting requirements and data analysis.

### Project 2: Healthcare Data Loading and Deployment – MCW

**Project Type:** Data Engineering and Deployment

**Technologies:** Azure Databricks, CI/CD Pipelines, PySpark, SQL, UAT, Production, QA

**Responsibilities:**

- Worked on healthcare data loading activities using CI/CD pipelines.
- Supported data deployment and loading processes across different environments.
- Executed CI/CD pipelines to support the deployment process.
- Triggered and monitored Azure Databricks jobs in UAT and Production environments.
- Performed QA activities to validate data loading and processing results.
- Supported data validation and troubleshooting during deployment activities.

### Project 3: CY2027 Healthcare Data Project

**Project Type:** Data Engineering and Deployment

**Technologies:** Azure Databricks, CI/CD Pipelines, PySpark, SQL, UAT, Production, QA

**Responsibilities:**

- Followed a similar data loading and deployment process used in the MCW project.
- Supported CI/CD pipeline execution.
- Triggered and monitored Databricks jobs in UAT and Production environments.
- Performed QA activities and validated data processing results.
- Supported data quality checks and troubleshooting throughout the process.

*Note: These project descriptions summarize professional responsibilities. No client-specific code, confidential business information, or actual patient data is included in this repository.*

## 4. Independent Portfolio Project: Healthcare Data Engineering ETL Pipeline

### Project Overview

This project demonstrates an end-to-end Healthcare Data Engineering ETL pipeline using Azure Databricks, PySpark, SQL, and Delta Lake.

The objective is to ingest, clean, transform, and analyze healthcare data to generate meaningful insights that support hospital operations and business decision-making.

This independent project uses synthetic healthcare datasets to demonstrate real-world data engineering concepts.

### Business Requirements

- Ingest patient, admission, and department data from CSV files.
- Identify and remove duplicate records.
- Handle missing and invalid data.
- Perform data validation and transformation.
- Store processed data using Delta Lake.
- Create analytical tables for reporting.
- Prepare curated datasets for Power BI dashboards.

## 5. Project Architecture

The project follows the Medallion Architecture.

### Bronze Layer – Raw Data

- Ingest raw healthcare CSV files.
- Preserve source data.
- Store raw records in Delta format.

### Silver Layer – Cleaned Data

- Remove duplicate records.
- Handle NULL values.
- Validate data types.
- Identify invalid dates.
- Perform data quality checks.
- Apply business transformation rules.

### Gold Layer – Business-Level Data

- Calculate total patient admissions.
- Analyze hospital department performance.
- Calculate hospital revenue.
- Analyze patient admission trends.
- Prepare aggregated datasets for Power BI reporting.

## 6. Technologies Used in the Portfolio Project

| Technology | Purpose |
|---|---|
| Azure Databricks | Data processing platform |
| PySpark | Data ingestion and transformation |
| SQL | Data analysis and querying |
| Delta Lake | Reliable data storage |
| ADLS Gen2 | Cloud storage, if configured |
| Power BI | Data visualization and reporting |
| GitHub | Project documentation and version control |

## 7. Dataset Description

This project uses three synthetic datasets.

### Patients Dataset

| Column | Description |
|---|---|
| patient_id | Unique patient identifier |
| patient_name | Synthetic patient name |
| age | Patient age |
| gender | Patient gender |
| city | Patient city |

### Admissions Dataset

| Column | Description |
|---|---|
| admission_id | Unique admission identifier |
| patient_id | Patient identifier |
| department_id | Hospital department identifier |
| admission_date | Patient admission date |
| discharge_date | Patient discharge date |
| bill_amount | Hospital billing amount |
| admission_type | Type of admission |

### Departments Dataset

| Column | Description |
|---|---|
| department_id | Department identifier |
| department_name | Hospital department name |

## 8. ETL Workflow

### Step 1: Data Ingestion

- Read CSV files using PySpark.
- Create Spark DataFrames.
- Inspect schemas and source records.
- Load raw data into the Bronze layer.

### Step 2: Data Cleaning

- Remove duplicate patient and admission records.
- Handle missing values.
- Validate patient and department identifiers.
- Convert date columns into appropriate date formats.
- Identify invalid records.

### Step 3: Data Transformation

- Join patient, admission, and department datasets.
- Calculate patient admission counts.
- Calculate hospital revenue.
- Calculate average length of hospital stay.
- Perform department-level aggregations.

### Step 4: Data Loading

- Store cleaned data in Silver Delta tables.
- Store aggregated data in Gold Delta tables.
- Prepare business-ready datasets for reporting.

## 9. Expected Business Insights

The Gold layer is designed to support the following analytics:

- Total number of patients.
- Total hospital admissions.
- Department-wise admission counts.
- Hospital revenue by department.
- Monthly admission trends.
- Average patient length of stay.
- Admission type distribution.

## 10. Power BI Dashboard

The curated Gold datasets can be connected to Power BI to develop an interactive healthcare dashboard.

Proposed dashboard components:

- Total Patients KPI.
- Total Admissions KPI.
- Total Hospital Revenue KPI.
- Monthly Patient Admission Trends.
- Department-wise Revenue Analysis.
- Admission Type Distribution.
- Average Length of Stay.

## 11. Repository Structure

```text
Healthcare-Data-Engineering-Project/
│
├── README.md
│
├── datasets/
│   ├── patients.csv
│   ├── admissions.csv
│   └── departments.csv
│
├── notebooks/
│   ├── 01_data_ingestion.py
│   ├── 02_data_cleaning.py
│   ├── 03_data_transformation.py
│   └── 04_data_analysis.py
│
├── sql/
│   └── healthcare_analysis.sql
│
├── powerbi/
│   └── healthcare_dashboard.pbix
│
├── screenshots/
│   └── dashboard_preview.png
│
└── architecture/
    └── etl_architecture.png
```

## 12. Project Outcomes

This portfolio demonstrates practical knowledge of:

- Building ETL pipelines using PySpark.
- Working with Azure Databricks.
- Implementing Bronze, Silver, and Gold layers.
- Performing data cleansing and validation.
- Using SQL for healthcare analytics.
- Working with Delta Lake.
- Executing and monitoring Databricks jobs.
- Understanding CI/CD deployment workflows.
- Working with UAT and Production environments.
- Performing QA and data validation.
- Developing Power BI dashboards and reports.

## 13. Data Privacy

All datasets included in the independent portfolio project are synthetic and created for educational and demonstration purposes.

No real patient records, Protected Health Information (PHI), confidential client information, proprietary source code, or internal project configurations are included.

## 14. Project Status

This repository is being developed incrementally.

The initial stage includes synthetic datasets and project documentation. PySpark notebooks, SQL scripts, Delta tables, and Power BI dashboard examples will be added as implementation progresses.

---

## About

**Domain:** Healthcare

**Role:** Data Engineer and Power BI Analyst

**Core Technologies:** Azure Databricks, PySpark, SQL, Delta Lake, Power BI, CI/CD

**Focus Areas:** Data Engineering, ETL Development, Data Loading, Data Quality, Deployment, Reporting, and Business Intelligence.
