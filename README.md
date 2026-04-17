# 🏗️ Ecommerce Data Lakehouse Pipeline

## 📌 Overview
This project implements an end-to-end **Data Lakehouse pipeline** using the Medallion Architecture (**Bronze, Silver, Gold**) on Databricks.  
It processes raw ecommerce data into clean, structured, and analytics-ready datasets using PySpark.

---

## 🚀 Architecture

The pipeline follows the **Medallion Architecture**:

### 🔹 Bronze Layer
- Ingest raw CSV data from source systems
- Apply schema enforcement
- Add metadata columns:
  - `_source_file`
  - `ingested_at`

### 🔹 Silver Layer
- Data cleaning and transformation
- Handle missing/null values
- Standardize formats (e.g., date conversion)
- Create structured datasets

### 🔹 Gold Layer
- Build fact and dimension tables
- Perform aggregations for analytics
- Prepare data for reporting and dashboards

---

## 🛠️ Tech Stack

- **Databricks**
- **PySpark**
- **Delta Lake**
- **SQL**
- **GitHub (Version Control)**

---

## 📂 Project Structure
Ecommerce/
│
├── bronze/
│ ├── ingest_orders
│ ├── ingest_products
│
├── silver/
│ ├── transform_orders
│ ├── clean_data
│
├── gold/
│ ├── fact_tables
│ ├── dimension_tables
│
├── schemas/
│ ├── schema_definitions
│
└── README.md


---

## ⚙️ Features

- ✅ Ingest multiple CSV files using PySpark
- ✅ Schema enforcement for consistent data types
- ✅ Metadata tracking for data lineage
- ✅ Data transformation and cleansing
- ✅ Creation of fact and dimension tables
- ✅ Scalable pipeline design using Spark

---

## 📊 Sample Workflow

1. Load raw data from storage (Volumes)
2. Apply schema and ingest into Bronze tables
3. Transform and clean data in Silver layer
4. Build analytics-ready tables in Gold layer

---

## 🧠 Key Learnings

- Implementing **Medallion Architecture**
- Working with **PySpark DataFrame API**
- Handling large datasets in distributed systems
- Managing data pipelines in Databricks
- Using Git for version control in data projects

---

## 🔮 Future Improvements

- Add data quality validation checks
- Implement incremental data loading
- Optimize performance using partitioning
- Integrate dashboards (Power BI / Tableau)
- Automate pipeline using workflows

---

## 👨‍💻 Author

**Chaduer Isaac**

---

## ⭐ Acknowledgment

This project is part of a hands-on data engineering learning journey focused on building real-world data pipelines using modern tools.
