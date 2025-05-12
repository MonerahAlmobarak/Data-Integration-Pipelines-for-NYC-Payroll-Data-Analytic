# Data Integration Pipelines for NYC Payroll Data Analytics

This project delivers a scalable and automated data analytics solution for the City of New York using Microsoft Azure. The goal is to support budget transparency and operational efficiency through dynamic data pipelines and cloud-native analytics.

## 📌 Project Overview

The City of New York has two main objectives:

1. **Analyze financial resource allocation** — Understand how much of the City’s budget is spent on salaries and overtime.
2. **Enable public access to payroll data** — Share transparent payroll information with the public to promote accountability.

As a Data Engineer, your responsibility is to design and implement high-quality pipelines that process payroll data from raw files into structured formats ready for analysis in Azure Synapse Analytics.

## 🛠️ Technologies Used

- **Azure Data Factory** – For pipeline orchestration and data transformation using Data Flows.
- **Azure Data Lake Storage Gen2** – For storing raw and processed data files.
- **Azure SQL Database** – For staging data and creating structured views.
- **Azure Synapse Analytics** – For querying payroll insights via external tables.
- **Azure Monitor (optional)** – For pipeline tracking and alerting.

## 🗂️ Source Data

The source data consists of CSV files:

- **Employee Master Data** – Basic employee details.
- **Monthly Payroll Data** – Salary and overtime data submitted by NYC agencies.

These files are stored in Azure Data Lake Storage Gen2 and ingested into the data platform.

## 🏗️ Architecture & Pipeline Workflow

\[Azure Data Lake Gen2 - Raw Files]
↓
\[Azure Data Factory - Ingestion Pipelines]
↓
\[Azure SQL Database - Staging & Views]
↓
\[Azure Data Factory - Data Flows & Aggregations]
↓
\[Azure Data Lake Gen2 - Processed Output]
↓
\[Azure Synapse Analytics - External Tables]
↓
\[Analytics, Dashboards, & Public Access]

### Key Steps:
- Ingest raw CSVs using ADF pipelines.
- Create SQL views in Azure SQL DB for basic structuring.
- Transform and aggregate salary/overtime data using ADF Data Flows.
- Export processed data back to Data Lake in parquet format.
- Build Synapse external tables on top of processed data for analysis.

## 📊 Outcomes

- Identify salary trends and overtime costs by department or agency.
- Provide a centralized data platform for internal analysis and public use.
- Improve transparency on how payroll funds are allocated.

## 🔁 Future Enhancements

- Add support for incremental data loads.
- Implement alerting and retry mechanisms.
- Integrate public-facing dashboards with Power BI.

## 👤 Author

**Monerah Almobarak**  
Data Essentials and Data Engineering with MS Azure
Nanodegree Program
