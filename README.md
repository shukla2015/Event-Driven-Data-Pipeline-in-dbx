# Event-Driven Data Pipeline in Databricks

An end-to-end **event-driven data engineering pipeline** built using **Databricks (dbx)**. The pipeline ingests raw data across Multi-entity data ingestion, validates and enriches it, and writes clean, merged output to Delta Lake tables.

## 🔧 Tech Stack
- Databricks (Apache Spark)
- Delta Lake
- Python (PySpark)
- Azure Data Lake Storage Gen2

## 📁 Notebooks Overview

| Notebook | Description |
|---|---|
| `customers data stage load` | Validates customer data at file level, then loads into staging table |
| `orders data stage load` | Validates orders data at file level, then loads into staging table |
| `inventory data stage load` | Validates inventory data at file level, then loads into staging table |
| `product data stage load` | Validates product data at file level, then loads into staging tableg |
| `shipping data stage load` | Validates shipping data at file level, then loads into staging table |
| `Data Validation and Cross - Reference` | Validates data quality and cross-references across domains |
| `Data_Enrichment_and_Business_Intelligence` | Applies business logic and enriches data |
| `Final_merge_operation` | Performs final Delta merge/upsert |

## 📌 Key Concepts Covered
- Event-driven pipeline design
- Multi-entity data ingestion from Azure Data Lake Storage Gen2 
- Data validation and cross-reference checks
- Delta Lake merge (upsert) operations
- Business intelligence aggregations

## 🚀 How to Run
1. Import all `.ipynb` notebooks into your Databricks workspace.
2. Configure your ADLS mount points and Delta table paths.
3. Run notebooks in sequence: Stage Load → Validation → Enrichment → Final Merge.

## 👤 Author
Shashank Shukla — [GitHub](https://github.com/shukla2015)
