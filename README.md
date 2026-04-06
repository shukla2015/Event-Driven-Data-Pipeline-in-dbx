# Event-Driven Data Pipeline in Databricks

An end-to-end **event-driven data engineering pipeline** built using **Databricks (dbx)**. The pipeline ingests raw data across Multi-entity data ingestion, validates and enriches it, and writes clean, merged output to Delta Lake tables.

## 🔧 Tech Stack
- Databricks (Apache Spark)
- Delta Lake
- Python (PySpark)
- Azure Data Lake Storage Gen2

## 🔄 Pipeline Flow
ADLS (Raw Files)
↓
File-level Validation → Staging Tables (Delta Lake)
↓
Data Validation & Cross-Reference
↓
Data Enrichment & Business Intelligence
↓
Final Merge Operation (Delta Upsert)
↓
Clean Analytics-Ready Delta Tables

## 📁 Repository Structure
Event-Driven-Data-Pipeline-in-dbx/
├── notebooks/
│   ├── customers data stage load.ipynb
│   ├── orders data stage load.ipynb
│   ├── inventory data stage load.ipynb
│   ├── product data stage load.ipynb
│   ├── shipping data stage load.ipynb
│   ├── Data Validation and Cross - Reference.ipynb
│   ├── Data_Enrichment_and_Business_Intelligence.ipynb
│   └── Final_merge_operation.ipynb
└── README.md

## 📁 Notebooks Overview

| Notebook | Description |
|---|---|
| `customers data stage load` | Validates customer data at file level, then loads into staging table |
| `orders data stage load` | Validates orders data at file level, then loads into staging table |
| `inventory data stage load` | Validates inventory data at file level, then loads into staging table |
| `product data stage load` | Validates product data at file level, then loads into staging table |
| `shipping data stage load` | Validates shipping data at file level, then loads into staging table |
| `Data Validation and Cross - Reference` | Cross-references data across all entities and applies quality checks |
| `Data_Enrichment_and_Business_Intelligence` | Applies business logic and enriches validated data |
| `Final_merge_operation` | Performs final Delta Lake merge/upsert into output tables |

## 📌 Key Concepts Covered
- File-level validation before staging table load
- Event-driven pipeline design using Databricks
- Data ingestion from ADLS for multiple business entities (customers, orders, inventory, products, shipping)
- Cross-reference checks across entity datasets
- Delta Lake merge (upsert) operations
- Business intelligence aggregations

## 🚀 How to Run
1. Mount your ADLS container in Databricks and configure the storage paths.
2. Run the five stage load notebooks to validate and load each entity into staging tables.
3. Run `Data Validation and Cross - Reference` for quality and cross-reference checks.
4. Run `Data_Enrichment_and_Business_Intelligence` to apply business logic.
5. Run `Final_merge_operation` to perform the final Delta merge.

## 👤 Author
Shashank Shukla — [GitHub](https://github.com/shukla2015)
