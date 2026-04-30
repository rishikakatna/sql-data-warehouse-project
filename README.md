# 🏗️ SQL Data Warehouse & Analytics Project

A end-to-end data warehousing and analytics solution built using SQL Server, implementing a medallion architecture (Bronze → Silver → Gold) to transform raw ERP and CRM data into structured, analytics-ready models.

---

## 📌 Project Overview

This project simulates a real-world data engineering workflow — ingesting raw data from multiple source systems, cleaning and transforming it through layered pipelines, and delivering business-ready analytical reports through a star schema data model.

**Business Problem:** Raw operational data from ERP and CRM systems was siloed, inconsistent, and not ready for reporting. This warehouse consolidates, cleans, and structures that data to enable reliable business analytics.

---

## 🏛️ Data Architecture

The warehouse follows the **Medallion Architecture** with three layers:

| Layer | Purpose |
|-------|---------|
| 🥉 **Bronze** | Raw data ingested as-is from ERP and CRM source systems |
| 🥈 **Silver** | Cleaned, standardized, and validated data |
| 🥇 **Gold** | Business-ready fact and dimension tables (Star Schema) |

---

## 🛠️ Tech Stack

- **Database:** SQL Server
- **ETL:** SQL-based stored procedures and scripts
- **Data Modeling:** Star Schema (Fact & Dimension tables)
- **Documentation:** Draw.io (architecture, data flow, ERD diagrams)
- **Version Control:** Git & GitHub

---

## 📂 Project Structure

```
sql-data-warehouse-project/
│
├── datasets/                  # Raw source data (ERP and CRM)
│   ├── source_crm/            # CRM system raw files
│   └── source_erp/            # ERP system raw files
│
├── docs/                      # Architecture and documentation
│   ├── data_architecture.drawio
│   ├── data_catalog.md
│   ├── data_flow.drawio
│   ├── data_models.drawio
│   ├── etl.drawio
│   └── naming-conventions.md
│
├── scripts/                   # SQL ETL scripts by layer
│   ├── bronze/                # Raw data load scripts
│   ├── silver/                # Cleaning and transformation scripts
│   └── gold/                  # Analytical model scripts
│
├── tests/                     # Data quality and validation scripts
├── README.md
└── .gitignore
```

---

## ⚙️ ETL Pipeline

**Bronze Layer — Extract & Load**
- Ingests raw CSV data from ERP and CRM source systems into SQL Server staging tables
- No transformations applied — preserves raw data as-is for auditability

**Silver Layer — Clean & Transform**
- Handles null values, duplicates, and inconsistent formats
- Standardizes data types, column naming, and business rules
- Applies data quality checks before promoting to Gold

**Gold Layer — Model & Deliver**
- Builds fact and dimension tables using Star Schema design
- Optimized for analytical queries and BI reporting
- Supports customer segmentation, product performance, and sales trend analysis

---

## 📊 Analytics & Reporting

SQL-based reports built on the Gold layer cover:

- 📈 **Revenue Trends** — Monthly and yearly sales performance
- 👥 **Customer Segmentation** — Behavior and purchase pattern analysis
- 📦 **Product Performance** — Top and bottom performing products
- 🌍 **Regional Analysis** — Sales breakdown by location

---

## 🔑 Key Outcomes

- Transformed raw, siloed ERP and CRM data into a unified analytics-ready warehouse
- Reduced reporting query time through optimized star schema modeling
- Implemented automated data quality checks across all pipeline layers
- Delivered structured SQL reports enabling data-driven business decisions

---

## 👩‍💻 About Me

I'm Rishika Katna, a Business Data Analyst with 2+ years of experience in SQL, Python, Power BI, and cloud analytics. This project reflects my interest in data engineering and warehouse design as an extension of my analytics background.

🔗 [LinkedIn](https://www.linkedin.com/in/rishika-katna-095a631bb) | [GitHub](https://github.com/rishikakatna)
