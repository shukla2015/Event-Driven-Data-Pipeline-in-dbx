# Event-Driven Data Pipeline in Databricks

An end-to-end **event-driven data engineering pipeline** built using **Databricks (dbx)**. The pipeline ingests raw data across multiple business domains, validates and enriches it, and writes clean, merged output to Delta Lake tables.

## 🔧 Tech Stack
- Databricks (Apache Spark)
- Delta Lake
- Python (PySpark)
- Azure Data Lake Storage Gen2

## 📁 Notebooks Overview

| Notebook | Description |
|---|---|
| `customers data stage load` | Loads raw customer data into staging |
| `orders data stage load` | Loads raw orders data into staging |
| `inventory data stage load` | Loads raw inventory data into staging |
| `product data stage load` | Loads raw product data into staging |
| `shipping data stage load` | Loads raw shipping data into staging |
| `Data Validation and Cross - Reference` | Validates data quality and cross-references across domains |
| `Data_Enrichment_and_Business_Intelligence` | Applies business logic and enriches data |
| `Final_merge_operation` | Performs final Delta merge/upsert |

## 📌 Key Concepts Covered
- Event-driven pipeline design
- Multi-domain data ingestion
- Data validation and cross-reference checks
- Delta Lake merge (upsert) operations
- Business intelligence aggregations

## 🚀 How to Run
1. Import all `.ipynb` notebooks into your Databricks workspace.
2. Configure your ADLS mount points and Delta table paths.
3. Run notebooks in sequence: Stage Load → Validation → Enrichment → Final Merge.

## 👤 Author
Shashank Shukla — [GitHub](https://github.com/shukla2015)
